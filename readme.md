# Git Cheat Sheet

First `init` a new repository to work with:

```
$git init REPO_NAME
cd REPO_NAME
```

**Note** Directories are not tracked, just add a `.keep`file

To ignore files add them to `.gitignore`:

```
log/*.log
```

To just add parts to the index we can use `git add -p` (`-p` as in "patch").

## Disaster Recovery

In case of deleted commits use `git reflog` and `git cherry-pck` to recover those commits:

```
$git cherry-pic LOST_COMIT_SHA1
```

**Note** Will be cleaned up once `git gc`run