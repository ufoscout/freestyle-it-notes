# GIT

## Init new repository
Create a new repository on the command-line (file README.md is already created)
```
$ git init
$ git add README.md
$ git commit -m "first commit"
$ git remote add origin repoUrl
$ git push -u origin master
```

## Basic Branching
Create a branch
```
$ git branch feature_branch_name
```

Switch to an existing branch
```
$ git branch feature_branch_name
$ git checkout feature_branch_name
```

Create and switch to a new branch
```
$ git checkout -b feature_branch_name
```

To push remote the locally created branch
```
$ git push -u origin feature_branch_name
```

To push all branches
```
$ git push --all origin
```
