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
git switch <newBranchName>
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
3. Check that the "base fork" is set to the main branch of the upstream.
4. Set the "head fork" to the branch in your origin with your changes.
5. Verify that the pull request contains the changes that you have made.
6. Click the green "Create pull request" button.
7. Edit the title and the "Leave a comment" box (use "Fixes #<bugid>")
8. Click the green "Create pull request" button.

## Synchronize Local and Origin main branches with Upstream main:

```
git switch main
git pull upstream main
git push
```

## Delete a Feature Branch:

```
git branch -d <BranchName>
git push origin :<BranchName>
```

## Resolve Conflicts:

```
git switch main
git pull upstream main
git switch <BranchName>
git merge main
git mergetool
git status
git commit -m "<descriptive message>"
git push origin :<BranchName>
```

## Force main to match Upstream:

```
git switch main
git fetch upstream main
git reset --hard upstream/main
git push origin main --force
```

## Undo all uncommitted changes to a file:

```
git restore <bad filename>
```

## Obtain a new GitHub PAT (personal authentication token)

  * The GitHub documentation on [Creating a personal access token](https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token)
explains the procedure in detail. Follow the step-by-step instructions
provided there, taking note of the following points which help with
our specific scenario:
    - You can choose any name you want for this PAT. "Repo access"
      would be an appropriate choice.
    - For the expiration of the token, it will be easiest to use the
      same token throughout the semester. Therefore, choose the Custom
      expiration option and select a date after the end of the
      semester. You can also choose to have no expiry date, if you
      don't care about the security of your GitHub repositories.
    - When choosing the scopes or permissions for the token, select
      the "repo" option and leave everything else unchecked.
    - The random string highlighted in green is your PAT. Copy this
      and save it somewhere secure. Treat it the same way you would
      treat any other password. Anyone who knows this PAT has full
      access to your GitHub repositories.
    - Your PAT now serves the purpose of a password for accessing your
      GitHub repository. Whenever you are asked for a "password" to
      access a repository, you should instead use this PAT. Your
      GitHub account password is still used for accessing GitHub from
      a web browser.

