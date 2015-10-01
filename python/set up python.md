#Set up python enviroment for django developers and more

##Install dependencies importants

	sudo apt-get install python-setuptools python-dev build-essential

##Install pip in ubuntu

	sudo apt-get install python-pip

##Install pip in osx

	sudo easy_install pip

##Install virtualenv and virtualenvwrapper in both

	sudo pip install virtualenv
	sudo pip install virtualenvwrapper
	cd $HOME
	mkdir .virtualenvs
	atom .bash_login  (open or create file .bash_login)

##add the follow line to .bash_login

	source /usr/local/bin/virtualenvwrapper.sh

##Add three lines to your shell startup file in .bashrc

	export WORKON_HOME=$HOME/.virtualenvs
	export PROJECT_HOME=$HOME/name_user
	source /usr/local/bin/virtualenvwrapper.sh

> with this allow change path (where virtualenvs creates) for virtualwrapper


##ready for use pip and virtualenv

	mkvirtualenv env


###Related

[Git CSM](https://git-scm.com/book/es/v1/Empezando-Instalando-Git)
[Tutorial Django](https://docs.google.com/presentation/d/1cpCbjrA5cv9igtz76xjcyjxMbxnqfrJRu6Xb02LzV98/edit?usp=sharing)
[Jamie Curle Tutorial](http://jamie.curle.io/posts/installing-pip-virtualenv-and-virtualenvwrapper-on-os-x/)
[virtualenvwrapper Documentation](http://virtualenvwrapper.readthedocs.org/en/latest/install.html/)
