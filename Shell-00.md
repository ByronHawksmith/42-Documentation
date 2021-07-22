# Tips
- Use `ls` to list all the files and sub-directories in the current directory
- Use `pwd` to see where you currently are in the file system

# VIM Tips
- To open a file with vim use `vim <file-name>`
- To insert characters into a file that has been opened with vim, you have to change into **insert mode** by pressing the `I` key
- To escape out of insert mode, you have to press the `ESC` key
- **MAKE SURE YOU HAVE PRESSED `ESC` BEFORE TRYING TO EXIT VIM**
- To exit out of a file and save your changes, type `:wq`
- To exit out of a file without saving your changes, type `:q!`

# GIT Tips
- Use `git clone <url> <repo-name>` to clone a remote repository
- Use `git status` to check the status of the current repository
- Use `git add .` to stage all currently unstaged files
- Use `git commit -m "<insert-message-here>"` to commit all currently stages files
- Use `git log` to see a history of all previous commits
- Use `git push` to push the changes on your local repository to the remote repository

# Introduction
1. Open a terminal and navigate to your home directory using `cd ~`
2. Navigate to the https://projects.intra.42.fr/ in your browser
3. Click "C Piscine Shell 00"
4. Click "Register"
5. Copy the git url which will look something like `git@vogsphere.42adel.org.au:vogsphere/...`
6. Clone the git repository using `git clone <url> Shell-00`
7. Change into the new Shell-00 directory using `cd Shell-00`

# Exercise 00
1. Navigate to your home directory using `cd ~`
2. Make a new directory called ex00 `mkdir ex00`
3. Change into the ex00 directory `cd ex00`
4. Create a new file called z `touch z`
5. Modify the file using vim by typing `vim z`
6. Read the VIM Tips section
7. Add a Z character to the file then save it
8. Test that you get the correct output by typing `cat z`

# Exercise 01
1. Navigate to your home directory using `cd ~`
2. Make a new directory called ex01 `mkdir ex01`
3. Change into the ex00 directory `cd ex01`
4. Create a new file called testShell00 `touch testShell00`
5. Observe changes `ls -l`
6. Redirect 40 random bytes into the file `head -c 40 /dev/urandom > testShell00`
7. Observe changes `ls -l`
8. Change the timestamp of the file `touch -t 202106012342 testShell00`
9. Observe changes `ls -l`
10. Change the permissions of the file for the user `chmod u-w testShell00`
11. Observe changes `ls -l`
12. Change the permissions of the file for the group and other  `chmod go+x testShell00`
13. Observe changes `ls -l`
14. Compress testShell00 into a tar file `tar -cf testShell00.tar testShell00`

## Raw Steps
```
touch testShell00;
head -c 40 /dev/urandom > testShell00;
touch -t 202106012342 testShell00;
chmod u-w testShell00;
chmod go+x testShell00;
tar -cf testShell00.tar testShell00;
```