# Git-Github-Tutorial
A Basic Tutorial for Git &amp; Github.

This doc is written with following Nick White's YouTube Video [Git Tutorial For Dummies](https://www.youtube.com/watch?v=mJ-qvsxPHpY&ab_channel=NickWhite)

### Git & Github are two different Things.

## What is GIT ?
Wikipedia's Definition : 
> Git is a software that tracks the changes in a set of files, usually used for coordinating work among programmers collaboratively developing source code during software development. Its goals include speed, data integrity, and support for distributed, non-linear workflows.

Git is basically a memory card. 💥🤯💥
If you have a project with only a single page like this repo or with a huge number of files like HTML, CSS, JavaScript, etc, whatever programming languages you want just like how you have a video game you want to save your progress as you go that way if you die you don't lose all of your progress so with git every so often you enter a command to save your progress.

## The Process :
Step 0: Download [Git](https://www.git-scm.com)

Step 1: Initialize the repo with this command -> ```git init```  So basically you have inserted the memory card to save some files 🤔 cause obviously you can't save anything without a memory card.

Step 2: Now we can add multiple files at a time like this -> ```git add .``` or by specifying the files with a space between each file ```git add index.html styles.css``` So basically we are saving our files or progress unto the "staging area (The staging area is like a rough draft space, it's where you can git add the version of a file or multiple files that you want to save in your next commit(in other words in the next version of your project)) " (But for namesake let's assume we are selecting the files which we want to commit).

( 95% of the amount we would just add everything i.e., use this command -> ```git add .```)

Step 3: Now we actually commit the change using this command -> ```git commit -m '---Describe the changes here---'``` So we are comiting i.e., moving the changes from the staging to committing area.

Note : ```git log``` We can look at the times we saved with the message, date & time, Author and the Hash Code (which can be used to go back to that saved version).

Note : How you can go back to that saved version ? Copy the Hash Code and use the command ```git checkout copied_HashCode``` That's it!!!

Now is the tricky part when we go back to version we are forced to change our branch. check that out with this command -> ```git branch```

> A good CheatSheet for GIT [Awesome-Cheatsheets-GIT](https://github.com/LeCoupa/awesome-cheatsheets/blob/master/tools/git.sh)

## What is GITHUB ?
Wikipedia's Definition : 
> GitHub, Inc. is a provider of Internet hosting for software development and version control using Git.

Github helps people save their code in cloud and enables developers across the globe to upload their own code files and to collaborate with fellow developers on open-source projects.

## The Process : Part - II

Step 4: Now Create a new repository, copy the repository link and use the command ```git remote add origin repository_link``` So we are using this to just make it available in the website. (Links the local git(Step 1) link to the website(cloud) repository link)

Step 5: Now push those changes to the Website(cloud) repository by using this command -> ```git push -u origin master```. So we have successfully created the link and we are pushing the commits to the Website(cloud).

### Branches : 
By Default all the code is in ```master``` branch. 

Why Branches ? Some other person wants to change your code for their purpose or their needs and they don't want it to be saved so the save it onto a different branch.

Step 5: Now let's create a new branch ```git checkout -b new_branch-Name```. We created a new branch.

Step 6: Now let's see all the branches ```git branch```  and switch to the new-branch ```git checkout -b new-branch``` and edit your stuff.

Step 7: Let's push the new-branch to github(Website(cloud)) by using this command ```git push origin new-branch```.

Step 8: Now you can merge the commits from the new-branch to the master by checking the files changed, commits using github without any commands and this process is called _Pull Request_.

Step 9: In Step 8, You the master liked someone's changes and merged them into the master but those changes aren't available in your local repository so now you have to pull those changes. You can use this command to pull those changes ```git pull origin master```.

These are basic stuff. 
