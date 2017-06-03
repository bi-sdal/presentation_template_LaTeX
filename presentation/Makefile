clean:
	make clean_temp
	rm -f *.pdf

clean_temp:
	rm -f *.aux *.log *.nav *.out *.snm *.toc *.bbl *blg

presentation.pdf: presentation.tex
	pdflatex presentation.tex
	bibtex presentation.aux
	pdflatex presentation.tex
	make clean_temp
