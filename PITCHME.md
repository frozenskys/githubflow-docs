#HSLIDE

Hello, <span style="color:#e49436">Git</span>!

![Logo](assets/git.png)


A Git CLI 101

#HSLIDE
Contents

- Repositories 
- Adding and Committing
- Fetch\Pull\Push 
- Tags
- Branching
- Merging Branches

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

Linking a <span style="color:#e49436">local</span> and <span style="color:#e49436">remote</span> repository

```bash
git remote add origin https://github.com/frozenskys/githubflow-docs.git
git push origin master
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

#VSLIDE

Fetch changes from the remote but <span style="color:#e49436">don't</span> merge them

```bash
git fetch
```

#VSLIDE

Fetch changes from the remote and <span style="color:#e49436">merge</span> them

```bash
git pull
``` 

#VSLIDE

Push <span style="color:#e49436">committed</span> changes to the remote

```bash
git push
```

#HSLIDE

Tags

#VSLIDE

Add a new Tag

```bash
git tag myTag name
# for versions you can use the following
git tag myTag 0.4.2
```

#VSLIDE

To Push Tags

```bash
git push --tags
```

#HSLIDE

Branching

#VSLIDE

Create a new branch from the current and check it out 

```bash
git checkout -b myNewBranch
```

#VSLIDE

Push your new branch to the remote 

```bash
git push origin myNewBranch
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

Merging Branches

#VSLIDE

```bash
git checkout master
git pull origin master
git merge someOtherBranch
git push origin master
```

#HSLIDE

The End :)