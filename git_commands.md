git markdown cheatsheet: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
* git config --global user.name "USERNAME"
* git config --global user.email "USERNAME@EMAIL.COM"
* git init . //create and initialize a directory as a git repository
* git add <file name>  //add a file to the staging area 
* git commit -m "Commit information"  //commit/save your file(s) in staging area to your local git repo
* git status 
* git log 
* git remote add "remote_repo"  // add remote repo to local system
* git clone <remote_repo>  // clone remote repo into local system when the local repo doesnt exist
* git pull origin master // pull any changes that exist on the remote repo that is not on your local repository. The local repository already exists, you are just making your repo sync with the remote repo
* git push origin master // push local changes on master branch to remote (same as origin) master (same master in command) branch. Push your code when you have changes not present in the remote repository. Code has to be commited to your local repository first.
* git checkout -- //undo changes in the working directory
* git checkout -- . // undo changes in the working directory
* git restore <file_name> // undo changes in the working directory
* git restore . // undo changes in the working directory
* git checkout <branch_name>
* git checkout <commit_id> file // to get a file from previous commit  
* git annotate <file-name>
* git branch --set-upstream-to=origin/master master
* git reset HEAD~N (N is number of commits to revert) //revert commits on local repository
* git checkout <branch_name>
* git checkout HEAD~1
* git rebase -i HEAD~N (N is number of commits to squash) // to combain multiple comments as a single. 
* git config --global user.name "USERNAME"
* git config --global user.email "USERNAME@EMAIL.COM"
* git push origin master
git remote add origin "GITHUB_REPO_URL"
* git add "<filename>" / git add . 
* git push origin <branch>
* git checkout -- <filename> // to revert changes from git working directory area
* git reset HEAD <filename> //unstage a file 
* git checkout <commit_id> <filename> // move to previous commit 
* git reset HEAD . //unstage all changes 
* git show <commit-id> 
* git show HEAD
* git show HEAD~1
* git annotate <filename>
* git branch --set-upstream-to=origin/master master
* git branch <branch_name> // to create a new branch
* git checkout -b <branch_name> // to create new branch and switch to branch 
* git merge <source_branch> <dest_branch> 
* git branch -d <branch_name> // to delete a branch
