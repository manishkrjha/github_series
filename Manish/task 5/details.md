> This file breifs you about getting started with git and github.


### Getting Started

**What is Git?**
Git is a free and open source distributed *version control* system designed to handle everything from small to very large projects with speed and efficiency.

**What is Github?**
GitHub is a website and cloud-based service that helps developers store and manage their code, as well as track and control changes to their code. Along with Git it can be used to manage your projects.

---

### Installing and configurartion

> Installation

For windows refer <a href="https://www.youtube.com/watch?v=cEGIFZDyszA&list=PL6gx4Cwl9DGAKWClAD_iKpNC0bGHxGhcx&index=1">this</a>.
For Mac refer <a href="https://www.youtube.com/watch?v=ZMgLZUYd8Cw">this</a>.
For Linux refer <a href="https://www.youtube.com/watch?v=LK0vMt_lEbQ&t=20s">this</a>.

You can check if git is properly installed or not by running the following in terminal:

```git --version```

> if the above line doesn't gives error *git* has been installed in your system successfully.

> Configuration

Type following commands in your terminal to configure your username and email

```
    git --config global user.name "Your name"
    git --config global user.email "your@email"
```

### Git Repository
A repository is like a folder for your project. Your project's repository contains all of your project's files and stores each file's revision history. You can also discuss and manage your project's work within the repository.

> How to make repo?

- open git bash
- create a folder
    - type ```git init``` in terminal.
    - This can be done by ```mkdir folder_name`` in git bash.
- create and store files/folders within it.

*Voila! Your repository has been created.*

> Commiting changes in the project

- Open the repo
- open file and make changes.
- open terminal.

    - write ```git status```. This will give the current status of files/changes in the project.
    - ```git add file_name``` to add files and folders you want to change.
    - Finally commit those changes using ```git commit -m "Add any commit message here(optional)"```

The commits will be saved in the repo.

> Pushing the repo on Github
The above changes till now are on the local system only. To push these changes on Github write

```git push origin master```

*The repo has been pushed to master branch on github*

### Making Changes in other's project

> Forking a Repo

Creating a “fork” is producing a personal copy of someone else’s project. Forks act as a sort of bridge between the original repository and your personal copy.

To **fork** a repo go to your desired repository on github and click on fork.

> Cloning a repo

After forking a project you get personal copy of that project **but** to make changes or to add features in the project you need to get that on your local developement enviroment.

- On the forked repo click on code and copy the *link*
- Open *git bash* and run following command:
    - ```git clone link```

Now you're all set to make changes in the project.    

### Branch
Git branch is a feature in git used for separating a feature or part of code from master in order not to mess something in our main code
Branches allow us to work over separate parts of the project or code without affecting the master branch (main working code). By default everything is stored in the master branch and when we create a new branch, the same files are copied and we can make changes to it without affecting the files in the master branch. We can add these changes to the master branch or any other branch whenever we want by merging the two branches.

> creating a branch 
   ```git branch branch_name```

> Moving to that branch
   ```git checkout branch_name```

*the above tasks can be done by single line* ```git checkout -b branch_name```. 
This will create a branch and move to that branch automatically. 

> Push changes from Branch
Once the changes are commited they chan be pushed to repository on github.

```git push --set-upstream origin branch_name```

### Merge and Merge Conflict

> Merge
You can combine two branches in your repo.

- Go to base branch where you want to merge your branch.

type ``` git merge branch_name ```

> Merge Conflict
When different files are changed git successfully commits changes but when the same piece of code is changed in two different ways git fails to configure the difference between two commits. Thus it raises conflict which is known as merge conflict.

### Pull Request
PR or pull request is a feature utilised whenever we want to contribute to someone else's repository. Pull requests let you tell others about changes you've pushed to a GitHub repository. In order to contribute to anyone else's project we create a pull request with the title and the description of the changes we want to make. If the project administrator finds the changes useful, he can accept the PR and merge. Creating a PR is subject to merge conflicts. We can only create a PR if there are no unresolved merge conflicts.

### Opening and Resoliving issues

> Creating issues
- Make and checkout to a new branch from master
- Make changes in intro.md file
- Add and commit the changes
- checkout to master branch and repeat step 2 and 3
- Merge the newBranch to master

*This will result in a merge conflict*

> Solving conflict
- abort the merge using ``` git merge --abort ```
- Switch to newBranch
- Make desired changes
- Add and commit
- Switch to master
- merge with master

This will resolve the conflict and now we can make PR on the repo.