## Git Work Flow 

Gitflow is a branching model for Git created by Vincent Driessen. 

### Parallel Development
Gitflow makes parallel development very easy by isolating new development from finished work. New development is done in **feature branches** and merbed back into the main body of colde when the developer is ready for the code to be released. 

### Collaboration
Feature branches make is easier for two or more developers to collaborate on the same feature. Each branch is a sandbox where the only bchanges are the changes necessary to get the new feature working. That makes it easy to see what each collaborator is doing. 

### Release Staging Area
As new development is completed, it gets merged back into the develop branch, which is a staging area for all completed features that haven’t yet been released. So when the next release is branched off of develop, it will automatically contain all of the new stuff that has been finished

### Support for Emergency Fixes
GitFlow supports **hotfix branches** - branches made from a tagged release. You can use these to make an emergency change, safe in the knowledge that the hotfix will only contain your emergency fix. There’s no risk that you’ll accidentally merge in new development at the same time.

## How it Works 

New development (features and non-emergency bug fixes) are built in **feature branches**: 
![image](https://user-images.githubusercontent.com/78187300/110263257-22220e80-7f84-11eb-971f-afc8baa8f119.png)

Feature branches are branched off of the develop branch, and finished features and fixes are merged back into the develop branch when they’re ready for release:
![image](https://user-images.githubusercontent.com/78187300/110263435-affdf980-7f84-11eb-8227-848def2f9b3b.png)

When it is time to make a release, a release branch is created off of develop:
![image](https://user-images.githubusercontent.com/78187300/110263566-200c7f80-7f85-11eb-8da9-37b65fb66098.png)

The code in the release branch is deployed onto a suitable test environment, tested, and any problems are fixed directly in the release branch. This deploy -> test -> fix -> redeploy -> retest cycle continues until you’re happy that the release is good enough to release to customers.
When the release is finished, the release branch is merged into master and into develop too, to make sure that any changes made in the release branch aren’t accidentally lost by new development.
![image](https://user-images.githubusercontent.com/78187300/110263671-6235c100-7f85-11eb-833e-ccfe7a3bf5c6.png)

The master branch tracks released code only. The only commits to master are merges from release branches and hotfix branches.
Hotfix branches are used to create emergency fixes:
![image](https://user-images.githubusercontent.com/78187300/110263766-a3c66c00-7f85-11eb-98c5-86bb23f8e84d.png)

They are branched directly from a tagged release in the master branch, and when finished are merged back into both master and develop to make sure that the hotfix isn’t accidentally lost when the next regular release occurs.



