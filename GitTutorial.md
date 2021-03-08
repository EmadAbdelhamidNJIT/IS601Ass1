# Git Tutorial
**Follow the following steps to get started with Git**

Create a step by step tutorial that explains how to set up Git and work collaboratively with more than one person.  You must explain the concept of branching and how to to use branches to avoid merge conflicts, your tutorial must illustrate how to create a merge conflict and resolve the merge conflict.   

1. Forking vs Cloning

2. Pull Request

3.  Adding a collaborator to a Github Repo.

## Setting Up Git 

1. In the upper-right corner of any page, use the  drop-down menu, and select New repository.

2. Type a short, memorable name for your repository. For example, "IS-601".

3. Optionally, add a description of your repository. For example, "mini-project1."

4. Choose a repository visibility. Options: *public, internal, or private*. When you chose to make your repository _public_ anyone can access it on the internet. _Private_ repositories are only accessible to you, people you explicitly share access with. _Internal_ repositories are accessible to enterprise members.

5. Select Initialize this repository with a README. README files often contain instructions and additional help, and details about patches or updates.

6. Click Create repository.

## How to work with more than one Person 

There are 2 ways to work with other users, the 1st is to share the repository link with another person. The 2nd is to _Fork_ the repository. 

## Forking Vs Cloning

If a repository is **forked** the recipient of the repository will obtain someone else's work as a starting point. From there each new user can create other files to support that forked project. Forking a repository allows the user to freely experiment with changes without affecting the original project. Forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea. The manager of a forked repository has full access to approve additional or supportive work done by another user. 

#### Cloning

Cloning a repository pulls down a full copy of all the repository data that GitHub has at that point in time, including all versions of every file and folder for the project. You can push your changes to the remote repository on GitHub, or pull other people's changes from GitHub

When you create a repository on GitHub, it exists as a remote repository. You can clone your repository to create a local copy on your computer and sync between the two locations.

## What is Branching & How to use branching to Avoid Merge Conflicts

Branching becomes thedifferent files to a project. A branch is analgously to a chapter in a book, where each chapter tells a part of a story. By default your repository has one branch named *main* which is considered to be the definitive branch. We use branches to experiment and make edits before committing them to *main*. When a branch is created off the main branch, a copy is being made, or snapshot, of *main* as it was at that point in time. If someone else made changes to the main branch while you were working on your branch, you could pull in those updates.

## How to Create & Resolve a Merge Conflict 

You can only resolve merge conflicts on GitHub that are caused by competing line changes, such as when people make different changes to the same line of the same file on different branches in your Git repository (see screenshot below). For all other types of merge conflicts, you must resolve the conflict locally on the command line. On GitHub, once you fix the conflict click on *Resolve* and proceed with merge. 

![git_merge conflict](https://user-images.githubusercontent.com/77909953/110269079-ed688400-7f90-11eb-8faf-175ad45eefda.jpg)

## Pull Request

Open **Pull** request> create a **New Pull Request** > specify the *To* and *From* repository (the base branch is where changes should be applied, the head branch contains what you would like to be applied)> finally click on *Create Pull Request*

## Adding a Collaborator

In GitHub, add a collaborator by going to the intended repository> click on settings> Manage access> Invite Collaborator> start typing the name of person you want to invite, then click a name in the list of matches> Add name to repositoryThe user will receive an email inviting them to the repository. Once they accept your invitation, they will have collaborator access to your repository.
