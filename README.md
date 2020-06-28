# A Simple, Hassle Free Guide to Starting and Using Git

This document is setup as a simple guide to provide you with a general overview together with all the essential commands needed to successfully start using 'git' to create and manage your projects.  For those  interested, the core git system was designed by Linus Torvalds who also developed the Linux kernel.

Essentially, 'git' is a non-linear, decentralised file version and tracking control system that in addition to being platform non-specific (i.e. not limited to specific programming languages) is able to 'role' back tracked files to previous versions (providing you have committed snapshots of the code),  it also supports collaboration between multiple authors across multiple networks to edit, manage and work on the same and/or different computer based files. If you want to share your local repository with a wider team or members of the public you can 'push' your work to a remote repository/storehouse such as gitHub or bitBucket, etc.

**The basic process is:**

- Create a 'Local Repository' (i.e. a folder on your local machine ) to hold your project.
- Initialise the local repository to use git.
- Edit/update and/or work with your files.
- Add files to your local repository's  'staging area' - this is the area that can be pushed to a remote repository; files stored locally but not added to your staging area will not be tracked.
- Commit (i.e. take a snapshot) of the changes to the files in the staging area.
- Push the snapshot to your remote repository for storage, collaboration or further deployment.



## Git - The Basic Commands

The following instructions illustrated using a Mac assumes that git  is already installed and should be executed via a 'Windows' command or 'Mac/Linux' terminal window.  

**1. Checking git is installed**

You can easily check the state and version of your git version by using the command:

`$ git --version`

*Once executed, the system should reply with (if installed) the current version of git; this will likely (based on your operating system) look something similar to:*

`git version 2.24.3 (Apple Git-128)` 

**2. Create a local repository (a.k.a. working directory) for your project**

`$ mkdir ./app-project-folder`

`$ cd ./app-project-folder`

`$ git init` 

*Once you have 'moved  to' (cd ./dir), or  created (mkdir ./dir) the local folder you want to use with your project executing the 'init' command will initialise the folder as a  local 'git' repository; essentially this process creates a hidden 'dot' folder in the current directory.  Once created, this folder does not (normally) need to be manually explored. To view/hide hidden files/folders (in a Finder window on a Mac) use, 'command-shift-dot' .  Once the repository has been initialised you can begin using other git commands.*  

Once executed, the system will likely reply with something similar to:

```
Initialized empty Git repository in /Users/purplehominid/app-project-folder/.git/
```

**3. Create a new, empty file in the local folder; this step can be skipped**

If you don't have a file available you can create one via the command or terminal window; Mac or Linux users can create an empty file using the following command:

`$ touch ./filename`

*Once executed, the system should simply return a new command prompt, to check if the file exists you can execute a command that lists all the files in the current folder:*

`$ ls -l`

*Once executed, if you're using a Mac or Linux system you'll be provided with a list of all the files and folders in the current directory - this may look something similar to:*

```
-rw-r--r--	1	Username	Group	0	20 Jun 08:45	filename
```

**4. Adding files to your project's git index (a.k.a. staging area)**

To enable tracking on specific files 'add' them to git staging area.  Files in the project's local repository are 'untracked' (not included in the git process) unless/until they're added to the staging area  - to add files to the staging are use the command:

`$ git add ./filename` 

*Once executed, if there are no errors the system replies with a new command prompt.  All files in local repository can be added simultaneously using the '.' character as a 'match all' wildcard:*

`$ git add .` 

**5. Checking the project's git index (a.k.a. staging area)**

To check the current state of git as well as the untracked and tracked files  use the command:

`$ git status`

*Once executed, the system will respond with details on your branch (discussed later), commit details as well as any staged and untracked files.*

```
On branch master
Changes to be committed:
	filename

Untracked files:
	filenameX
	filenameY
```

**6. Create a snapshot of the current system (staging area)**

To commit (take a snapshot) of the current system use the command:

`$ git commit`

*Once executed, the system may ask you to provide a 'commit' message describing the revisions or modifications.*

**7. Publish your snapshot to your remote repository  (staging area)** 

When ready you can share (publish) your current snapshot using the command:

`$ git push`

*Once executed, the system may ask you to provide a 'commit' message describing your revisions and/or modifications - this is useful when reviewing and working with others.*

**8. Restore or pull a previously shared snapshot back to your local repository**

Before you can start working locally with a previously shared snapshot you need to pull the files from your remote repository using the command:

`$ git pull`

*Once executed, the system will ....*





git pull <remote master> <local repo master> --allow-unrelated-histories

git config --global user.email "6672701+PurpleHominid@users.noreply.github.com"

git push master master

git config --global user.email 
