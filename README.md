# A Simple, Hassle Free Guide to Starting and Using Git

This document is setup as a simple guide to provide you with a general overview together with all the essential commands needed to successfully start using 'git' to create and manage your projects.  For those  interested, the core git system was designed by Linus Torvalds who also developed the Linux kernel.

Essentially, 'git' is a decentralised file version control system that in addition to being able to 'role' back to previous versions of a file also supports collaboration between multiple authors to edit and manage computer based files. 



## Git - The Basic Commands

The following instructions *(illustrated using a Mac terminal window)* should be executed via a 'Windows' command or 'Mac/Linux' terminal window.  



**1 Create a local repository for your project**

`$ mkdir ./app-project-folder`

`$ cd ./app-project-folder`

`$ git init` 

*Once you have 'moved  to' (cd ./dir), or  created (mkdir ./dir) the local folder you want to use with a specific project executing this command will initialise a local 'git' repository (essentially creating a hidden 'dot' folder in the current directory; once created, this folder does not (normally) need to be manually explored.  Once the repository has been initialised you can begin using other git commands.*

