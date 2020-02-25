FIG=$(wildcard fig/*.fig)
FIG2PDF=$(FIG:.fig=.pdf)


NAME=main
PDF=$(NAME).pdf
SOURCE=$(NAME).tex


all: $(PDF)  

bib: $(SOURCE)
	pdflatex  $<
	bibtex $(NAME)
	pdflatex  $<

%.pdf: %.tex
	pdflatex  $<

%.pdf: %.fig
	fig2dev -L pdf $< > $@


clean:
	rm -f *~ $(FIG2PDF) ${NAME} main.pdf *.tmp
