### *Creating and pushing your first project.*### 


## STEP 1 - Install Git
Download *Git* from official website and install.
 - Then verify the installation:
   `git --version`
   If version appears -> Git is instlled successfully.
   ( Git is installed locally on your system and will track all of your project changes.)
## STEP 2 - Configure Git ( for the first time setup)
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```
## STEP 3 - Create a project folder.
Example: `git-first-repo`
Inside that create your files like - index.html , main.py
Write code in your files.

### STEP 4 - Now initialize git repositry.
Inside your vs code open the folder and in the terminal run: 
`git init`
~ This converts a normal folder into a Git repository.
Git now starts tracking changes.
  
### STEP 5 - You can check status now. 
`git status`
It helps you in showing. modified files, untracked files, staged files

### STEP 6 - Stage Files
`git add .`
This moves files into the staging area.
(Think of staging as selecting changes to save.)

### STEP 7 - Commit Changes
`git commit -m "Initial project commit"`
A commit is like a save point in your project history. it helps when you later have to find the versions of your code.

### Step 8 — Create Repository on GitHub
Now to to github website. On your profile create a new repository. 

Click:
New Repository

Fill:
Repository name
Description
Public
Then click Create Repository.

### STEP 9 - Connect Local Repo to GitHub
Copy repo link.
Run - `git remote add origin <repo-url>`
This connects your local repository to remote repository.

### STEP 10 - Push Code to GitHub. 
`git push -u origin main`
Push means uploading your code to GitHub.
Refresh GitHub page → code appears.

#### STEP 11 - for further commits.
After modifying the files.
Run: 
```bash
git add .
git status
git commit -m "Added workshop text"
git push
```
( In add . - you can wrtie the specific file name also which you want to commit chnages. )
~ Every change creates a new commit version.

### Step 12 - Show Commit History
On your GitHub Repo: 
Click Commits.
You can see - who changed code, when, what changed
Also to show: 
git log


### Step 13 - Show Code Difference
Run: `git diff`
This shows exact code modifications.

### Collaboration Workflow ###

## Step 1 - Clone Repository
`git clone <repo-url>`
Clone = download entire repository with history.

## Step 2 - Pull Latest Changes
`git pull`
Pull = get latest updates from GitHub.

## Step 3 - Branching
```bash
git branch new-feature
git checkout new-feature
```
## Step 4 - Merge Branch
`git checkout main`
`git merge new-feature`
This combines feature code into main project.

## Step 5 — Fork Repository (Open Source Concept)

Fork = copy someone else's repository to your account.

Steps:
1. Click Fork
2. Repository copied to your profile
3. Clone forked repo
4. Make changes
5. Push changes

##  Step 6 — Pull Request (Important)
After making changes:
Click Pull Request
Maintainer reviews code and merges it.
