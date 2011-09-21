src=ii-sp

all:
	rubber -d $(src)
	@if [ -d bin ];then mv $(src).pdf bin/;else mkdir bin; mv $(src).pdf bin/;fi

clean:
	rubber --clean ${src}

distclean: clean 
	rm -rf bin/
x:
	okular bin/$(src).pdf &> /dev/null &
