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

To list existing branches
```
# remote + local branches
$ git branch -a

# remote only
$ git branch -r
```

To cache the credentials (it should work only with https connectors):
```
git config --global credential.helper 'cache --timeout 3600'
```

Delete all local unstaged file/directory and revert modified unstaged files:
```
git clean -df
git checkout -- .
```

Delete local branches no longer on remote:
```
git remote prune origin
```

Set the local author and email for a repository:
```
git config user.email me@example.com
git config user.name "My Name" 
```
If you add the flag --global then it modifies your global config. 


## Merge

Merge a branch without fast-fastword and without autocommit
```
git merge <branchName> --no-commit --no-ff
```

Merge using the --squash option, all of the commits made on branch B will be "lumped together" and merged as a single commit.

The easy way of squashing all the commits performed in a topic branch is:
```
git reset referenceReleaseBranch
```