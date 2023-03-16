---
title: Version control system. Git.
subtitle: This post is about how to get started with Git. First, let's learn the basics of version control systems, then move on to how to run Git on your OS and finally configure it for work. At the end of the chapter, you'll already know what Git is and why you should use it, and you'll also have a system that's finally set up to work.

# Summary for listings and search engines
summary: This post is about how to get started with Git. First, let's learn the basics of version control systems, then move on to how to run Git on your OS and finally configure it for work. At the end of the chapter, you'll already know what Git is and why you should use it, and you'll also have a system that's finally set up to work.

# Link this post with a project
projects: []

# Date published
date: '2023-03-16T00:00:00Z'

# Date updated
lastmod: '2023-03-16T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.

authors:
  - Irina

tags:
  - Git

categories:
  - study
---

```python
import libr
print('hello')
```

## About the version control system

What is a "version control system" and why is it important? A version control system is a system that writes changes to a file or set of files over time and allows you to return to a specific version later. For file version control, this book will use the source code of the software as an example, although in fact you can use version control for almost any type of file.

If you are a graphic or web designer and want to save each version of the image or layout (most likely, you will want), the version control system (hereinafter referred to as SCR) is just what you need. It allows you to return files to the state they were in before the changes, return the project to its original state, see the changes, see who last changed something and caused the problem, who set the task and when, and much more. Using SCR also means in general that if you break something or lose files, you can easily fix it. On top of that, you'll get it all without any extra effort.

## Local version control systems

Many people use copying files to a separate directory (perhaps even a time-stamped directory if they are smart enough) as a version control method. This approach is very common because of its simplicity, but it is incredibly prone to errors. You can easily forget which directory you are in and accidentally change the wrong file or copy the wrong files.

In order to solve this problem, programmers long ago developed local VCS with a simple database that stores records of all changes in files, thereby controlling audits.

One of the popular SCR was the RCS system, which is still distributed today with many computers. RCS stores sets of patches (differences between files) on disk in a special format, using which it can recreate the state of each file at a given point in time.

## Centralized version control systems

The next major problem that people face is the need to interact with other developers. In order to deal with it, centralized version control systems (CSCR) were developed. Systems such as CVS, Subversion, and Perforce use a single server containing all versions of files, and a number of clients that retrieve files from this centralized repository. The application of CSCR has been the standard for many years.

This approach has many advantages, especially over local SLE. For example, all the developers of the project to some extent know what each of them does. Administrators have full control over who can do what, and it is much easier to administer CSCR than it is to operate on-premises databases on each tenant.

Despite this, this approach also has serious drawbacks. The most obvious disadvantage is a single point of failure, represented by a centralized server. If this server goes down for an hour, then during this time no one will be able to use version control to save the changes they are working on, nor will anyone be able to share these changes with other developers. If the hard disk on which the central database is stored is damaged, and there are no timely backups, you will lose everything - the entire history of the project, except for single snapshots of the repository that were saved on the local machines of the developers. Local SLE suffers from the same problem: when the entire history of the project is stored in one place, you risk losing everything.

## Distributed version control systems

This is where distributed version control systems (RSKV) come into play. In RSCV (such as Git, Mercurial, Bazaar, or Darcs), clients don't just download a snapshot of all files (the state of files at a specific point in time) — they copy the repository entirely. In this case, if one of the servers through which the developers exchanged data dies, any client repository can be copied to another server to continue. Each copy of the repository is a complete backup of all data.

Moreover, many RSCs can interact with multiple remote repositories at the same time, so you can work with different groups of people using different approaches at the same time within the same project. This allows you to apply several approaches at once in the development, for example, hierarchical models, which is completely impossible in centralized systems.

## Resource

https://git-scm.com/book/ru/v2/Введение-О-системе-контроля-версий

