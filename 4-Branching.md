## Branching

1. **Introduction to Branching**
Branching in Git allows you to diverge from the main line of development and continue to work without affecting the main branch. It's a powerful feature that supports parallel development, experimentation, and isolated bug fixes.

2. What are Branches
Theory
Branches are pointers to a specific commit in the history. The default branch in Git is usually named main or master. When you create a new branch, you're creating a new line of development.

Command
To create a new branch:

sh
Copy code
git branch <branch_name>
To switch to the newly created branch:

sh
Copy code
git checkout <branch_name>
Or, create and switch to a new branch in one command:

sh
Copy code
git checkout -b <branch_name>
3. Getting a Repository
Theory
As before, cloning a repository sets up your local environment to work with branches and other Git features.

Command
sh
Copy code
git clone <repository_url>
cd <repository_name>
4. Working with Branches
Theory
After creating and switching to a branch, you can make changes, commit them, and push the branch to a remote repository.

Commands
Create and switch to a new branch:

sh
Copy code
git checkout -b <new_branch>
Push the branch to the remote repository:

sh
Copy code
git push origin <new_branch>
5. Comparing Branches
Theory
You can compare the differences between branches to see what changes have been made.

Command
sh
Copy code
git diff <branch1> <branch2>
6. Stashing
Theory
Stashing allows you to save your working directory's changes temporarily so you can switch branches without committing unfinished work.

Command
To stash changes:

sh
Copy code
git stash
To apply stashed changes:

sh
Copy code
git stash apply
7. Merging
Theory
Merging integrates changes from different branches. There are different types of merges, including fast-forward merges and three-way merges.

Command
To merge a branch into the current branch:

sh
Copy code
git merge <branch_name>
8. Fast-forward Merges
Theory
A fast-forward merge occurs when the branch being merged has all of its commits ahead of the current branch. Git simply moves the current branch pointer forward.

Command
sh
Copy code
git merge <branch_name>
9. Three-way Merges
Theory
A three-way merge occurs when there have been divergent changes in both branches. Git creates a new merge commit to combine these changes.

Command
sh
Copy code
git merge <branch_name>
10. Viewing Merged and Unmerged Branches
Theory
You can view the status of merged and unmerged branches to track progress and pending work.

Command
To list merged branches:

sh
Copy code
git branch --merged
To list unmerged branches:

sh
Copy code
git branch --no-merged
11. Merge Conflicts
Theory
Merge conflicts occur when changes in two branches conflict and cannot be automatically merged. Resolving conflicts involves manually editing files to reconcile these differences.

Command
To resolve conflicts, edit the files and then:

sh
Copy code
git add <resolved_file>
git commit
12. Graphical Merge Tools
Theory
Graphical merge tools can simplify the process of resolving conflicts by providing a visual representation of changes.

Command
To use a graphical merge tool:

sh
Copy code
git mergetool
13. Aborting a Merge
Theory
If a merge goes wrong, you can abort it and return to the pre-merge state.

Command
sh
Copy code
git merge --abort
14. Undoing a Faulty Merge
Theory
If a merge has already been completed and committed but you want to undo it, you can revert the merge commit.

Command
To undo a merge commit:

sh
Copy code
git revert -m 1 <merge_commit_hash>
15. Squash Merging
Theory
Squash merging combines all changes from a branch into a single commit on the target branch. This keeps the history clean and concise.

Command
sh
Copy code
git merge --squash <branch_name>
16. Rebasing
Theory
Rebasing rewrites the commit history by moving or combining commits. This creates a linear history, which can make the history cleaner and easier to understand.

Command
To rebase one branch onto another:

sh
Copy code
git rebase <branch_name>
17. Cherry Picking
Theory
Cherry-picking allows you to apply a specific commit from one branch to another. This is useful for selectively porting bug fixes or features.

Command
To cherry-pick a commit:

sh
Copy code
git cherry-pick <commit_hash>
18. Picking a File from Another Branch
Theory
You can take a specific file from another branch without merging the entire branch.

Command
To checkout a file from another branch:

sh
Copy code
git checkout <branch_name> -- <file_path>
Conclusion
Understanding and utilizing branching in Git enables you to manage parallel development, isolate work, and maintain a clean project history. Branching, merging, rebasing, and other related commands are fundamental to effective version control and collaborative development.
