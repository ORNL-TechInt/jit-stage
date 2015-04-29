
all: summary.txt
	asciidoc --backend=html -a data-uri -a theme-flask -a toc \
	-a toclevels=4 -a icons -a numbered \
	-o summary.html summary.txt

clean:
	@if [ -e "summary.html" ]; then rm summary.html; fi

check: 
	@echo "spellcheck summary.txt..."
