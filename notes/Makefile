all: setup build clean

setup:
	mkdir -p .build
	cp -rv python-notes.bib python-notes.tex chapters .build

build:
	cd .build && \
	  latexmk -pdf -xelatex python-notes.tex && \
	  cp python-notes.pdf ..

clean:
	rm -rf .build
