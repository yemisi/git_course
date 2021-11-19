git markdown cheatsheet: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
```
* git config --global user.name "USERNAME"
* git config --global user.email "USERNAME@EMAIL.COM"
* git init . //create and initialize a directory as a git repository
* git add <file name>  //add a file to the staging area 
* git add . 
* git commit -m "Commit information"  //commit/save your file(s) in staging area to your local git repo
* git status 
* git log 
```
#### To push an existing repository from the command line to new remote repo
```
* git remote add origin "GITHUB_REPO_URL" // before you can push to a remote repo, the remote and local repo need to be linked via .git/config file 
EXAMPLE: git remote add origin git@github.com:yemisi/testrepo.git
* git push -u origin <branch> // push local changes on current branch to remote repo (aka origin) where branch is the remote branch name. Push your code when you have changes not present in the remote repository. Code has to be commited to your local repository first.
```

```
* git clone <remote_repo>  // clone remote repo into local system when the local repo doesnt exist
* git pull origin master // pull any changes that exist on the remote repo that is not on your local repository. The local repository already exists, you are just making your repo sync with the remote repo
```

#### Undo changes in working directory
```
* git restore <file_name> // undo changes in specified file in the working directory
* git restore . // undo all changes in the working directory  
* git checkout -- <filename> // undo changes in specified file in the working directory
* git checkout -- . // undo changes in all files in the working directory
```
#### Undo changes in staging area 
```
* git restore --staged <file_name>  #unstage files from Staging area to working directory  
* git restore <file_name> #then use git restore to undo changes from working directory  
```
#### Undo changes in local repository if not commited to remote repository
```
* git reset HEAD~ #same as HEAD~1. It reverts changes from local repo to working directory. NOTE that the last commit will be removed, so use on private not public/main branch
* git restore <file_name> #then use git restore to undo changes from the working directory  
```

```
* git reset HEAD <filename> //unstage a file 
* git reset HEAD . //unstage all changes 
* git reset HEAD~N (N is number of commits to revert) //revert commits on local repository
* git checkout HEAD~1
```

```
* git checkout <commit_id> file // to get a file from previous commit  
* git checkout <commit_id> // move to previous commit 
* git rebase -i HEAD~N (N is number of commits to squash) // to combain multiple comments as a single. 
```

#### View details about each commit
```
* git annotate <file-name> //shows who wrote each line of a file
* git show <commit-id> 
* git show HEAD
* git show HEAD~1 
``` 

```
* git checkout <branch_name>
* git branch --set-upstream-to=origin/master master
* git branch <branch_name> // to create a new branch
* git checkout -b <branch_name> // to create new branch and switch to branch 
* git merge <source_branch> <dest_branch> 
* git branch -d <branch_name> // to delete a branch
* git branch --set-upstream-to=origin/master master
```
