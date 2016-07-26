all: setup build clean

setup:
	mkdir -p .build
	cp -rv python-notes.bib python-notes.tex chapters code listings .build

build:
	cd .build && \
	  latexmk -pdf python-notes.tex && \
	  cp python-notes.pdf ..

clean:
	rm -rf .build
