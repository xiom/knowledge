# What is git?

Git is a version control system for computer files, it was created by Linus Torvalds in 2005 for development of the linux kernel.

# What makes git good?

His (Linus) design criteria specified four things: 

* Patching should take no more than three seconds
* Concurrent Versions System (CVS) as an example of what not to do; if in doubt, make the exact opposite decision
* Support a distributed, BitKeeper-like workflow
* Include very strong safeguards against corruption, either accidental or malicious

Its current maintainer, since 2005 is Junio Hamano software engineer at Google. Who Linus says has 'taste' and does a great job at maintaining and developing git.

# Why did Linus create git?

Linus Torvalds work on the Linux Kernel had shifted from writing code to being the top level maintainer of the kernel meaning
that most of his work consists of merging code from many different sources. This means merging has to be fast and painless,
also a distributed workflow was important for linux. By 2005 the linux kernel had become a big open-source project and it's
distributed organisational structure reflects that. 

https://git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows
```
## Distributed Workflows
Unlike Centralized Version Control Systems (CVCSs), the distributed nature of Git allows you to be far more flexible in how developers collaborate on projects. In centralized systems, every developer is a node working more or less equally on a central hub. In Git, however, every developer is potentially both a node and a hub — that is, every developer can both contribute code to other repositories and maintain a public repository on which others can base their work and which they can contribute to. This opens a vast range of workflow possibilities for your project and/or your team, so we’ll cover a few common paradigms that take advantage of this flexibility. We’ll go over the strengths and possible weaknesses of each design; you can choose a single one to use, or you can mix and match features from each.
```



