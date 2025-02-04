# Repo initialisation & conflict management in git.

## Initialising a local repo

Initialising a local git repo, using the following command on the `root folder.`

```
git init
```

### Cloning a repo,

```
git clone repo-url
```

## creating & changing branches

To create a `feature` branch, 

```
git checkout feature/branch
```

This command creates a branch named `feature/branch`, if you want to switch to already available branch `git branch -b new-branch/feature `the branch already exists changes the   `HEAD` to the mentioned branch

use `git branch -a` for listing all available branches.


## pushing changes to a repo.

The workflow when done commiting changes to the repo,

```
git add .
```

The above commands `stages` all the changes made to the file, 

```
git commit -m "feat: features added/ changed"
```

This stages the commit,

```
git push origin main
```

pushes the changes made to the remote repository.

## checking for `diff` in github,

`diff` is the workflow to check for changes made by different developers working on the same file/folder.

checking for changes made to the `root` initialised folder,

```
git status
```

for checking changes made to specific files:

```
git diff file-name
```

for checking changes make to a branch

```
git diff branch-name
```

## Best practices for `pre-commit` workflow.

- Always `git pull --rebase` for changing the file to latest commit. 
-
