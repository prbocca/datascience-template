TARGET = main
TEXFILES = $(wildcard *.tex)
BIBFILES = $(wildcard *.bib)
EPSFILES = $(patsubst %.fig,%.eps,$(wildcard *.fig))

all: clean 
	make $(TARGET).pdf 

%.pdf: $(TEXFILES) $(BIBFILES)
	pdflatex $(TARGET).tex $@ && pythontex $(TARGET).tex   && makeindex main.idx -s styleInd.ist && biber $(TARGET) && pdflatex $(TARGET).tex $@ && pdflatex $(TARGET).tex $@

%.ps: %.dvi
	dvips -o $@ $<

%.dvi: $(TEXFILES) $(EPSFILES)
	latex $(TARGET).tex
	bibtex $(TARGET)
	latex $(TARGET).tex
	latex $(TARGET).tex

%.eps: %.fig
	fig2dev -L eps $< > $@

clean:
	-rm $(TARGET).ps *.dvi *.aux *.bbl *.blg *.log *.out *.tex.backup *.tex~ *.bib~ $(TARGET).bcf $(TARGET).idx $(TARGET).ilg $(TARGET).ind $(TARGET).ptc $(TARGET).toc $(TARGET).run.xml $(TARGET)-concordance.tex $(TARGET).pdf

force:
	gmake clean
	gmake all

tar:
	-rm $(TARGET).tar $(TARGET).tar.gz
	tar cvf $(TARGET).tar Makefile *.tex *.fig *.bib
	gzip $(TARGET).tar
  


