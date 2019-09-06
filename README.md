# GIT
GIT tutorial and notes

Link: https://learngitbranching.js.org/
	
Git notes:
<br>
--------------------------------------- Remote ---------------------------------------------------
- git clone							//clone the repository
- git fakeTeamwork |<branch name> /& <num> [optional]|		//plop down a commit on master
- git fetch							//download from remote 
- git pull							//short-handed for fetch + merge
	-- rebase						//short-handed for fetch + rebase
- git push							//upload your changes to remote
	///////////////////////// both push and fectch////////////////////////////
	   origin <place>					//ex: git push origin master (update without checkout, "origin" is usually default)
	   origin <source>:<destination>			//git the commit from source(location ^/~) and upload it (destinaiton is created if not exist)
	   origin :<source>					//delete branch on remote [push], make new branch [fetch]
<br>
--------------------------------------- Other ----------------------------------------------------
- git commit							//save changes
- git branch <new branch name> <location>			//create branch
	     -f <brName> <location>  				//force to change a branch location
	     -u <tracked branch> <new track branch name> 	//set track #2 for already exist[uncommon]
- git checkout <branch name> or HEAD				//move to branch
              + ^ or ^^ or ^<num>				//move to a brand parent or grandparent and <num> to pick which way
	      + ~ or ~<num>					//move up 1 or <num>
- git checkout -b <new branch name>				//combine create brand + checkout command
	       -b <new track branch name> <tracked branch>	//set track #1
- git merge <branch name>					//merge work of 2 branches (checkout 1 of them and merge with the other)
- git rebase <branch name>|<pick branch(es)> [optional]|	//move one branch to the ohter (current to named)
	     -i <start location>				// give UI to reorganize/not pick commits populate at the location choiced 
- git reset <back to location>					//move the branch backware remove previous commit (checkout branch)
- git revert <branch name>					//revert back to the previous but make a new commit instead of remove the precious one (checkout branch)
- git cherry-pick <commit1> <commit2>...			//git the commit from different locations and populate it this the current checkout branch
- git tag <tage name> <branch name>				//create a tage for a branch
- git describe <brand name>					//give location base parent tag
