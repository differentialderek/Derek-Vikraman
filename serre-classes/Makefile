all: main.pdf TAGS
main.pdf:always; latexmk -pdf main
always:
clean:; rm -f *.aux *.fdb_latexmk *.fls *.log *.out *.toc *.brf *.blg *.bbl
veryclean:clean; rm -f *.pdf
ZTors.pdf:always; latexmk -pdf ZTors

BOOKFILES :=                                            \
	main.tex                                        \

TAGS : Makefile *.tex
	etags $(BOOKFILES)
