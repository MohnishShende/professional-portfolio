.PHONY: all clean compile text

all: compile text

compile:
	mkdir -p compiled
	xelatex -interaction=nonstopmode -halt-on-error cv.tex
	xelatex -interaction=nonstopmode -halt-on-error cv.tex
	mv cv.pdf compiled/mohnish-shende-cybersecurity-cv.pdf

text: compile
	pdftotext compiled/mohnish-shende-cybersecurity-cv.pdf compiled/cv.txt

clean:
	rm -f cv.aux cv.log cv.out cv.toc cv.synctex.gz cv.fls cv.fdb_latexmk
	rm -rf compiled
