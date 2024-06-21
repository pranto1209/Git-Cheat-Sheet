# Git Cheat Sheet

## Configure tooling

Configure user information for all local repositories.

```bash
# Sets the name you want attached to your commit transactions
git config --global user.name "[name]"

# Sets the email you want attached to your commit transactions
git config --global user.email "[email address]"

# Enables helpful colorization of command line output
git config --global color.ui auto
```

## Create repositories

When starting out with a new repository, you only need to do it 
once; either locally, then push to GitHub, or by cloning an 
existing repository.

```bash
# Turn an existing directory into a git repository
git init

# Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits
git clone [url]
```

## Git Stage Commit

```bash
git restore .

git add .

git reset

git reset --hard

git reset HEAD~

git commit -m "Add files via commit"
```

## Git Branch

```bash
# list your branches. a * will appear next to the currently active branch
git branch

# create a new branch at the current commit
git branch [branch-name]

git branch newbranch

git checkout newbranch

git merge main

git branch -a

git checkout -b <new-local-branch-name> origin/<remote-branch-name>
```

## Git Remote

```bash
git remote add origin https://github.com/pranto1209/GitCommand.git

git remote -v

git remote set-url origin https://github.com/pranto1209/Git.git

git push -u origin main

git push -u origin --all

git pull https://github.com/pranto1209/E-commerce-Store.git
```


## Github new repository

```bash
…or create a new repository on the command line

echo "# Competitive-Programming" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/pranto1209/Competitive-Programming.git
git push -u origin main


…or push an existing repository from the command line

git remote add origin https://github.com/pranto1209/Competitive-Programming.git
git branch -M main
git push -u origin main
```