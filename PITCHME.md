#HSLIDE

Intermediate <span style="color:#e49436">git</span>

![Logo](assets/github.png)

#HSLIDE

Before we start...

There is an introduction to <span style="color:#e49436">git</span> here if you need it...

https://www.gitpitch.com/frozenskys/githubflow-docs/introduction-to-git

#HSLIDE

Merging a branch from a remote (upstream) fork.

#VSLIDE
Add the Remote you would like to sync (in this case we will call it `agc93`)

```bash
git remote -v
git remote add agc93 https://github.com/agc93/cake.git
git remote -v
```

#VSLIDE

Merge the remote branch - in this case we'll merge `agc93\develop` into our develop branch.

```bash
git fetch agc93
git checkout develop
git merge agc93/develop
```

#VSLIDE

Push the changes to the remote.

```bash
git push
```

#HSLIDE

Squashing !

#VSLIDE

Squash last 2 commits into 1 (Assuming you haven't pushed!)
```bash
git reset --soft HEAD~2
git commit -m"My Message"
```

#VSLIDE

Squash merge your branch into another.
This will take all the commits from the `develop` branch, squash them into 1 commit and then merge it with your `master` branch.
```bash
git checkout master
git merge --squash bugfix
git commit
```

#VSLIDE

A better squash merge
```bash
git checkout bugfix
git merge master
```
Resolve any conflicts, build, run tests, etc. then:
```bash
git checkout master
git merge --squash bugfix
git commit
```

#HSLIDE

Rebasing & Cleaning

#VSLIDE

Clean files that are in .gitignore

```bash
git clean -xfd
```

#VSLIDE

Reset back 2 commits and leave changes since in place
```bash
git reset --soft HEAD~2
```

Reset back 3 commits

```
git reset -- HEAD~2
```

Undo all changes since last commit
```bash
git checkout -- .
```


#VSLIDE
Rebase changes in one branch onto another

```bash
git rebase --onto target-branch source-branch
```

#HSLIDE

The End :)