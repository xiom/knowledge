# What is git?

Git is a version control system for computer files (usually codebases), it was created by Linus Torvalds in 2005 for development of the linux kernel.

## What makes git good?

His design criteria specified four things: 

* Patching should take no more than three seconds
* Concurrent Versions System (CVS) as an example of what not to do; if in doubt, make the exact opposite decision
* Support a distributed, BitKeeper-like workflow
* Include very strong safeguards against corruption, either accidental or malicious
s 
Its current maintainer, since 2005 is Junio Hamano software engineer at Google. Who Linus says has 'taste' and does a great job at maintaining and developing git.

## Why did Linus create git?

Linus Torvalds work on the Linux Kernel had shifted from writing code to being the top level maintainer of the kernel meaning
that most of his work consists of merging code from many different sources. This means merging has to be fast and painless,
also a distributed workflow was important for linux. By 2005 the linux kernel had become a big open-source project and it's
distributed organisational structure reflects that. 

https://git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows
https://en.wikipedia.org/wiki/Distributed_version_control

## What are the differences between Distributed version control versus centralized

In distributed VCS every codebase including its full history is mirrored on every developer's computer.
This extra redundancy has advantages and allows for more usecases and workflows.

Every developer who has cloned a project could potentially restore the original server including its entire history. 

Most work can be done fast and offline

You can work with multiple repositories and groups from within the same project, and many other (distributed) workflows

https://git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows
https://en.wikipedia.org/wiki/Distributed_version_control

# How to set up and configure git

## Intalling git

I'd stick with something like

```
$ sudo apt install git-all
```

## Configuring git
For me this would be:


```
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```
configuration has three levels

1. --system : system level
2. --global : user level
3. --local  : repository level

Local being the default when working from within a git repository







