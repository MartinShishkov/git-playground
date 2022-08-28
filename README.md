# Git Basics

New files are not initially tracked by git, so they appear as `Untracked` when executing `git status`

There are a few stages that a file can be in - Unstaged, Staged and Remote, but I might be wrong for the last one.

To stage ALL unstaged files we can execute `git add .`, if we want to stage only specific ones we just enumerate them with `git add <list of file names>`

To unstage ALL staged files execute `git reset`

Discard ALL unstaged changes `git checkout -- .`

Discard specific unstaged change `git checkout -- <filename>`

Create a new branch? - `git branch <branch-name>`

Want to make a fast commit? - `git commit -m "Your commit message"`
Commits only commit staged changes. This means we have to either execute `git add .` or whatever we want to stage.
There's a shortcut if we want to execute `git add .` followed by `git commit -m "You commit message"`. Instead, we can execute `git commit -a` which will bring up Vim or some other editor. 

## Command-line text editor
Press the `I` key to enter INSERT mode, enter your message, then press the ESC key to exit INSERT mode and type :wq to quit and save the editor.

# Logging/Info
Which branch I'm currently on? - `git branch`

Display repository as a visual graph? - `git log --graph --oneline --branches`

# Interactive rebase
## Squashing commits
We can create as many commits in our branch as we want, but when we're done with our work, it's a good idea to squash them into a single commit so that the repo does not get polluted with lots of unnecessary commits.

To do that we can use the Interactive Rebase functionality of git. 
