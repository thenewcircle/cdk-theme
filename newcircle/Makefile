all: clean
	lessc newcircle.less > newcircle.css

clean:
	rm -rf newcircle *.css *.zip

install: all
	rm -rf newcircle
	mkdir newcircle
	mv *.css newcircle
	zip newcircle.zip newcircle/*
	cdk --install-theme=newcircle.zip

