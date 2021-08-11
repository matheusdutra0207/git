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

Alias to show the beautiful log

```
l = !git log --pretty=format:'%C(yellow)%h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
```

