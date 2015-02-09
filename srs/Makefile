
all: srs.txt
	asciidoc --backend=html -a data-uri -a theme-flask -a toc \
	-a toclevels=4 -a icons -a numbered \
	-o srs.html srs.txt

clean:
	@if [ -e "srs.html" ]; then rm srs.html; fi

check: 
	@echo "spellcheck srs.txt..."
