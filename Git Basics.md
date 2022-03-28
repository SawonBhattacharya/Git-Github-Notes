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