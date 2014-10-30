install: newcircle.zip
	cdk --install-theme=newcircle.zip
	cdk --default-theme=newcircle

newcircle.css: newcircle.less
	lessc newcircle.less > newcircle.css

newcircle.zip: newcircle.css
	rm -rf newcircle
	mkdir newcircle
	cp *.css newcircle
	zip newcircle.zip newcircle/*
	rm -rf newcircle

clean:
	rm -rf newcircle *.zip

purge:
	rm -rf newcircle *.css *.zip

