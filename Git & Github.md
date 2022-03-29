## 1. Add local git repo in github
```
git remote add origin https://github.com/w3schools-test/hello-world.git
```

git remote add origin URL specifies that you are adding a remote repository, with the specified URL, as an origin to your local Git repo.

## 2. Github fetch and merge
When working as a team on a project, it is important that everyone stays up to date.

Any time you start working on a project, you should get the most recent changes to your local copy.

With Git, you can do that with pull.

pull is a combination of 2 different commands:

<b>a. fetch</b>

fetch gets all the change history of a tracked branch/repo.

So, on your local Git, fetch updates to see what has changed on GitHub:
```
git fetch origin
```
<b>b. merge</b>

merge combines the current branch, with a specified branch.

We have confirmed that the updates are as expected, and we can merge our current branch (master) with origin/master:

```
git merge origin/master
```

<b>c. pull</b>

pull is a combination of fetch and merge. It is used to pull all changes from a remote repository into the branch you are working on.

Make another change to the Readme.md file on GitHub.

```
git pull origin
```

## 3. Github push

```
git push origin
```

Push the updates from local repo to Github

## 4. Github branch
```
git branch 
```

we can use the -a option to see all local and remote branches:
```
git branch -a
```