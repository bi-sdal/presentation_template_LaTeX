# SDAL LaTeX Pressentation Template

This is the LaTeX presetnation originally created by Emily Molfino when she was a 
post-doc in the lab ~2016.

# How to use this template

All files are located in the `presentation` directory.

The `presentation.tex` is the presentation LaTeX file.

> There are comments and notes in this file on how to use the document.

Bibtex entries are placed in `bib.bib`.

Figures are placed in the `figures` directory,
and referenced in the `tex` file using `figures/my_figure`

## Compile the presentation

`cd` into the `presention` directory.

then run:
```
	pdflatex presentation.tex
	pdflatex presentation.tex
```
You will need to do this twice if you want the progress bar to be rendered correctly
(this is also discussed within the comments in `presentation.tex`)

## Compile the presentation with bibtex references

`cd` into the `presentation directory

```
	pdflatex presentation.tex
	bibtex presentation.aux
	pdflatex presentation.tex
```

# Using the `Makefile`

A make file has been created to run the above commands automatically.

First, `cd` into the presentation, then you can run one of the below commands

- `make presentation.pdf` will fully render the presentation with the correct progressbar and bibliography
- `make clean` will delete all files created by `LaTeX` so you can start a clean compile
- `make clean_teamp` will remove all the temporary files created during the compiling process
