CC = gcc
CFLAGS = -Wall -Wshadow -Wunreachable-code -Wredundant-decls -Wdeclaration-after-statement -g -lpthread

target = Writing1

all: pdf

pdf:
	latex main.tex
	dvips -R -Poutline -t letter main.dvi -o main.ps
	ps2pdf main.ps
	rm main.aux
	rm main.dvi
	rm main.log
	rm main.ps
	rm main.out
clean:
	rm -rf *.o Writing1 *~ *.aux *.log *.out *.pyg *.blg *.bbl *.dvi *.ps *.pdf

.PHONY: all pdf
