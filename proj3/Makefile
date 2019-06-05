# Project> proj3
# Author: Peter Koprda (xkoprd00)
# Date: April 2019

PROJ=proj3
PACK=xkoprd00-fit
PACKAGES=algorithm2e.sty

.PHONY: clean pack pdflatex

$(PROJ).pdf:$(PROJ).ps
	ps2pdf -sPAPERSIZE=a4 $^

$(PROJ).ps:$(PROJ).dvi
	dvips $^

$(PROJ).dvi:$(PROJ).tex
	latex $^
	latex $^

pdflatex:$(PROJ).tex
	pdflatex $^

pack:clean $(PACK).tar.gz

clean:
	rm -f $(PROJ).aux $(PROJ).dvi $(PROJ).ps $(PROJ).log $^
