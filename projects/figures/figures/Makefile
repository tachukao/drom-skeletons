SUBDIRS := $(wildcard */*.gp)

.PHONY: all clean 

all: 
	for dir in $(SUBDIRS); do \
		cd $$(dirname $$dir) && gnuplot $$(dirname $$dir).gp; \
	done

clean: 
	for dir in $(SUBDIRS); do \
		cd $$(dirname $$dir) && rm *.pdf && latexmk -c; \
	done
      
%.pdf: 
	cd $(*F) && gnuplot $(*F).gp 
