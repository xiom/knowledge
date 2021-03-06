# What is Git?

Git is a version control system for computer files (usually codebases), it was created by Linus Torvalds in 2005 for development of the linux kernel.


## What makes Git good?

His design criteria specified four things: 

* Patching should take no more than three seconds
* Concurrent Versions System (CVS) as an example of what not to do; if in doubt, make the exact opposite decision
* Support a distributed, BitKeeper-like workflow
* Include very strong safeguards against corruption, either accidental or malicious
s 
Its current maintainer, since 2005 is Junio Hamano software engineer at Google. Who Linus says has 'taste' and does a great job at maintaining and developing Git.


## Why did Linus create Git?

Linus Torvalds work on the Linux Kernel had shifted from writing code to being the top level maintainer of the kernel meaning
that most of his work consists of merging code from many different sources. This means merging has to be fast and painless,
also a distributed workflow was important for linux. By 2005 the linux kernel had become a big open-source project and it's
distributed organisational structure reflects that. 


## What are the differences between Distributed version control versus centralized

In distributed VCS every codebase including its full history is mirrored on every developer's computer.
This extra redundancy has advantages and allows for more usecases and workflows.

Every developer who has cloned a project could potentially restore the original server including its entire history. 

Most work can be done fast and offline

You can work with multiple repositories and groups from within the same project, and many other (distributed) workflows

https://git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows

https://en.wikipedia.org/wiki/Distributed_version_controlsudo


# How does Git work?

* snapshots vs diff
* integrity (checksums)
* cumulative 
* local
* three data states, modified, commited staged

# How to set up and configure Git?

## Intalling Git

I'd stick with something like

```
$ sudo apt install git-all
```

## Configuring Git
For me this would be:


```
$ git config --global user.name "J.M. Filius"
$ git config --global user.email joscha@xiom.nl
```
Configuration has three levels lower levels override the higher, from top to bottom they are:

1. System `--system`
2. User `--global`
3. Local `--local`

Local being the default when working from within a Git repository.

## Help and additional support

* Manual `git help <verb>`, concise `git <verb> -h`
* https://git-scm.com/book
* irc.freenode.net #git #github

# Working with Git repositories

## Creating a repository

1. 'init' git repository in the directory
2. 'add' files in the codebase to track to the index
3. 'add' the licence to the index
4. 'commit' files in index to repository including a commit message

```
$ git init
$ git add *.py
$ git add LICENCE
$ git commit -m 'init of project'
```
Or clone a repository

$ git clone https://github.com/xiom/some_repository

Files in the working directory can be either 
* tracked
  * unmodified
  * moddified
  * staged
* or untracked

```
Untracked          Unmodified          Modified          Staged
  |                     |                  |                |
  + Add the file ------------------------------------------->
  |                     + Edit the file --->                |
  |                     |                  + Stage the file >
  <-----Remove the file +                  |                |
  |                     <---------------------------- Commit+
```

## Checking the status of your files

`$ git status

1. Modification of tracked files
2. Branch and branch vs origin
3. List untracked files in working directory






