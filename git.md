# "Gitting" to know Git

## Version Control

Git is version control software. What this means is that each time you "committ" a file, you are saving a snapshot of that file at the time of committ.

Committs are saved so you can go back and recall older versions of the file in question at various points in history.

A **repository** is a file system/project in Git. 

## Installing Git

For information on installing Git, visit [here](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)

From the terminal, you can check Git status by using the command **git congig --list**

From the terminal, you can see help files by using the command **git help *command***

## Cloning

Cloning a repository is copying it to your local drive. You can do this by hitting the "git clone" button in GitHub, navigating to the correct location via terminal, and then using the command 

>git clone address

where "address" is the web address you copied by hitting the Git Clone button.

After cloning, you do work on your file locally, in say VSCode. You must do this so that the version of the file in Git is not "ahead" of your file locally. This will cause a ***merge conflict***.

The *head* of your project is the file that is most recent. After you make changes to your file locally, you then need to update in Git through a terminal process called ACP.

## ACP

*ACP* is an important acronym that stands for add, commit, push. We explain below:

### Add

- Use the command **git add filename** to add file to be tracked.

- You can use **git status** to see that that file has changes that need to be committed.

### Commit

- Use the command **git commit -m "*note*"** to commit file changes, leaving yourself a note of what was changed.

### Push

- The command **git push origin master** pushes your local cloned repository to the remote repository (remote means not local - so the one on GitHub).

  - In this command, *orgigin* refers to the remote repo, and *master* refers to the local repo. These are default monikers that can be renamed.
  
## Testing

This is to test if I can perform an ACP.