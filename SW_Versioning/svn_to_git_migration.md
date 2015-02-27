# SVN to GIT migration

Easy and complete guide to migrate here:


To migrate only a subfolder of SVN use this syntax:
```
git svn clone svn+ssh://path/to/repo/ --trunk=trunk/directory --branches=branches/*/directory --tags=tags/*/directory
```