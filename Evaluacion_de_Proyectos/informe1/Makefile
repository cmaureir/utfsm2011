SHELL=/bin/bash
NAME=informe1
BIN=bin

DEPENDENCIES=$(NAME).tex

all:
	@if [ -d bin ];then echo "building..." bin/;else mkdir bin/;fi
	@pdflatex $(NAME).tex
	@pdflatex $(NAME).tex
	@mv $(NAME).pdf bin/
	@make clean

clean:
	@rm -f *.{out,aux,toc,log,bbl,blg,lof,lot} src/*.aux 

distclean: clean
	@rm -rf bin/ 

x:
	xpdf bin/${NAME}.pdf &> /dev/null &

e:
	evince bin/${NAME}.pdf &> /dev/null &

o: 
	okular bin/${NAME}.pdf &> /dev/null &
