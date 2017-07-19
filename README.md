# Git-Cheat
### Basic Commands
```rm -rf <directory name>: removes non-empty directory.
HEAD: is a pointer that refers to the tip of the current checked out branch
git status:
git diff: shows differences between file changes; difference between repository and the working directory.

```
### Add and Commit in One Step
'git commit -am 'message'': passes staging process; works well for modifications, not new or untracked files.


### Branching: 
```
Allows to try new ideas on branch without changing master branch
cat .git/HEAD: 
ls -la .git/refs/heads:
git branch new_branch: creates new branch; this branch has all the stuff master contains.
git checkout <name of branch>: switches branches
  -When you create a new branch you can make changes to it without changing the master content. Use
    checkout to switch back and forth. When you go back to master the new branch changes wont reflect. cool.
**Create and switch branches**
git checkout -b <new name>: it creates and checks out branch all at the same time.
  -it will include whatever branch you created from in the new branch created.
  - modified files should be clean before you can switch branches
git diff master..<new branch>: will show the different changes made.
git branch --merged: shows what branches have merged changes
** Rename Branches**
git -m <old name> <new name>: renames branches
** Delete Branch **
git branch -d <name of branch to delete>:
```
**CHAP 11 MERGING**
