![Workflow](https://github.com/user-attachments/assets/3baa6d5f-4c4b-4a16-9463-917e56bfa6dc)

## Working Directory:
This is where your project files are located on your local machine.
You make changes to your files here.

## Staging Area:
This area holds the changes you intend to include in your next commit.
It is like a buffer between the working directory and the local repository.

## Local Repository:
This is the repository on your local machine where committed changes are stored.
It contains the history of all your commits.

## Remote Repository:
This is a repository hosted on a remote server (like GitHub, GitLab, or Bitbucket).
It is used for sharing changes with others and for backup.

## Commands:
    git add
Moves changes from the working directory to the staging area.
Command: git add <file> or git add . (to add all changes).

    git commit
Moves changes from the staging area to the local repository.
A commit represents a snapshot of your project at a certain point in time.
Command: git commit -m "commit message"
    
    git push
Uploads commits from the local repository to the remote repository.
This is how you share your changes with others or back them up.
Command: git push <remote> <branch>
    
    git pull
Fetches and merges changes from the remote repository to the local repository.
This is used to update your local project with changes made by others.
Command: git pull <remote> <branch>
    
    git checkout
Switches between different branches or commits.
Also used to revert changes in the working directory.
Command: git checkout <branch> or git checkout <commit>

## Workflow:
You start by making changes to your files in the working directory.
Use git add to move changes to the staging area when you're ready to commit them.
Use git commit to save the changes in your local repository.
Use git push to send your commits to the remote repository.
Use git pull to get the latest changes from the remote repository.
Use git checkout to switch branches or revert changes.
