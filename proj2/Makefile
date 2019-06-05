#Project:proj2
#Name:Peter Koprda
#Date:18.03.2019

PROJ=proj2
PACK=xkoprd00-fit

.PHONY: clean pack pdflatex

pdflatex:$(PROJ).tex
	pdflatex $(PROJ).tex
	pdflatex $(PROJ).tex

pack:$(PACK).tar.gz

clean:
	rm -f $(PROJ).aux $(PROJ).dvi $(PROJ).log $(PROJ).ps $(PROJ).synctex.gz $(PROJ).fls $(PROJ).fdb_latexmk
