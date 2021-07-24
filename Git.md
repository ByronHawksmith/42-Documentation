# Title
`git clone <url> <repo-name>` - Clone a repo from a url and give it a specific repo name

`git remote add github <url>` - Add a new remote called github

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

`git commit --amend <commit-id>` - Ammend a commit

`git reset --hard <commit-id>` - Move the HEAD back to the desired commit, discard all changes after that commit

`git rev-list --max-parents=0 HEAD` - Get the hash of the first commit.

`git branch test origin/<branch-name>` - Pull down a branch from a remote repository.
