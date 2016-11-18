# Git basic commands
List of basic commands to start git

### 1: git clone

Create a working copy of a local repository

`git clone /path/to/repository`


### 2: git add

`git add -u` Adds only currently tracked files.

`git add -A` Adds all modified, deleted & new files in the working tree to stage


### 3: git commit

`git commit -m "Commit message"` - Commit files added to staging

**Commit message should be:**

* Discriptive
* Lowercase
* Present tense

**Add new changes to an existing commit?**

`git commit --amend` - If you already pushed the commits to remote repo. you shouldn't perform this command


### 4: git pull

`git pull origin <branchname>` - Fetch and merge changes on the remote server to your working directory.

`git branch origin <branchname> --rebase` - Reapply your local commits on top of remote commits


### 5: git push

`git push origin <branchname>` - Pushes your local commit in a branch to remote

`git push --all origin` - Push to all branches to your remote repository


### 6: git status

`git status` - Gives the current status of your current working tree(ex: modified, deleted, newly created files, .. )


### 7: git branch

`git branch` - List all the branches

`git checkout -b <branchname>` - Create a new branch and switch to it

`git checkout <branchname>` - Switch from one branch to another

`git branch -d <branchname>` - Delete the feature branch


### 7: git log

`git log` - Git log list the commits made in that repository in reverse chronological order

`git log --oneline` - prints only commit message


### 8: git reset

`git reset --hard` - Revert to a previous commit, ignoring any changes


### 9: git stash

`git stash`

**warning** - The command saves your local modifications away and reverts the working directory to match the HEAD commit.

`git stash apply`

**warning** - This command brings latest stashed changes to working directory
