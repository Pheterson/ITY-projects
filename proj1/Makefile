# 
# Project:Project 1
# Author: Peter Koprda
# Date:   04.03.2019

PROJ=proj1
PACK=xkoprd00-fit

.PHONY: clean pack pdflatex

$(PROJ).pdf: $(PROJ).ps
	ps2pdf $(PROJ).ps

$(PROJ).ps: $(PROJ).dvi
	dvips $(PROJ).dvi

$(PROJ).dvi: $(PROJ).tex
	latex $(PROJ).tex

$(PACK).tar.gz:$(PROJ).tex
	tar -czf $(PACK).tar.gz Makefile $(PROJ).tex

pdflatex:$(PROJ).tex
	pdflatex:$(PROJ).tex

pack:$(PACK).tar.gz

clean:
	rm -f $(PROJ).aux $(PROJ).dvi $(PROJ).log $(PROJ).ps $(PROJ).syntex.gz $(PROJ).fls $(PROJ).fdb_latexmk
