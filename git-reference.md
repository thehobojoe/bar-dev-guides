
## Checking out a new remote

When testing a PR from a forked repo, you will need to add a new remote.

```
git remote add thehobojoe https://github.com/thehobojoe/Beyond-All-Reason
git fetch thehobojoe
```

Then you will need to check out the desired branch

```
git checkout --track thehobojoe/cool-new-branch
```

Similarly, if you have your own fork and need to update from the main repo, you will need to add the main repo as a remote. When doing this, the convention is to call it `upstream`. So if I am on `thehobojoe/cool-new-branch` and I want to get the latest commits from the main repo, I would do:

```
git pull upstream master
```


## Branching

List branches

```
git branch
```

Create branch

```
git branch new-branch
```

Create and checkout a branch

```
git checkout -b new-feature-branch
```

Delete branch safely (it will not delete if any code is not present on the remote)

```
git branch -d old-branch-name
```

Force delete branch 

```
git branch -D old-branch-name
```
## Merging

## Clearing changes
```
git reset --hard HEAD
```

This will undo all changes and set the repository to the latest commit. Note that this is for only uncommitted changes, it will have no effect on local commits.
## Squashing

TBD. Squashing from CLI is extremely painful, this is where git GUI's can really make things easier