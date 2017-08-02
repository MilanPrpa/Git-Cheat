# Git-Cheat
### Basic Commands
`rm -rf <directory name>`: removes non-empty directory.

`HEAD:` is a pointer that refers to the tip of the current checked out branch

`git status`:

`git diff`: shows differences between file changes; difference between repository and the working directory.


### Add and Commit in One Step
`git commit -am 'message'`: passes staging process; works well for modifications, not new or untracked files.


### Branching: 
Allows to try new ideas on branch without changing master branch
`cat .git/HEAD`: 

`ls -la .git/refs/heads`: shows branches in repository

`git branch new_branch`: creates new branch; this branch has all the stuff master contains.

`git checkout <name of branch>`: switches branches

  #### When you create a new branch you can make changes to it without changing the master content. Make sure to commit 
  modified file. It wont reflect in the master.
  Use checkout to switch back and forth. When you go back to master the new branch changes wont reflect. cool.

**Create and switch branches**

`git checkout -b <new name>`: it creates and checks out branch all at the same time.
  -it will include whatever branch you created from in the new branch created.
  - modified files should be clean before you can switch branches

`git diff master..<new branch>`: will show the different changes made.

`git branch --merged`: shows what branches have merged changes
** Rename Branches**

`git -m <old name> <new name>`: renames branches

** Delete Branch **

`git branch -d <name of branch to delete>`:

### Merging Branches

1. checkout branch things are being recieved too.
`git merge <name of file you are merging>`: fast-forward
2. True Merge
3. Merge Conflicts: making changes to new branch then going to master and commiting changes there as well.
4. Resolving conflicts  
  a. abort option `git merge --abort`:
5. `git log --graph --oneline --all --decorate`: graph of all branches and merges

### Remotes

1. Create repo in GitHub w/out Readme.

2. `git remote add origin <url>`: adds GitHub

3. `git remote -v`
   `cat .git/config`:
   `git remote rm origin`: removes remote
   
4. `git push -u origin master`: push up to github

### Clone Remote Repository: brings remote repository to my machine.
1. `git clone <remote url>`:

### Tracking remote branches

`cat .git/config`:

### Pushing changes to remote repo
`git push`: able to do this because this branch is tracked using -u

`git log --oneline origin/master`: will show the push

### Fetching changes to a remote repo













