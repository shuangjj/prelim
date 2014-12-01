
TEX=latex
BIBTEX=bibtex

DOCNAME=PrelimI-Shuang

all: $(DOCNAME).pdf
	evince $< &

%.pdf: %.dvi
	dvipdf $<

%.dvi: %.tex
	$(TEX) $<
	#$(BIBTEX) $(DOCNAME)
	$(TEX) $<
	$(TEX) $<


clean:
	rm -f *.dvi *.pdf *.log *.aux *.bbl *.blg
