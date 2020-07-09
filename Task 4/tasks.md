> Day 1

**Q1. What do you mean by git and GitHub?**
*ans:*
Git is a piece of software that does version control system. It lets you manage and keep track of entire history that you are working on your computer.
                              Git is a particularly special tool which has a lot of advanced and sophisticated features for collaboration.First developed in 2005.
-GitHub is a cloud-based hosting service that lets you manage Git repositories. If you have open-source projects that use Git, then GitHub is designed to help you better manage them.


**Q2.  Why GitHub is so popular and used in most of the projects?**
*ans:*
GitHub is a Git repository hosting service, but it adds many of its own features. While Git is a command line tool, GitHub provides a Web-based graphical interface. It also provides access control and several collaboration features, such as a wikis and basic task management tools for every project.GitHub is the world's largest software development platform. It provides cloud storage for source code, supports all popular programming languages, and streamlines the iteration process.

**Q3. What is a version control system? How Git is a VCS?**
*ans:*
Version control systems are a category of software tools that help a software team manage changes to source code over time. Version control software keeps track of every modification to the code in a special kind of database.
                          Git is a VCS because it allows to manage the multiple track of your files stored in your computer.

**Q4. What are the other platforms similar to GitHub?**
*ans:*

Other platforms similar to GitHub:-
- GitLab
- SourceForge
- Google Cloud Source Repositories
- GitKraken
- Apache Allura
- BitBucket
- Launchpad
- AWS CodeCommit



**Q5. Why are you interested in learning of Git and Github?**
*ans:*

- Have your code reviewed by the community.
- GitHub is a repository, it allows your work to get out in front of the public.
- GitHub also tracks changes in a changelog, so you can know exactly what is changed each time.
- Use Multiple Integration Options.

> DAY 2

**a. How git workflow works?**
*ans:* Git workflow defines a branching model which provides a systematic framework for managing projects. It keeps checks of the versions and the changes commited, provides liberty in making branches and switching between versions.

**b.What are the different stages of git project as commit, add?**
*ans:* The main stages of git project are
         - status:  displays the status of working directory as well as tells you what changes have been committed.
        - add: Add the changes in the working directory to staging area
        - commit: updates the changes added to staging area.

**c. Is it possible to do a git commit before git add. If you have made any changes. Explain why?**
*ans:* No, it is necessary to add the changes before commiting that to staging area otherwise git won't know what changes do we want to make.

**d. Why is git diff used?**
*ans:* Git diff provides us the difference between the previous and the current version of the file.

**e. Can we leave commit message as blank?**
*ans:* Yes but this is not considered as a good practice as message help us to keep record of (by using git log) the changes we've made.

> Day 3

**Share the link of the PR you've made.**
<a href="https://github.com/codewayy/github_series/pull/134">PR1</a>
<a href="https://github.com/codewayy/github_series/pull/135">PR2</a>

**a) What is meant by the term fork and clone?**
*ans:* Forking a project means creating a personal copy of the project for making changes, debugging etc.
After forking any project, the project remains on the github account. In order to make changes in the files we clone the project to get that in our system.

**b) What are branches in github?**
*ans:* Branches are different roadmaps that someone can go through while working in git environment. All the branches whirl around the master branch. Side branched can pe made to do experimental changes of in case you are working in a team.

**c) What is PR?**
*ans:* After commiting changes in a project the local repo is compared with original repository and a pull request is generated to ask the original repo to apply the changes. PR could be accepted or rejected but it doesnt makes any difference in forked repo.

**d) Can we delete master branch? If not why?**
*ans:* Master branch is root of the repo so in to deleted master branch any other branch should be assigned as our root branch. After that, the selected branch starts acting as master. After that we can delete  the branch which was previously master.

**e) How can we delete a branch?**
*ans:* To delete a branch first we need to get out of that branch as git doesnt allow to delete a branch we are currently working on.
after that we can use

```
git branch -d localBranchName  //to delete a branch locally
git push origin --delete remoteBranchName //to delete a branch remotely

```


