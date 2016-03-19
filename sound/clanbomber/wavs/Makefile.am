EXTRA_DIST = break.wav clear.wav corpse_explode.wav deepfall.wav die.wav explode.wav forward.wav horny.wav hurry_up.wav joint.wav klatsch.wav menu_back.wav putbomb.wav rewind.wav schnief.wav splash1a.wav splash2a.wav stop.wav time_over.wav typewriter.wav whoosh.wav winlevel.wav wow.wav crunch.wav 

.PHONY: files

files:
        @files=s $(DISTFILES) 2> /dev/null ; for p in $$files; do \
	  echo $$p; \
        done
        @for subdir in $(SUBDIRS); do \
	  files=d $$subdir; $(MAKE) files | grep -v "make\[[1-9]\]"; \
          for file in $$files; do \
            echo $$subdir/$$file; \
	  done; \
        done
