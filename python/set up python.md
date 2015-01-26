##Set up python enviroment for django developers and more
	sudo apt-get install python-setuptools python-dev build-essential
	sudo apt-get install python-pip
	sudo pip install virtualenvwrapper
	mkdir .virtualenvs
	export WORKON_HOME=~/.virtualenvs
	mkdir -p $WORKON_HOME
	source /usr/local/bin/virtualenvwrapper.sh

add to .bashrc
	export WORKON_HOME=$HOME/.virtualenvs
	export PROJECT_HOME=$HOME/Proyectos
	export VIRTUALENVWRAPPER_SCRIPT=/usr/local/bin/virtualenvwrapper.sh
	source /usr/local/bin/virtualenvwrapper_lazy.sh

ready for use pip and virtualenv

	mkvirtualenv env


###related
	[Tutorial Django](https://docs.google.com/presentation/d/1cpCbjrA5cv9igtz76xjcyjxMbxnqfrJRu6Xb02LzV98/edit?usp=sharing)