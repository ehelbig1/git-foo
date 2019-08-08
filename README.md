# Git-Foo

Everything you need to know about git, or at least where to find it!

## Git Help

Like any great software, Git has excellent documentation!

There are many ways to learn more about Git and specific tools:

1. From the command-line
	* $ git help \<verb\>
	* $ git \<verb\> --help
	* $ git \<verb\> -h (will output a list of command options)  
	* $ man git-\<ver\>

2. Websites
	* [man-pages](https://git-scm.com)
	* [Git How To](http://githowto.com) (A fun interactive tutorial)

## Git vs Other VCS

## Git Architecture

It's important to understand the basic underlying architecture Git uses. Most Git tools make use of this architecture
and understanding it will allow you to better understand these tools. 

There are three main areas that files move through during the Git flow.

![Git Architecture](./images/architecture.png)

### The Working Directory

This is the project directory on you file system. Nothing super interesting here!

The file can be in two states _tracked_ (meaning Git is versioning that file) and _untracked_ (meaning Git is not versioning the file).

### The Index (Staging Area)

File can be added to the _Index_ using `git add`. This is an area, a file in fact `.git/index`, that sits in between your working directory and repository.
Any files that are in this staging area will be stored in the repository upon running `git commit`. The _Index_ can be used to break changes to several files
into multiple commits if needed.

### The Repository


