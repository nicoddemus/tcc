# $Id: Makefile,v 1.1 2003/04/10 23:12:59 gweber Exp $

all: tese.pdf

tese.dvi : tese.tex
	latex --output-directory=output tese
	bibtex --output-directory=output output\tese
	latex --output-directory=output tese
	latex --output-directory=output tese
	
tese.pdf: tese.dvi
	pdflatex --output-directory=output tese

clean:
	rm -f *.aux *.log *.blg *.bbl *.dvi *.ps *.pdf *.toc *.lot *.lof
