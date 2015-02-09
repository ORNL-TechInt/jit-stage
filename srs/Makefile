#DOC_DEST_DIR=/Users/2gr/Sites/
DOC_DEST_DIR=www/
DOCUMENT=SRS

all: srs.txt
	asciidoc --backend=html -a data-uri -a theme-flask -a toc \
	-a toclevels=4 -a icons -a numbered \
	-o $(DOC_DEST_DIR)/$(DOCUMENT).html srs.txt

clean:
	rm $(DOC_DEST_DIR)/$(DOCUMENT).html

check: 
	@echo "spellcheck srs.txt..."
