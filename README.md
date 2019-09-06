# GIT
GIT tutorial and notes

Link: https://learngitbranching.js.org/
	
Git notes:
<br>
--------------------------------------- Remote ---------------------------------------------------
<br>
- git clone&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;//clone the repository<br>
- git fakeTeamwork |<branch name> /& <num> [optional]|		//plop down a commit on master<br>
- git fetch							//download from remote<br>
- git pull							//short-handed for fetch + merge<br>
	-- rebase						//short-handed for fetch + rebase<br>
- git push							//upload your changes to remote
<br>
	///////////////////////// both push and fectch////////////////////////////<br>
	   origin <place>					//ex: git push origin master (update without checkout, "origin" is usually default)<br>
	   origin <source>:<destination>			//git the commit from source(location ^/~) and upload it (destinaiton is created if not exist)<br>
	   origin :<source>					//delete branch on remote [push], make new branch [fetch]
<br>
--------------------------------------- Other ----------------------------------------------------<br>
- git commit							//save changes<br>
- git branch <new branch name> <location>			//create branch<br>
	     -f <brName> <location>  				//force to change a branch location<br>
	     -u <tracked branch> <new track branch name> 	//set track #2 for already exist[uncommon]<br>
- git checkout <branch name> or HEAD				//move to branch<br>
              + ^ or ^^ or ^<num>				//move to a brand parent or grandparent and <num> to pick which way<br>
	      + ~ or ~<num>					//move up 1 or <num><br>
- git checkout -b <new branch name>				//combine create brand + checkout command<br>
	       -b <new track branch name> <tracked branch>	//set track #1<br>
- git merge <branch name>					//merge work of 2 branches (checkout 1 of them and merge with the other)<br>
- git rebase <branch name>|<pick branch(es)> [optional]|	//move one branch to the ohter (current to named)<br>
	-i <start location>				// give UI to reorganize/not pick commits populate at the location choiced <br>
- git reset <back to location>					//move the branch backware remove previous commit (checkout branch)<br>
- git revert <branch name>					//revert back to the previous but make a new commit instead of remove the precious one (checkout branch)<br>
- git cherry-pick <commit1> <commit2>...			//git the commit from different locations and populate it this the current checkout branch<br>
- git tag <tage name> <branch name>				//create a tage for a branch<br>	
- git describe <brand name>					//give location base parent tag
