cdk-theme
=========

NewCircle's theme for use with twitter's courseware development kit (CDK)


### Install NewCircle theme in cdk 
The code example below works on Ubuntu 12.04 LTS and should work for MacOS as well. vcdk refers to the name of python virtualenv. Susbitute the name of your virtualenv if it differs or omitt the source line all together if you do not use
python virtualenv. 
    
    $ git clone 
    $ cd cdk-theme/newcircle
    $ source ~/vcdk/bin/activate
    (vcdk) $ make install

If this is your first time installing the newcircle theme, set it as the default theme as well.    
    
    (vcdk) $ sudo cdk --default-theme=newcircle
