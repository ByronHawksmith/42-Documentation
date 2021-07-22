# Title

`git clone <url> <repo-name>`
`git add remote github <url>`
`git status` - Check the status of the current repo (should be run frequently)
`git add .` - Stage all unstaged files
`git commit -m "<message>"` - Create a commit with a given message
`git push origin --all` - Push all changes to 42
`git push github --all` - Push all changes to github

# C Testing Workflow
`git checkout -b testing` - Checkout to a new branch called testing (code with mains goes here)
`git branch -v` - List all branches
`git checkout master` - Checkout to the master branch
`git merge testing` - Merge the testing branch into the current branch

# Other helpful stuff
`git ls-files` - Show all tracked files
`git rm --cached <file>` - Stop tracking a particular file (you will need to commit and push to persist changes)
`git rm -r --cached <folder>` - Stop tracking a particular folder (you will need to commit and push to persist changes)
