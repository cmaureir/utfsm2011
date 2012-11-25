SHELL=/bin/bash
NAME=informeFinal
BIN=bin

DEPENDENCIES=$(NAME).tex

all: $(NAME).tex
	@if [ -d bin ];then echo "building..." bin/;else mkdir bin/;fi
	@pdflatex $(NAME).tex
	@pdflatex $(NAME).tex
	@mv $(NAME).pdf bin/
	@make clean
	@evince bin/$(NAME).pdf &

clean:
	@rm -f *.{out,aux,toc,log,bbl,blg,lof,lot} src/*.aux *~ src/*~ 

distclean: clean
	@rm -rf bin/ 

x: 
	xpdf bin/${NAME}.pdf &> /dev/null &

e: 
	evince bin/${NAME}.pdf &> /dev/null &

o: 
	okular bin/${NAME}.pdf &> /dev/null &
