.PHONY : all clean tex pdf view

all: tex pdf

tex: slides.tex

pdf: slides.pdf

slides.tex: slides.txt Makefile
	wiki2beamer slides.txt > slides.tex
	
slides.pdf: slides.tex Makefile
	pdflatex slides.tex

clean:
	rm -f slides.aux slides.log slides.nav slides.out slides.pdf slides.snm slides.tex slides.toc
