# Git basic commands
Here list out some basic Git commands to get you going with Git

### 1: Clone - Check out a repository

Create a working copy of a local repository

```html
git clone /path/to/repository
```


### 2: Add files

Add one or more files to branch

```html
git add <filename>
git add *
```

### 3: Commit - Commit changes to head
Commit the files you've added with git add.

* Commit message should be write in release note
* Better using lowercase
* Avoid symbols + - /

```html
git commit -m "Commit message"
```

### 4: Pull - Get update from server or master

Fetch and merge changes on the remote server to your working directory.

```html
git pull
```

### 5: Push - Send changes to branch

Send the changes to the master branch or Other from your local repository

```html
git push origin master/branch
```


### 6: Status - List the files you've changed

List the files you've changed and those you still need to add or commit

```html
git status
```

### 7: Branches

**Branch list** - List all the branches
```html
git branch
```

**Switch Branch** - Switch from one branch to another
```html
git checkout <branchname>
```

**Delete Branch** - Delete the feature branch
```html
git branch -d <branchname>
```

### 7: Log -  Lists the commits
Git log list the commits made in that repository in reverse chronological order

```html
$ git log
```

### 8: Changing a commit message
You can change the most recent commit message using the below command

```html
git commit --amend
```
* The commit only exists in your local repository and has not been pushed to GitHub
* Enter the new commit message and press Enter
* The new commit and message will appear on GitHub the next time you push


### 9: Reset - Revert Git repository
To revert to a previous commit, ignoring any changes
* **HEAD** code get from the git log, Use the first eight digit letter from the commit line
* **0d1d7fc3**2e5a947fbd92ee598033d85bfc445a50
* The new commit and message will appear on GitHub the next time you push

```html
git reset --hard HEAD
git reset --hard 0d1d7fc3
```


###

```html
```
