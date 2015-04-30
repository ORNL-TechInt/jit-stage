# No table of contents for this document
all: summary.txt
	asciidoc --backend=html -a data-uri -a theme-flask \
	-o summary.html summary.txt

pdf: summary.txt
	a2x -f pdf -d article --fop summary.txt 

clean:
	@if [ -e "summary.html" ]; then rm summary.html; fi

check: 
	@echo "spellcheck summary.txt...";
	aspell check summary.txt
