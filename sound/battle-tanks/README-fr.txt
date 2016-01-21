Version b�ta de Battle Tanks
(Les b�ta testeurs peuvent consid�rer que ce fichier est leur manuel.)

Installation :
D�compactez les fichiers dans un r�pertoire quelconque (par exemple, C:\Jeux\Btanks\).

Ce paquet est fourni sans installeur, vous devrez donc utiliser l'invite de commande pour changer de mode de fonctionnement (si n�cessaire), voir la liste ci-dessous.

Le jeu peut fonctionner de deux fa�ons diff�rentes :
1. En utilisant le rendu OpenGL.  Celui-ci tire parti des capacit�s de votre carte graphique.  Les pilotes d'origine de votre carte graphique sont probablement install�s et sont suffisant en g�n�ral.  Si ce n'est pas le cas, les performances risquent d'�tre extr�mement faibles.
2. En utilisant le rendu logiciel.  Cela fonctionne ind�pendamment de la carte graphique utilis�e, au prix d'une baisse mod�r�e de performances.

Param�tres optionnels de la ligne de commande :
--no-gl     d�sactive l'utilisation d'OpenGL (acc�l�ration mat�rielle)
--force-gl  force l'utilisation d'OpenGL, m�me si aucune acc�l�ration mat�rielle n'est d�tect�e.
--fs        active le mode plein �cran (il sera activ� par d�faut � l'avenir)
--lang=XX   force le choix de la langue (XX - un code ISO � deux lettres : en, ru, de, fr)
--vsync     active la synchronisation verticale -- � utiliser en cas de probl�mes d'affichage
--connect=host  se connecte � l'h�te donn� en argument
--no-sound      d�sactive compl�tement le son.
--sound         active le son, m�me s'il est d�sactiv� dans les pr�f�rences (bt.xml).

La r�solution d'�cran peut �galement �tre pr�cis�e :
-0 640x480
-1 800x600 (valeur par d�faut)
-2 1024x768
-3 1152x864
-4 1280x1024

--connect=nomdhote/IP  rejoindre la partie � l'adresse IP ou au nom d'h�te sp�cifi�
--no-sound             d�sactive le son (bruitages et musique)

Les erreurs sont report�es dans le fichier de log "stderr.txt".

