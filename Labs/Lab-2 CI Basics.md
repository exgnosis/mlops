# Lab 2 - Working with CI

## Objectives
This lab is a hands-on review of working with continuous integration with source code.

## Part 1 - Git basics
This lab will go through some of the basic operations using git to create, version and maintain a git repository.

This lab can be done in either CloudShell or Cloud9

### Step 1-1 - Configure git
Before you can commit any changes to any repository, git has to know who you are so that it can track who made the changes.

This is done with the commands:

```console
git config --global user.email "youremail@yourdomain.com"
git config --global user.name "My Name"
```
These don't have to be your real name and email, they just need to establish some kind of identity

### Step 1-2 - Working with git
Create a directory and cd into it.  Then run the commands below:

```Console
$ mkdir testgit
$ cd testgit
testgit$ git init
Initialized empty Git repository in /home/cloudshell-user/testgit/.git/
```
Git uses a two stage commit which is explained in the git documentation. This will be demonstrated by the instructor.  A file called test.txt is created, added to the staging area and then commited.  The log command shows the commit being recorded

```Console
$ git status  # should show untacked files
$ git add test.txt
$ git commit -m "Initial commit"
$ git log
```
Edit the file then go through the same process again.  You should now see both commits in the "git log " printout.

### Step 1-3 - Working with branches
Branches represent different lines of work. It is beyond the scope of this lab to go into the details of branching and merging beyond the basics. The instructor will go through the basic of created and merging a simple branch.

The commands below are the ones used in the demo for your reference, but are not intended to followed as step by step how to instructions
```Console
$ git branch -l   # list branches
$ git checkout -b dev  # create a new branch dev and start using it'
$ git checkout master  # checkout them master branch
$ git merge dev  # merge the changes from the dev branch to the master branch
```

### Step 1-4 - Working with tags
Tags are used to identify a specific commit as having some special significance, like being in a specific release.
We will just do a very simple tag to illustrate how they work.

The commands used in the demo are"

```Console
$ git tag -l    # list the tags
$ git tag rel1  # tags the commit to be made with the tag rel1
$ git show rel1 # shows the commit tagged with rel1
```
Note that if we try and tag a second commit with rel1, git won't get us.

### Step 1-5 - Working with Code Commit
Note code commit works very similar to GitHub and GitLab.

---


## Part 2 - Virtual Environments

We often want to work in a customized environment in Python.  In this section, you will create and activate a python virtual environment

The commands used are

```Console

$ python3 -m venv ~/.myenv   # creates the environment
$ source ~/.myenv/bin/activate  # activates
$ deactivate   # deactivates the environment.
```
---





