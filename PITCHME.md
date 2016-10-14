#HSLIDE

Hello, <span style="color:#e49436">Git</span>!

A Git CLI 101

#HSLIDE
Contents

- Create new repo 
- Clone existing repo 
- Commit (and Add) 
- Fetch\Pull\Push 
- Branch 
- Merge 

#HSLIDE

Make sure your git is configured correctly

```bash
git config --global user.name "Fred Flintstone"
git config --global user.email "fred@bedrock.com"
git config --global core.autocrlf true
```

#HSLIDE

Creating git repositories

#VSLIDE

Create an empty repository for a new project

```bash
mkdir myNewProject
cd myNewProject
git init
```

#VSLIDE 

Create a repository for an existing project

```bash
cd myExistingProject
git init
# Add all the code
git add .
git commit -m "Initial Import"
```

#VSLIDE 

Clone an exsiting remote repository

```bash
git clone https://github.com/frozenskys/githubflow-docs.git
cd githubflow-docs
```

#HSLIDE

Adding and Commiting

#VSLIDE

Commit to your local repository

```bash
git commit -m "A good commit message for this change."
```

#HSLIDE

Fetch\Pull\Push

#HSLIDE

Branching

- Branches should be short lived
- Never develop on master! 

#VSLIDE

![Logo](assets/branching.png)

#VSLIDE

Create a new branch from the current and check it out 

```
git checkout -b myNewBranch
```

#VSLIDE
Switch back to master

```
git checkout master
```

#VSLIDE
List branches

```
git branch
```

#HSLIDE

The End :)