# Git

## 1.

List all the remote repository
```
git remote -v
```

Add a remote repository in a project

```
git remote add origin <url>
```

### Config

Show all the you git settings

```
git config --list
```

Edit system file

```
git config --system --edit 
```

Edit user file

```
git config --global --edit 
```

Define VScode as default editor

```
git config --global core.editor code
```

Define user in file

```
[user]
  name = Matheus Dutra
  email = matheusdutra0207@gmail.com
```

Edit your project file

```
git config --local --edit 
```
All the define settings in local file will prevail over else files.

## 2.

Show the files will be add

```
git status
```

```
git status -s
```

### Alias

#### Add a alias in your global file 

1º. Open the file
```
git config --global --edit 
```
2º. Edit
```
[alias]
  s = !git status -s
  c = !git add --all && git commit -m
```

Merge the next commit with last
```
git commit --amend --no-edit
```
## 3.

## Log

list projects' commits

```
git commit log --oneline
```

Alias to show a beautiful log

```
l = !git log --pretty=format:'%C(yellow)%h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
```

# 4.

## Reset

Revert the add command
```
git reset <file name>
```

Revert a commit returning the files to stage/index
```
git reset <id of the previous commit you want to remove> --soft
```

Revert a commit returning the files to workspace
```
git reset <id of the previous commit you want to remove> --mixed
```

Revert a commit undoing all the commit's changes
```
git reset <id of the previous commit you want to remove> --hard
```

Remove files from workspace

```
git reset --hard
```

## Revert

Revert a commit with another commit that undoes the changes. 

```
git revert <commit id>
```

# 5.

## Checkout 
Revert changes that are in the workspace and have already been commited(are not untracked)

```
git checkout <file name>
```

Open the project in a specific commit(The command below open a new branch with the project in the specific commit)

```
git checkout <commit id or tag name>
```

Change to a branch 

```
git checkout <branch name>
```

Create a new branch

```
git checkout -b <branch name>
```

## Clean

Shows the file to be removed

```
git clean -n
```

Remove untracked files

```
git clean -f
```
