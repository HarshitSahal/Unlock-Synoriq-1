# Unlock-Synoriq-1
1. Git and GitHub
-  Git is an open-source distributed version contol system which is used to track changes in files & helpful when working in team. Git can be used with github to get remote repository 
   and visual interface to our repositories. Using git we can access our remote repositories online to github. We can work on our poject offline and push file/folder into git or we can clone 
   or pull previous saved files to work offline using github.

2. Basic commands in Git
-  'git --version'							       -> Show version of git installed
-   git init 								          -> Create a new git repository
-   git status 								          -> Displays the state of the working directory
-   git add 									          -> Adds a change in the working directory
-   git commit -m "....." 					       -> Used for saving changes with message
-   git config --global user.email "email.id"  -> Adds an email with repository
-   git config --global user.name "username"   -> Adds an username with repository
-   git remote add origin <link of repository> ->  Add a new remote
-   git push -u origin master 				       -> Push file to master
-   git log 									          -> Check log of repository
-   git --help 								          -> For help

3. Branching and Merging
-  Branching is process to create, list, rename, and delete branches from our repository.
  
   Commands:
 -  git branch <branch name> 				       -> Creates branch 
 -  git checkout <branch name> 				    -> takes us to the branch

-  Merging is used to merge two branches. 
  
   Commands:
 -  git merge <branch name> 					    -> Merge branch to master
 -  git branch -d <branch name> 				    -> Delete branch from local
 -  git push origin --delete <branch name> 	 -> Delete branch from remote

4. Git Tags
-  Tags are reference that point to specific points in Git history.
   
   Commands:
-   git tag <tag name> 						     -> Creates a tag
-   git tag -a <tag name> -m "message" 		  -> Creates an annotated tag
-   git tag 									        -> To check creted tags
-   git show <tag name> 						     -> To check details of particular tag
-   git tag -l <char>.* 						     -> To show tags stating with character
   git push origin <tag name> 				  -> To push tag in remote
   git push --tags 							     -> Push all tags once in remote
   git tag -d <tag name> 					     -> Delete tag from local
   git tag --delete <tag name> 				  -> Delete tag from local
   git push origin -d <tag name> 			  -> Delete tag from remote
   git push origin --delete <tag name> 	  -> Delete tag from remote
   git tag -d <tag names> 					     -> Delete multiple tags from local
   git push origin -d <tag names> 			  -> Delete multiple tags from remote
   git checkout -b <branch name> <tag name> -> Create a branch from tag and checkout the branch
   git tag <tag name> <reference of commit> -> Create a tag from past commit
   
5. Difference between Merge and Rebase
-  git merge
   . It is a non-destructive operation.
   . Existing branches are not changed.
   . It adds a new commit, preserving complete history and chronological order.
   
   git rebase
   . It is a command that allows developers to integrate changes from one branch to another.
   . It moves the entire feature branch to begin on the tip of the master branch.
   . It cleans intermediate commits by making them a single commit, which can be helpful for DevOps teams.
