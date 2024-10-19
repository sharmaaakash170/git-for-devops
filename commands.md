Comprehensive Git Commands

## Configuration
- Set your name:  
  git config --global user.name "Your Name"
- Set your email:  
  git config --global user.email "you@example.com"
- View current configuration:  
  git config --list

## Repository Commands
- Initialize a new repository:  
  git init
- Clone an existing repository:  
  git clone <repository-url>

## Basic Commands
- Check the status of your repository:  
  git status
- Add files to staging:  
  git add <file>
  or add all files:  
  git add .
- Commit changes:  
  git commit -m "Your commit message"
- View commit history:  
  git log
- View a specific commit:  
  git show <commit-hash>

## Branching
- List branches:  
  git branch
- Create a new branch:  
  git branch <branch-name>
- Switch to a branch:  
  git checkout <branch-name>
- Create and switch to a new branch:  
  git checkout -b <branch-name>
- Delete a branch:  
  git branch -d <branch-name>

## Merging
- Merge a branch into the current branch:  
  git merge <branch-name>
- Abort a merge:  
  git merge --abort

## Remote Repositories
- Add a remote repository:  
  git remote add origin <repository-url>
- Push changes to a remote repository:  
  git push origin <branch-name>
- Pull changes from a remote repository:  
  git pull origin <branch-name>
- View remote repositories:  
  git remote -v
- Remove a remote:  
  git remote remove <remote-name>

## Viewing Changes
- Show changes in the working directory:  
  git diff
- Show changes staged for the next commit:  
  git diff --cached

## Undoing Changes
- Unstage a file:  
  git reset <file>
- Discard changes in a file:  
  git checkout -- <file>
- Revert a commit:  
  git revert <commit-hash>

## Stashing
- Stash changes:  
  git stash
- List stashed changes:  
  git stash list
- Apply the most recent stash:  
  git stash apply
- Drop a stash:  
  git stash drop <stash@{index}>

## Tagging
- Create a tag:  
  git tag <tag-name>
- Create an annotated tag:  
  git tag -a <tag-name> -m "Tag message"
- Push tags to the remote:  
  git push origin --tags

## Cleaning Up
- Remove untracked files:  
  git clean -f
- Remove untracked directories:  
  git clean -fd

## Advanced Commands
- Rebase a branch:  
  git rebase <branch>
- Cherry-pick a commit:  
  git cherry-pick <commit-hash>
- View the commit history graphically:  
  git log --graph --oneline --all
