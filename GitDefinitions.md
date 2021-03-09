# Definitions 

## Repository 
Is a project folder, this is the place that holds all branches and commits. Every project collaborator will push and merge work in to the main repository and present it as one complete project.

## Clone
a local version of a repository, including all commits and branches

## Fork
 
Is a copy of a repository on GitHub owned by a different user. This repository is shared with new users to collaborate on. Here all parties are linked to a single project. 

## Branch
Branches are an important part of working with Git. Any commits you make will be made on the branch you’re currently “checked out”

$ git branch [branch-name]

Creates a new branch

$ git checkout [branch-name]

Switches to the specified branch and updates the working directory

$ git branch -d [branch-name]

Deletes the specified branch

## Commit - a git command that allows you to change a file or set of files; It is like a snapshot of your project.

Before the Commit 

![image](https://user-images.githubusercontent.com/78187300/109912583-5fcc2200-7c7a-11eb-9c6e-f35e27c9f812.png)

After the commit 

![image](https://user-images.githubusercontent.com/78187300/109912614-6eb2d480-7c7a-11eb-98be-0191ca3696d3.png)


## Merge - a git command that allows you to bring the forked history back together again

Before the merge

![image](https://user-images.githubusercontent.com/78187300/109909621-6bb4e580-7c74-11eb-9505-34956de62230.png)

Afer the merge 

![image](https://user-images.githubusercontent.com/78187300/109909680-82f3d300-7c74-11eb-9204-f178e68294df.png)


## Checkout

## Push - a command that allows you to upload content from your local repository to a remote repository

Before Git Push  

![image](https://user-images.githubusercontent.com/78187300/109909180-a5d1b780-7c73-11eb-8af4-0a978b46b03b.png)  

After Git Push 

![image](https://user-images.githubusercontent.com/78187300/109909271-cef24800-7c73-11eb-949c-66b5a7657d15.png)

## Pull - a command used to fetch and download content from a remote repository and immediately updates the local repository to match that content. Once the content is downloaded, it is merged. A new merge commit is formed and HEAD branch is updated pointing to the new commit. So, git pull is a fetch and rebase. 

Before Git Pull 

![image](https://user-images.githubusercontent.com/78187300/109907782-03183980-7c71-11eb-984e-0bb89f62ca05.png)

After Git Pull 

![image](https://user-images.githubusercontent.com/78187300/109907963-6b671b00-7c71-11eb-83df-c01b2a90ef20.png)

## Remote Add/ Remove/ Show

The "remote" repository that is the source of a fetch or pull operation. This parameter can be either a URL or the name of a remote (see the section REMOTES).

“Git Add”: This command updates the index using the current content found in the working tree, to prepare the content staged for the next commit. It typically adds the current content of existing paths as a whole, but with some options it can also be used to add content with only part of the changes made to the working tree files applied or remove paths that do not exist in the working tree anymore.

“Git Remove”: A user can remove a branch by simply typing in ‘git push origin  :<location>’ 
“Git Show”: Is the default for ‘git log’…git-show is a command line utility that is used to view expanded details on Git objects such as blobs, trees, tags, and commits. git-show has specific behavior per object type. Tags show the tag message and other objects included in the tag. Trees show the names and content of objects in a tree.

## Git Status
git status command displays the state of the working directory and the staging area. It lets you see which changes have been staged, which haven't, and which files aren't being tracked by Git.

While working on the project, after every ‘git add –all’ commit I checkout the status of my branch, if I committed the message using the wrong name it returns a message ‘untracked files ~$ster Branch.docx’ I realize the misspelling deviated the commit.


## Master Branch

In Git, "master" is a naming convention for a branch. The link for our repository for this group assignment is found https://github.com/EmadAbdelhamidNJIT/IS601Ass1.git 

After cloning the Master (downloading) a project from a remote server, the resulting local repository has a single local branch: the so-called "master" branch. This means that "master" can be seen as a repository's "default" branch.

![gitpicture](https://user-images.githubusercontent.com/77909953/110259352-34e11700-7f75-11eb-920f-966c0c74e09c.png)
