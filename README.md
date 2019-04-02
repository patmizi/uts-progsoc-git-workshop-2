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

### Resolving Merge Conflicts

