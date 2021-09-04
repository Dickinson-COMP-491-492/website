# Git/GitHub Command Cheat Sheet

## Initial Git Configuration:

```
git config --global user.name <GitHubUserName>
git config --global user.email <you@email.org>
git config --global push.default simple
git config --global merge.tool meld
git config --global mergetool.keepBackup false
git config --global credential.helper cache
```

## Fork the Upstream Repository:

1. Log into your GitHub account
2. Go to the repository for the project in GitHub
3. Click on the "Fork" button in the upper right hand corner.

## Clone Origin Repository to Local Machine:
1. From the GitHub repository click the green "Clone or Downlaod" button.
2. Make sure that the URL shown has your GitHub user name in it.
3. Click the little clipboard icon to copy your Origin Repository URL.
4. On your machine: `git clone <Origin Repository URL>`


## Add Upstream Repository as new Remote:

```
git remote add upstream <Upstream Repo URL>
git remote -v
```


## Listing Branches and Creating a Feature Branch:

```
git branch
git branch <newBranchName>
git checkout <newBranchName>
```

## Status, Add, Commit:

```
git status
git add <FileToAdd> [<AnotherFileToAdd> ...]
git commit -m "a descriptive message here."
Display the Commit Log:
git log
```

Within `git log`:
 * return key - advance one line
 * spacebar - advance one screen
 * `q` - terminate log listing


## Push a Feature Branch to Origin:

`git push origin <branchName>`

## Making a Pull Request:

1. Open your `github-issues-activity` repository on GitHub.
2. Click the "New pull request" button.
3. Check that the "base fork" is set to the master branch of the upstream.
4. Set the "head fork" to the branch in your origin with your changes.
5. Verify that the pull request contains the changes that you have made.
6. Click the green "Create pull request" button.
7. Edit the title and the "Leave a comment" box (use "Fixes #<bugid>")
8. Click the green "Create pull request" button.

## Synchronize Local and Origin master branches with Upstream master:

```
git checkout master
git pull upstream master
git push
```

## Delete a Feature Branch:

```
git branch -d <BranchName>
git push origin :<BranchName>
```

## Resolve Conflicts:

```
git checkout master
git pull upstream master
git checkout <BranchName>
git merge master
git mergetool
git status
git commit -m "<descriptive message>"
git push origin :<BranchName>
```

## Force master to match Upstream:

```
git checkout master
git fetch upstream master
git reset --hard upstream/master
git push origin master --force
```

## Undo all uncommitted changes to a file:

```
git checkout -- <bad filename>
```


