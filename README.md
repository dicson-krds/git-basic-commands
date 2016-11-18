# Git basic commands
List of basic commands to start git

### 1: git clone

Create a working copy of a local repository

```html
git clone /path/to/repository
```


### 2: git add

**git add -u** - Adds only currently tracked files.

```html
git add -u
```

**git add -A** -  Adds all modified, deleted & new files in the working tree to stage

```html
git add -A
```

### 3: git commit
Commit files added to staging

```html
git commit -m "Commit message"
```
**Commit msg should be:**
* Commit message should be discriptive
* Lowercase
* Present tense

Add new changes to an existing commit?

git commit --amend

**Note:** If you already pushed the commits to remote repo. you shouldn't perform this command

### 4: git pull

Fetch and merge changes on the remote server to your working directory.

```html
git pull origin <branchname>
```

**pull rebase** - Reapply your local commits on top of remote commits
```html
git branch origin <branchname> --rebase
```

### 5: git push

git push origin <branchname>
**Note:** Pushes your local commit in a branch to remote

git push --all origin
**Note:** Push to all branches to your remote repository

### 6: git status

Gives the current status of your current working tree(ex: modified, deleted, newly created files, .. )

```html
git status
```

### 7: git branch

**Branch list** - List all the branches
```html
git branch
```

**Add Branch** - Create a new branch and switch to it
```html
git checkout -b <branchname>
```

**Switch Branch** - Switch from one branch to another
```html
git checkout <branchname>
```

**Delete Branch** - Delete the feature branch
```html
git branch -d <branchname>
```

### 7: git log

$ git log
**Note:** Git log list the commits made in that repository in reverse chronological order

git log --oneline
**Note:** prints only commit msg


### 8: git reset

Revert to a previous commit, ignoring any changes

```html
git reset --hard
```


### 9: git stash

git stash
**Note:** The command saves your local modifications away and reverts the working directory to match the HEAD commit.

git stash list
**Note:** This command lists a queue of stashes

git stash apply
**Note:** This command brings latest stashed changes to working directory
