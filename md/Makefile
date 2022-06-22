%.pdf:
	pandoc -o $*.pdf $*.md

PDFTARGETS=main.pdf

WORDTARGETS=main.docx

# put main.docx into targets if necessary.

TARGETS=$(PDFTARGETS)

all: $(TARGETS)
	
clean:
	rm -rf $(TARGETS)
