## 1. Git Version
```
git --version
```

## 2. Git User Details
```
git config --global user.name "USER_NAME"
git config --global user.email "email@address"
```

## 3. Git Directory creation
```
a. mkdir myproject
```
To create Directory
```
b. cd myproject
```
To change the directory

## 4. Git initialization
```
git init
```
After entering the github repo Initialize the Git Repository.

## 5. Git Status
```
a. git status
```
To check and track the github repository and it's files.

```
b. git status --short
```
### Note: Short status flags are:

1. <i>?? - Untracked files</i>
2. <i>A - Files added to stage</i>
3. <i>M - Modified files</i>
4. <i>D - Deleted files</i>

Files in your Git repository folder can be in one of 2 states:

<b>Tracked - files that Git knows about and are added to the repository
Untracked - files that are in your working directory, but not added to the repository</b>

## 6. Git Staging Environment
One of the core functions of Git is the concepts of the Staging Environment, and the Commit.

As you are working, you may be adding, editing and removing files. But whenever you hit a milestone or finish a part of the work, you should add the files to a Staging Environment.

Staged files are files that are ready to be committed to the repository you are working on.

```
a. git add index.html
```
```
b. git add --all
```

## 7. Git Commit
Since we have finished our work, we are ready move from stage to commit for our repo.

Adding commits keep track of our progress and changes as we work. Git considers each commit change point or "save point". It is a point in the project you can go back to if you find a bug, or want to make a change.

When we commit, we should always include a message.

By adding clear messages to each commit, it is easy for yourself (and others) to see what has changed and when.

```
git commit -m "First release of Hello World!"
```

## 8. Git Commit without Stage
Sometimes, when you make small changes, using the staging environment seems like a waste of time. It is possible to commit changes directly, skipping the staging environment. The -a option will automatically stage every changed, already tracked file.

```
git commit -a -m "Updated index.html with a new line"
```

## 9. Git Commit Log

```
git log
```


## 10. Git Help
If you are having trouble remembering commands or options for commands, you can use Git help.

There are a couple of different ways you can use the help command in command line:

```
a. git command -help
```

See all the available options for the specific command
```
b. git help --all 
```
See all possible commands


## 11. Git Branch

Working with Git Branches
In Git, a branch is a new/separate version of the main repository.

Let's say you have a large project, and you need to update the design on it.

### How would that work without and with Git:

#### <b>Without Git:</b>

Make copies of all the relevant files to avoid impacting the live version
Start working with the design and find that code depend on code in other files, that also need to be changed!
Make copies of the dependant files as well. Making sure that every file dependency references the correct file name
EMERGENCY! There is an unrelated error somewhere else in the project that needs to be fixed ASAP!
Save all your files, making a note of the names of the copies you were working on
Work on the unrelated error and update the code to fix it
Go back to the design, and finish the work there
Copy the code or rename the files, so the updated design is on the live version
(2 weeks later, you realize that the unrelated error was not fixed in the new design version because you copied the files before the fix)

#### <b>With Git:</b>

With a new branch called new-design, edit the code directly without impacting the main branch
EMERGENCY! There is an unrelated error somewhere else in the project that needs to be fixed ASAP!
Create a new branch from the main project called small-error-fix
Fix the unrelated error and merge the small-error-fix branch with the main branch
You go back to the new-design branch, and finish the work there
Merge the new-design branch with main (getting alerted to the small error fix that you were missing)
Branches allow you to work on different parts of a project without impacting the main branch.

When the work is complete, a branch can be merged with the main project.

You can even switch between branches and work on different projects without them interfering with each other.

Branching in Git is very lightweight and fast!

```
a. git branch
  hello-world-images
* main
```

We can see the new branch with the name "hello-world-images", but the * beside main specifies that we are currently on that branch.

```
b. git checkout hello-world-images
```

checkout is the command used to check out a branch. Moving us from the current branch, to the one specified at the end of the command

## 12. Git Branch Merge
Merge Branches
We have the emergency fix ready, and so let's merge the main and emergency-fix branches.

We have the emergency fix ready, and so let's merge the main and emergency-fix branches.

First, we need to change to the main branch (use checkout command to shift to main branch)

```
git merge emergency-fix
```

## 13. Git Delete branch

```
git branch -d emergency-fix
```