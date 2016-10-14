#HSLIDE

Hello, <span style="color:#e49436">Git</span>!

![Logo](assets/git-pull-request.png)


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

Create an empty repository for a <span style="color:#e49436">new</span> project

```bash
mkdir myNewProject
cd myNewProject
git init
```

#VSLIDE 

Create a repository for an <span style="color:#e49436">existing</span> project

```bash
cd myExistingProject
git init
# Add all the code
git add .
git commit -m "Initial Import"
```

#VSLIDE 

Clone an existing <span style="color:#e49436">remote</span> repository

```bash
git clone https://github.com/frozenskys/githubflow-docs.git
cd githubflow-docs
```

#HSLIDE

Adding and Committing

#VSLIDE

Commit to your local repository

```bash
git commit -m "A good commit message for this change."
```

#HSLIDE

Fetch\Pull\Push

#VSLIDE

Always <span style="color:#e49436">PULL</span> before you <span style="color:#e49436">PUSH</span>

#HSLIDE

Branching

- Branches should be short lived
- Never develop on master! 

#VSLIDE

![Logo](assets/branching.png)

#VSLIDE

Create a new branch from the current and check it out 

```bash
git checkout -b myNewBranch
```

#VSLIDE
Switch back to master

```bash
git checkout master
```

#VSLIDE
List branches

```bash
git branch
```

#HSLIDE

The End :)