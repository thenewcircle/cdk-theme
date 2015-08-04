cdk-theme
=========

NewCircle's theme for use with twitter's courseware development kit (CDK). The code example below works on Ubuntu 12.04 and 14.04 LTS. They should work for MacOS as well. I am looking for a volunteer to submit instructions for Windows based cdk authoring environments.  vcdk refers to the name of a Python virtual environment. Substitute the name of your virtual environment if different or omit the source line altogether if you do not use a Python virtual environment.

### Install NewCircle CDK Theme Without NodeJS Less (lessc) 
Use these instructions If you do not need to make updates to theme's CSS file.
	
    $ cd ~
    $ git clone https://github.com/thenewcircle/cdk-theme.git
    $ cd cdk-theme/newcircle
    $ source ~/vcdk/bin/activate       
	(vcdk) $ cdk install theme=newcircle.zip
    (vcdk) $ cdk --default-theme=newcircle


### Install NewCircle CDK Theme With Less for CSS Modification
If you need to modify the theme, install lessc before regenerating the theme by calling make. The Makefile contains calls to lessc.
    
    $ git clone https://github.com/thenewcircle/cdk-theme.git
    $ cd cdk-theme/newcircle
    $ source ~/vcdk/bin/activate
    (vcdk) $ make install

If this is your first time installing the newcircle theme, set it as the default theme as well.    
    
    (vcdk) $ cdk --default-theme=newcircle


### Dependencies
This project uses lessc to reduce the size of css files. 

#### Install on Ubuntu 12.04
    sudo apt-get install lessc

#### Install on Ubuntu 14.04
Note, if you intend to develop using NodeJS on Ubuntu 14.04, you should review the posts on Stack Overflow describing the differences in the NodeJS versions available. This README file assumes one just wants a copy of lessc on the command line.

    sudo apt-get install nodejs-legacy
    sudo npm install -g npm   # update npm
	sudo npm install -g less less-plugin-clean-css

#### Install on Windows 
Please submit if you have a solution.

#### Install on MacOS
The easiest way is to use a package manager such as HomeBrew

    $ brew install npm
    $ npm install --global less

Make sure that the /usr/local/bin/ directory is in your PATH, or equivalent, before running the make install command. 
