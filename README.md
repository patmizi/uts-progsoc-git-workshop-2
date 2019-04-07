## UTS ProgSoc Git Workshop
This portion of the workshop will revolve around what to do when encountering a
merge conflict. Please make sure that you fork this repository and not create your
own.

### Getting Started

To get started, fork this repository.

![fork button on github](./img/fork.png)

The next step is to clone the forked version of this repository. On the main page of the repo, copy the url shown here:

![where to copy url on github](./img/git-clone.png)

Then use the command in your terminal:

```
git clone https://github.com/<your_github_username>/uts-progsoc-git-workshop-2.git
```

You should now be able to redirect into the directory just created using the command line.

Next, it is good to get in the habit after each command to use `git status`. Let us use it now.

```
git status
```

Now check which branch you are on:

```
git branch
```

You should only see `master` which is the default branch in this repo.

When there are other branches in your repo the green branch is the current one you are on.

### Merge Conflicts

This happens when two developers work on the same file at the same time. Usually each branch is supposed to work on
files independent of other branches but sometimes it can't be helped ¯\\\_(ツ)\_/¯

In this exercise you will learn to resolve a merge conflict by pulling in conflicting changes from this upstream
repository.

#### Preparation

To start off, make sure you have no existing changes in the cloned repo

```
git status
```

Next, you will make changes to the index.html file using your favourite text editor. This file is an html document
containing a basic html table with some content.

Add some extra rows to this table and push those changes to the remote repository.

```
git add index.html
git status
git commit -m 'Added some extra rows to the table'
git push
```

#### Creating the merge conflict

After pushing your changes, and under the instruction of the the person running the workshop. You are going
to pull changes from the source of the forked repo. To do this you will need to do the following:

```
git fetch upstream
git pull
```

If done correctly this should create a merge conflict in index.html and you should see the following output:
