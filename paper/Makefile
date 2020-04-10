MAIN=paper
SRCS=$(wildcard *.tex *.sty *.bib)

.PHONY: all clean reallyclearn
all: ${MAIN}.pdf
clean:
	latexmk -c && rm comment.cut
reallyclean:
	latexmk -C

%.pdf: %.tex ${SRCS}
	latexmk -pdf $<
