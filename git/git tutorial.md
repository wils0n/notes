##Install git in ubuntu  
	sudo apt-get install git
	git config --global user.name "aaaa"
	git config --global user.email "aaaa@gmail.com"
	ssh-keygen
	enter
	enter

##add key to github or bitbucket  
	copy code from ~/.ssh/id_rsa.pub to SSH keys in GitHub or Bitbucket

##create project and first commit
	git init
	git add .
	git commit -m "first commit"
	git remote add origin git@github:wils0n/pythonadas...
	git push origin master
