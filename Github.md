# Add SSH Key to Github
1. Sign up for a github account
2. Click on your profile in the top right
3. Click on settings
4. Click on SSH and GPG keys
5. Click on new SSH Key, give it a name, for example iMac
6. Open a terminal
7. Run `cat ~/.ssh/id_rsa.pub`
8. Copy the SSH public key into the GitHub website
9. Click Add SSH key

# Create a new repository on Github
1. Click on profile in top right
2. Click on repositories
3. Click on new repository
4. Give it the name of your current project, `C-00` for example
5. Make it public or private, completely up to you.
6. Click create repository

# Linking your Github repo to your local Git repo
1. Click the SSH button
2. Copy the link
3. Go to your terminal
4. CD into the directory for your current project, `cd C-00`
5. Run `git remote add github <url>`
6. Run `git remote -v` to see your repository
7. Run `git push github` to push all your changes to github
8. Refresh the repository website page

# How to stop tracking unwanted files
1. Run `git ls-files` to see which files you are tracking
2. Run `git rm --cached <file-path> <file-path> <file-path> ...` to stop tracking a particular file
3. Run `git status` to see your changes
4. Run `git add .` to stage your latest changes
5. Run `git commit -m "Removed unwanted files"` to commit your latest changes
6. Run `git push github master` to persist your changes on github
7. Run `git push origin master` to persist your changes on 42

# Creating a .gitignore file
1. Run `vim .gitignore`
2. Put the following in the file
```
.DS_Store
*.swp
*.out
```
3. Run `git status` to see the effect your .gitignore has taken
4. Run `git add .gitignore`
5. Run `git status to check all the files`
6. Run `git add .`
7. Run `git commit -m "Create .gitignore"`
8. Run `git push github`
9. Run `git push origin`
10. Go back to Github.com, refresh the github page to see your changes
