// Extracted using following script

Path = '/path/to/a_wave2.res'
Dst = '/path/to/output/folder'
Ext = '.wav'

Bs = Path.get
N = Bs.take{2}.u2
ESize = 9+4
Es = map E Bs.drop{2}.take{N*ESize}.group{ESize}
     | [E.take{8}.utf8 E.drop{9}.u4 0]

Es.(N-1).2 <= Bs.size - Es.(N-1).1
for I N-1:
| K = N-I-2
| Es.K.2 <= Es.(K+1).1 - Es.K.1

for Name,Offset,Size Es: "[Dst]/[Name][Ext]".set{Bs.drop{Offset}.take{Size}}