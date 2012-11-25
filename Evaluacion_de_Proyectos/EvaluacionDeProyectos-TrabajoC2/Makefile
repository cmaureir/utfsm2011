SHELL=/bin/bash
NAME=tc2
BIN=bin

DEPENDENCIES=$(NAME).tex

all: $(NAME).tex
	@if [ -d bin ];then echo "building..." bin/;else mkdir bin/;fi
	@rubber -d $(NAME)
	@mv $(NAME).pdf bin/
	@make clean

clean:
	@rm -f *.{out,aux,toc,log,bbl,blg,lof,lot} src/*.aux *~ src/*~ 

distclean: clean
	@rm -rf bin/ 

x: 
	okular bin/${NAME}.pdf &> /dev/null &
