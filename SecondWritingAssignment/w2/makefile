CC = gcc
CFLAGS = -Wall -Wshadow -Wunreachable-code -Wredundant-decls -Wdeclaration-after-statement -g -lpthread

target = w2

all: pdf

pdf:
	latex main.tex
	dvips -R -Poutline -t letter main.dvi -o main.ps
	ps2pdf main.ps
	rm main.aux
	rm main.dvi
	rm main.log
	rm main.ps
clean:
	rm -rf *.o w2 *~ *.aux *.log *.out *.pyg *.blg *.bbl *.dvi *.ps *.pdf

.PHONY: all pdf
