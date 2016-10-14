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

Create a New Repository

```bash
mkdir myNewProject
cd myNewProject
git init
```

#VSLIDE 
Use git for a legacy Project

```bash
cd myExistingProject
git init
git add .
git commit -m "Initial Import"
```

#HSLIDE 
Clone an exsiting Repository

```bash
git clone https://github.com/frozenskys/githubflow-docs.git
cd githubflow-docs
```

#HSLIDE
Commit to your local repository

```bash
git commit -m "A good commit message - that details this small change change."
```

#HSLIDE
Fetch\Pull\Push

#HSLIDE
Branching
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