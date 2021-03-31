# Open Coding Hour GitHub Workshop

Welcome to the Open Coding Hour GitHub workshop! This document is a guide to supplement our hands on workshop during Open Coding Hour on 3/31/2021
Rachael Cox and Alex Lukasiewicz will walk you through the basics of using GitHub. We will start by covering some common terms used in the git world and then walking through the process of intializing your own repository to begin tracking a solo project.
We will also cover how to work on collaborative projects and demonstrate what happens when things go wrong.

## Why use git? :octocat:

There are tons of reasons why someone would use git, from [hosting a website](https://github.com/wilkelab/wilkelab.github.io) to [publishing a package](https://github.com/rachaelcox/diffprot) to [ensuring reproducibility](https://github.com/marcottelab/CoEVxIMP) of published results  

One of the main advantages to using git while developing your code is for **version control**.

GitHub offers a robust Version Control System (VCS) called git that tracks and maintains a history of changes to files, allowing you to tweak, break, improve, break again, and recover scripts without having to keep track of "myscript_v3.py" one day and "myscript_v4" the next

### More reasons to use git (for bioinformaticians) 
 
 <img src=data/perez-riverol_fig_1.png width="700" height="500">

Collaborating on a project is made easier with the GitHub forking and branching system (which we will demonstrate later in the workshop) 

![Jim Vallandingam figure](https://vallandingham.me/images/git/git_diagrams.png)

### When to use git? 

## Important Vocabulary and Concepts 
Most defitions from [1](https://doi-org.ezproxy.lib.utexas.edu/10.1371/journal.pcbi.1004668)

**Branch**: A copy of the files in your main repository. Useful for developing new features while keeping your old code intact. Useful for all the reasons you would want a stable version preserved: fixing bugs, writing new functions, sandboxing, and collaborative changes.

**Clone**: Create a local copy of a repository on your personal computer. Does not maintain a connection to the repo you have cloned from.

**Commit**: Once changes have been implemented, commits are a snapshot of those changes made. Usually associated with some unique message that you can use to track your changes over time.

**Fork**: Copy of another GitHub repository to your own while maintaining a connection to the original repo. Changes made to the main repo can be **pulled** as they are updated. **Forking** allows for collaboration on projects as you can also push changes to be **merged** if allowed by the owner of the repo.

**Merge**: Update files by incorporating changes from your own **branches** or from **forked branches**

**Pull**: To retrieve changes from a remote repository to your local repository 

**Push**: To send changes from your local repository to your remote repository 

**Repository**: Directory containing all of your tracked files with associated version history. Also referred to as a repo.


## Setting up your first GitHub repo on a solo project

If you have already been working on a project locally, do not fear! You can initialize your a repository in your local directory and start making commits.

There are two approaches to initializing a repo on GitHub:
1. From scratch on your GitHub webpage
2. From an already existing local directory 

### Initialize repo from scratch using the GitHub webpage 

* Navigate to your personal GitHub page and click on the Repositories tab  

### Initialize repo from your local files 

Navigate to the directory that you wish to add to a remote github repository 

Initialize the git VSC with 

```bash
git init
```
Then stage all the files you would like to be tracked with

```bash
git add [your file] 
```
or to stage all files 

```bash
git add .
```

Add a commit message with 

```bash
git commit -m "initial commit"
```

Then create a new repository as we did above

After this there are two ways to connect to your remote repository:

**Method 1**

Connect staged local files to online repo
```bash 
git remote add origin git@github.com:username/your_repo
```
Push files to master branch online
```bash 
git push -u origin master
```

**Method 2**

```bash 
git remote add origin https://github.com/username/new_repo
```

*Note: username and password logins are being depreciated by GitHub in August 2021, but logging in with an SSH key is not. [See the GitHub guide to setting up your ssh key](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh)

### What is a readme?
We are currently looking at an example of a README file. This is a text file that helps orient a new collaborator or member of the GitHub community to your project. There are some conventions that help others understand what is going on in your repo.   

  
## Forking, Branches, and Merging with Rachael
  
### In class example: 

Try forking this repository yourself 
  
## Additional resources to help on your GitHub journey 

**Academic Papers**

* (1) [A Quick Introduction to Version Control with Git and GitHub](https://doi-org.ezproxy.lib.utexas.edu/10.1371/journal.pcbi.1004668)

* (2) [Ten Simple Rules for Taking Advantage of Git and GitHub](https://doi-org.ezproxy.lib.utexas.edu/10.1371/journal.pcbi.1004947)

**Quick Start Guides (good for bookmarking)**

* 

* For when things go wrong [Oh Shit, Git](https://ohshitgit.com/)

* Markdown guide for :poodle: [git suppored emojis!](https://www.webfx.com/tools/emoji-cheat-sheet/) :poodle:

**For more hands-on practice**

* [GitHub learning labs](https://lab.github.com/)
* Learning more about git branching in a [playable game](https://learngitbranching.js.org/)
* 

