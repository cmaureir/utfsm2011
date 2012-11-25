SRC=music-labs

all:
	@pdflatex $(SRC).tex
	@pdflatex $(SRC).tex
	@echo "moviendo PDF al directorio bin/ "
	@mkdir -p bin/
	@mv $(SRC).pdf bin/
	@rm -rf *.{aux,log,dvi,ps,out,toc,nav,snm,vrb}

x:
	xpdf bin/$(SRC).pdf &> /dev/null

clean:
	@echo "limpiando..."
	@rm -rf *.{aux,log,dvi,ps,out,toc,nav,snm,vrb}
	@rm -rf src/*.{aux,log,dvi,ps,out,toc,nav,snm,vrb}

distclean: clean
	@ echo "borrando PDF..."
	@rm -rf *.pdf bin/*.pdf
