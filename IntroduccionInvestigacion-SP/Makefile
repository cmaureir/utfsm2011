src=ii-sp

all:
	rubber -d $(src)
	@if [ -d bin ];then mv $(src).pdf bin/;else mkdir bin; mv $(src).pdf bin/;fi

clean:
	rm -f  src/*.{aux,log}
	rm -f $(src).{aux,log,bbl,blg,out}
	rm -f  src/*.{aux,log}        	
distclean: clean 
	rm -rf bin/
x:
	okular bin/$(src).pdf
