all: clean
	lessc newcircle.less > newcircle.css
	rm -rf newcircle
	mkdir newcircle
	mv *.css newcircle
	zip newcircle.zip newcircle/*

clean:
	rm -rf newcircle *.css *.zip

install: all
	cdk --install-theme=newcircle.zip

