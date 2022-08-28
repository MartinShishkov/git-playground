> New files are not initially tracked by git, so they appear as `Untracked` when executing `git status`

> There are a few stages that a file can be in - Unstaged, Staged and Remote, but I might be wrong for the last one.

> To stage ALL unstaged files we can execute `git add .`, if we want to stage only specific ones we just enumerate them with `git add <list of file names>`

> Which branch I'm currently on? - `git branch`

> Want to make a fast commit? - `git commit -m "Your commit message"`

# Interactive rebase

## Squashing commits
We can create as many commits in our branch as we want, but when we're done with our work, it's a good idea to squash them into a single commit so that the repo does not get polluted with lots of unnecessary commits.

To do that we can use the Interactive Rebase functionality of git. 
