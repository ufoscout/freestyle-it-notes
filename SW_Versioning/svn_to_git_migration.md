# SVN to GIT migration

Easy and complete guide to migrate here:
http://john.albin.net/git/convert-subversion-to-git


To migrate only a subfolder of SVN use this syntax:
```
git svn clone http://path/to/repo/ --trunk=trunk/directory --branches=branches/*/directory --tags=tags/*/directory
```