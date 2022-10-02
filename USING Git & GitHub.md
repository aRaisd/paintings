Git - a distributed Version Control System  (VCS)

1- INSTALL Git - go to  git-scm.com

2- FIRST SETUP, SET CONFIG VALUES (to configure username, password and email on local repo ) 
  - git --version (to check version)
  - git config --global user.name "GeeksforGeeks"
  - git config --global user.password "1234321"
  - git config --global user.email "GFGexample@gmail.orgg"
  - git config --list --show-origin
  - usefull commands:
    - git help <verb>  /  git <verb> --help
    - git status              - shows the branch, changes to be committed and untracked files
    - touch .gitignore        - to list the files to be ignored
    - git add -A              - add all files to staging area
    - git add .gitignore      - add .gitignore to staging area
    - git reset .gitignore    - to remove .gitignore from staging area
    - git commit -m "message" - to commit, which adds the files in the stage area to the repo    
    - git log                 - display the commits made, hash number, the Auther, date and the message for each ccommit
    - git clone <url> <where to clone>  - cloning from a remote repo <url>
    - git clone ../remote_repo.git .    - cloning from a remote repo
    - git remote -v											- viewing info about the remote repo
    - git branch -a
    - git diff								- shows changes made, '-' in red are codes remooved. '+' in green are codes added

3- TYPICAL WORKFLOW
	
	- git branch calc-div 		- create a branch 'cal-div' from the master branch
	- git checkout calc-div	 	- change branch cal-div
	- git diff
	- git status
	- git add -A 			- adds changes to staginng  area
	- git commit -m "message"	- commits the changes to the local branch calc-div! No effect on the master branch / remote repo 
	- git pull origin master
	- git push origin master
	

	
		 											
	
  

======================================================================
  
  
GETTING STARTED USINNG GIT  2 SCENERIOS - (to track changes)  

SCENERIO 1 - Existing Project on local repository
----------------------
  a) INITIALIZE A REPOSITORY from existing code
    $ git init  - creates a '.git' file (on Git CMD  in the project folder)


SCENERIO 2 - Existing Project on remote repository ( on Github):  paintings
---------------------------------------------------------------------
  a) Created README.md file
  b) Copied https://github.com/aRaisd/paintings.git (for HTTPS from Code 'drop down')
  c) On local repository:
    - Create a paintings folder.
    - In Git-CMD Type: git clone https://github.com/aRaisd/paintings.git .
