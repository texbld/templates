output:
	mkdir output

# change the source file depending on where your essay actually is.
SRC=src/sample.md

output/Submission.pdf: output output/essay.tex
	pdflatex essay
	biber essay
	pdflatex essay
	mv essay.pdf output/Submission.pdf

output/essay.tex: output
	pandoc -o output/essay.tex $(SRC)

PDFTARGETS=output/Submission.pdf

TARGETS=$(PDFTARGETS) output/essay.tex

all: $(TARGETS) junk

clean: junk
	rm -rf $(TARGETS)
	rm -rf output

veryclean: junk clean
	rm -rf output

junk:
	rm -rf `ls essay.* | grep -vE "tex|bib"`
	

.PHONY: all clean junk
