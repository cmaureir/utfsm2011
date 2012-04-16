src=ppaa-sp

all:
	rubber -d $(src)

clean:
	rubber --clean ${src}

distclean: clean
	rm -rf bin/
x:
	okular bin/$(src).pdf &> /dev/null &
