DOC_DEST_DIR=/Users/2gr/Sites/

all: srs.txt
	@if [ ! -d "www" ]; then echo "Creating Directory"; ln -s \
$(DOC_DEST_DIR) www ; fi
	asciidoc --backend=html -a data-uri -a theme-flask -a toc \
	-a toclevels=4 -a icons -a numbered \
	-o $(DOC_DEST_DIR)/srs.html srs.txt

clean:
	@if [ -e "$(DOC_DEST_DIR)/$(DOCUMENT).html" ]; then \
	rm $(DOC_DEST_DIR)/srs.html; fi

check: 
	@echo "spellcheck srs.txt..."
