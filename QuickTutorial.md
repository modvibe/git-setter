---
# Git Cheats #
---

Simple workflow
---------------

***Scenario: Create a remote repository on file server and clone it to local.***

### Create a remote bare repository (optional)

-	\*If remote repository already exists, you may skip this part.
-   On remote server (e.g. “remsvr(Z:)”), type;
#
    mkdir repo
    cd repo
    git init --bare


### Clone remote repository to local

-   Switch to your local directory, and type;

#
	mkdir myrepo
	cd myrepo
	git init
	git clone Z:/repo .

Now both remote and local repository are ready-to-git.
 

**\#TODO: Write about; add, commit, merge, push, pull**

 

### Checking history of commits

-   If you want to see the history of commits, there are several options.  
    The very first place to start is;
#
	git log

-   If you want to see it extremely simple, you may add;

#
	git log --oneline

-   If above may be too simple, you may want to do this;

#
	git log --pretty=format:"%h - %an, %cd : %s"

-   Or this;
#
	git log --pretty=format:"%h - %an, %ar : %s"

