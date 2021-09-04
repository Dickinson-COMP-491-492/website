# Git and GitHub Workflow activity

[under construction]

## Introduction

Many H/FOSS projects use GitHub as the repository for their source
code. This activity is designed to familiarize you with the common
workflow elements for interacting with H/FOSS projects hosted on
GitHub. The activity is divided into four parts:

* [Part 1 - Before the First Class](#part-1-before-the-first-class):
  You will complete this before the first hands-on class period with
  Git/GitHub. It will walk you through the process of configuring Git,
  forking a repository on GitHub, cloning that repository to your
  local machine, and setting up an upstream remote in Git.
* [Part 2 - Hands-On in the First
  Class](#part-2-hands-on-in-the-first-class): You will complete this
  part hands-on during the first class period. It will walk you
  through the process of claiming an issue, creating a working branch,
  fixing the issue, pushing the fix to your GitHub repo, making a pull
  request, and keeping your local and remote repos into synch with
  upstream changes.
* Part 3 - Before the Second Class: You will complete this part
  following the first class period and before the second. In it you
  will repeat the process of claiming an issue, creating a branch,
  making a fix, pushing the fix to your GitHub repo and making a pull
  request.
* Part 4 - Hands-On in the Second Class: You will complete this part
  hands-on during the second class period. It will walk you through
  the process of resolving conflicts with concurrent upstream
  changes. You will synchronize your repos with the upstream, use a
  graphical merge tool to resolve conflicts and update your pull
  request before finally resynchronizing your repo with the upstream
  one final time.
  
## Prerequisites:

* A basic familiarity with Git is helpful before beginning this
activity. The following sites provide good starting points:
  - [Learn Git Branching: Introduction Sequence
(1-4)](https://learngitbranching.js.org/) 
  - [Video Introduction to Git](https://git-scm.com/videos)
* You should have already completed the Software Installation
  activity. All work for this Git/GitHub Workflow activity should be
  completed in the Ubuntu install from the Software Installation
  activity.
* In addition, you should have received and accepted the e-mail
  invitation from GitHub "to collaborate on the
  `github-issues-activity` repository."

## General Information:

In the following text, commands to be typed at the terminal are shown
in mono-spaced type `like this` and any parts of those commands that
you will need to customize for yourself are shown in angle brackets
`<*like this*>`. The angle brackets are not part of the command and
should be omitted when you fill in the appropriate values.

Each time you reach a ![stop](images/stop.png
"stop")*Checkpoint*![stop](images/stop.png "stop"), please stop and
wait. These are points at which we will discuss subtleties of the
operations and ensure that the class is progressing together. If you
reach a checkpoint before other groups, check to see if you might be
able to provide assistance.

The [slides used during the activity](07-githubslides.pdf) are
available for later reference. The titles of the slides illustrating
each task correspond to underlined sub-section names below.

A [GitHub cheatsheet](07-github-cheatsheet.md) with a short summary of each of the sets of commands that we use for particular tasks is also available.

## Part 1: Before the First Class

In order to allow us to focus on the more interesting and complicated parts of Git/GitHub in class you are asked to do some parts of this activity now, before the first class period. You'll also be asked after this class to do some additional work in preparation for the second class period.

### Configuring Git

There are a few settings in the Git configuration that need to be set before we begin. Note that these commands will only need to be issued once on each machine where you use Git. Issue the following commands (customizing as appropriate) to setup the Git configuration:

```
git config --global user.name <GitHubUserName>
git config --global user.email <you@email.org>
git config --global push.default simple
git config --global merge.tool meld
git config --global mergetool.keepBackup false
git config --global credential.helper cache
```

Use the following command to ensure that you have set all of the configurations:

```
git config --global --list
```


### Forking the Upstream

Any H/FOSS project on which you will work will maintain a repository
on a Git compatible site that contains all of the code for the
project. We will use GitHub, but a similar process exists for all of
the others as well. The project's repository will be read-only except
for the core project team that manages the project. So to work on the
code for the project you will create a copy of the repository in your
own GitHub account. The process of making this copy is called *forking*
and the repository belonging to the H/FOSS project itself is called
the *upstream repository*.

To fork the Upstream Repository:

1. Log into your GitHub account
1. Go to the repository for the project in GitHub
   * Often you would have this URL or you can use the search feature
     in GitHub. For this activity you will need to clone the
     `COMP491/github-issues-activity` repository.
1. Click on the "Fork" button in the upper right hand corner.
1. If a pop-up dialog appears, select your GitHub account from those
   shown.
1. Look at your repositories in GitHub and verify that you have a fork
   of the `git-hub-issues-activity` repository.

### Cloning your Origin

The fork of the upstream repository in your GitHub account is called your *origin repository*. Because this repository is in your GitHub account you will be able to both read and write to this repository. It will provide cloud storage for all of the work you do on the project and will also be the means for contributing code back to the main project through pull requests. To work on the code however, you will *clone* your origin repository onto your local machine making a copy of it into a *local repository*.

To clone your origin repository:

1. From the github-issues-activity repository click the green "Clone or Download" button.
1. Make sure that the URL shown has your GitHub user name in it.
1. Click the little clipboard icon to copy your Origin Repository URL.
1. Open a terminal window on your machine.
1. Navigate to the directory where you want to store your cloned
   repository.
1. Use the command: `git clone <Origin Repository URL>`
1. Verify that you now have a local repository:
   - You should have a directory named `github-issues-activity` in the
     current directory.
   - Change into the `github-issues-activity` directory.
   - Verify that it contains three files (`Calculator.java`, 
     `Instructor.md`,  `README.md`).

### Setting the Upstream Remote

You now have a local repository which is a clone all of the code in
your origin repository, which was forked from the upstream
repository. Your origin repository and the upstream repository are
both referred to as *remote repositories* in Git terminology,
reflecting that they are not local to your machine. The Git tool on
your machine will keep track of the remote repositories (i.e. your
origin and the upstream) corresponding to your local repository. This
will be useful when working on H/FOSS projects to push changes from
your local repository to your origin and to pull changes made by
others in the upstream into your local repository. However, at this
time your Git tool only knows about your origin remote because that is
the repository you cloned. You will need to tell Git where to find the
upstream repository.

To set the Upstream Repository:

1. Change into the github-issues-activity directory.
1. Use the command: `git remote -v`
   * This will list all of the remote repositories that Git knows
     about. At this time it should list only your origin repository (2
     lines, one for fetch and one for push). Verify that the URL for
     the origin contains your GitHub username in the URL. So something
     similar to: 
     ```
     origin https://github.com/braughtstu/github-issues-activity.git (fetch)
     origin https://github.com/braughtstu/github-issues-activity.git (push)
     ```
	 If it does not and instead contains the course GitHub URL
     from which you forked the repository you will need to delete the
     github-issues-activity directory and repeat the "cloning your
     origin" step above before continuing.
1. Go to the upstream repository on GitHub.
1. Use the "Clone or Download" button to copy the upstream repository URL.
1. Use the command: `git remote add upstream <Upstream Repository URL>`
1. Use the command: `git remote -v`
   * You should now see four lines (2 for origin and 2 for
     upstream). The lines for upstream should contain the course
     GitHub URL and those for origin should contain your GitHub
     username. So something like:
   ```
   origin https://github.com/braughtstu/github-issues-activity.git (fetch)
   origin https://github.com/braughtstu/github-issues-activity.git (push)
   upstream https://github.com/COMP491/github-issues-activity.git (fetch)
   upstream https://github.com/COMP491/github-issues-activity.git (push)
   ```

### Snapshot

Make snapshot of your virtual machine.

![stop](images/stop.png "stop")Checkpoint![stop](images/stop.png
"stop")


## Part 2: Hands-On in the First Class

In a common GitHub workflow you will, as you have done, fork a repository (the Upstream repo) into your own GitHub account (your origin repo) and then clone that to your local machine (your Local repo). At that point your local repo, your origin repo and the upstream repo will all be identical. In addition, each of these repositories will have a *main branch*, which contains the current reference version of the code according to the upstream repository.

In practice you will never edit code on the main branch. Instead, each time you want to work on the code (add a feature, fix a bug, etc) you will create a new *feature branch* and edit the code there. The feature branch behaves like it is a full copy of the main branch, but git is smart enough to just store the changes you make without making a full copy. In other words, it really just keeps track of the changes that would have to be made to get from the main branch to the version in your feature branch. By editing code on your feature branch, you will be able to leave the main branch in a state that is consistent with the upstream repository. This will be very helpful in integrating changes made by others into your local and origin repositories. It also has the advantage of making it easy to discard changes if you decide they are not working out.

As you work on the feature or bug fix you'll *commit* changes to the feature branch in your local repo. When you've finished work on the feature or bug fix you'll push your feature branch to your origin and then issue a pull request for that feature branch to the upstream. The manager of the upstream can then merge your changes into the project (most likely after asking for some additional work).

The following steps walk you through the basic process of creating and working on a feature branch, committing changes to your local repository, pushing a feature branch to your origin, creating a pull request and finally bringing your local and origin main branches back into sycnh with the upstream.

### Claim An Issue

Go to the GitHub Issues tab on the upstream repository and browse the
"Round1" bugs. Comment on one of the "Round1" tickets that you want to
fix. Refresh the page and check if you are the first commenter on the
ticket. If you are, then the bug is yours. If you are not the first
commenter on the issue try another until you are!

 ![stop](images/stop.png "stop")Checkpoint![stop](images/stop.png
"stop") 

### Branch and Fix

As described above you should never edit code on the main branch. So any time you plan to make changes to the code you will need to create a new feature branch.

To create a feature branch:

1. Open a terminal on your machine.
1. Change into the directory containing your local repository.
1. `git branch`
   * This will list all of the branches in your local
     repository. Currently there is only a main branch. Also notice
     that a `*` appears beside main. This indicates that the files on
     which you are working are those as they exist in the main branch.
1. `git branch round1fix`
   * This creates a new branch named round1fix in your local
     repository.

1. `git branch`
   * Notice the difference.
   
1. `git checkout round1fix`
   * This will switch you to the round1fix branch and allow you to
     edit the files on that branch, ensuring that the files in the
     main branch are unchanged and remain consistent with the
     upstream.
   
1. `git branch`
   * Notice the difference.
   
Now edit the `Calculator.java` file to make the fix described in the
issue that you claimed. Be sure not to edit any other code in the
class.

`gedit Calculator.java`

If time permits you should also be sure that your modified code
compiles:

`javac Calculator.java`

 ![stop](images/stop.png "stop")Checkpoint![stop](images/stop.png
"stop") 

### Status, Stage and Commit

When you edit a file you are changing its contents but not the copy
that is in your local repository. To make your changes part of the
local repository you will *commit* the changes to the
repository. There are several steps to this process.

Determine which files have been changed, add the changed files to be committed to the repository to the *staging area* and confirm that they have been added:

```
git status
git add <FileToAdd>
git status
```

Once the files are in the staging area they can be committed to the
repository. Each commit should reflect a complete unit of work and the
commit should have a clear message indicating what that work was.

Commit your change to your local repository and verify they have been committed:

```
git commit -m "<a descriptive message here>"
git status
```

You can also see a list of the commits that have been made to the
repository:

`git log`

Within the `log` program:
  * return - advance one line
  * space - advance one screen
  * `q` - terminate log listing

Just to get a little more feel for the way your local repository
behaves do the following:

1. `cat Calculator.java`
   * Is your change there?
1. git checkout main
1. git branch
1. cat Calculator.java
   * Is your change there? Why not?
1. git checkout round1fix
1. git branch
1. cat Calculator.java
   * Is your change there?

![stop](images/stop.png "stop")Checkpoint![stop](images/stop.png
"stop") 

### Push Branch to Origin

The changes you have made are now in your local repository with a nice
descriptive commit message. To contribute those changes to the
original project you'll need to first push your feature branch from
your local repository to your origin.

Push your branch to origin:

`git push origin round1fix`

You will be asked for your GitHub username and password. However,
GitHub security measures require that instead of your password you
should use a PAT (personal authentication token). See the GitHub
documentation on [Creating a personal access
token](https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token).

Check that your feature branch and changes have been pushed to your origin by looking at the `github-issues-activity` repository in your GitHub account. You should verify several things:

* There is a message about "Your recently pushed branches" that should
  indicate that `round1fix` was just pushed.
* The dropdown list with "Branch: main" will now contain "round1fix"
  when you open it up.
  - If you choose "round1fix" the `Calculator.java` file will contain
    your change.
  - If you choose "main" the `Calculator.java` file will not contain
    your change.
 
![stop](images/stop.png "stop")Checkpoint![stop](images/stop.png
 "stop")

### Making a Pull Request

A *pull request* is the mechanism by which code changes that you have made can be contributed back to a project. More specifically, it is a request, through GitHub, from you to a project asking them to consider incorporating changes you have in your fork of their project (i.e. your origin) into their repository (i.e. the main branch of the upstream).

Make a pull request for your `round1fix` branch:

1. Open your github-issues-activty repository on GitHub.
1. Click the "New pull request" button.
1. Check that the "base fork" is set to the main branch of the upstream.
   * This is always the branch where you want your changes to go. In
     this case, into the main branch of the `github-issues-activity`
     repository for the course.
1. Set the "head fork" to the `round1fix` branch in your `github-issues-respository`.
   * This is always the branch that contains the changes that you want
     to have integrated into the upstream.
1. Scroll down and verify that the pull request contains the changes
   that you have made:
   * Your commit message should be listed.
   * The changes you made to the `Calculator.java file` should be shown.
1. Click the green "Create pull request" button.
1. Edit the title and the "Leave a comment" box to give information
   about the changes you are proposing.
   * Use this to explain to the project managers what you have done
     and why. In particular, because this work resolves an issue from
     the issue tracker the issue should be referenced in the
     comment. Include the text "Fixes #bugid" (e.g. `Fixes #123`) to
     indicate which bug your changes have fixed. We'll see later that
     this will allow the issue to be automatically closed if/when the
     project managers merge your pull request into the upstream main.
1. Click the "Create pull request" button.

Once you create the pull request it will be reviewed by the project
managers. If everything looks good they will merge the changes into
the main branch of the project. The more likely scenario is that they
will comment on your pull request with some additional things to
consider or other changes to make. When you do that you can then
update your pull request by pushing the branch to your origin
again. They will then review the pull request again. This cycle may
repeat several times before your proposed changes are actually merged
into the project.

 ![stop](images/stop.png "stop")Checkpoint![stop](images/stop.png
"stop") 

### Synchronize Local and Origin with Upstream

Once your pull request, and everyone else's too, has been merged into
the upstream main, the main branch of your local and origin
repositories will be out of synch with (i.e. different than) the
upstream main. This will occur frequently in any project where there
are multiple developers contributing. When this happens you will need
to synchronize your repositories with the upstream repository. This is
done by *pulling* the changes from the upstream main and *merging*
them into to the main branch of your local repo and then finally
pushing them to your origin. Because you have been careful to never
edit the code in the main branch of your local repo this is an easy
process.

Verify that your local main is out of synch with the upstream:

1. `git checkout main`
1. `git branch`
   * Ensure that you are on the main branch.
1. `cat Calculator.java`
1. Compare what you see in the terminal to the version of
   `Calculator.java` that is in the upstream repository on GitHub.
   * Your local version should contain no changes, not even yours. The
     upstream should contain everyone's changes, including yours.

Synchronize your main branches with the upstream main:

1. `git checkout main`
1. `git branch`
   * Ensure that you are on the main branch.
1. `git pull upstream main`
1. `cat Calculator.java`
1. Check that what you see now in the terminal is identical to the
   version of `Calculator.java` that is in the upstream repository on
   GitHub.
1. Verify that the changes do not yet exist in the version of
   `Calculator.java` in your origin on GitHub.
1. `git push origin main`
1. Check that the version of `Calculator.java` in your origin on
   GitHub now contains the changes too, and thus your local and origin
   main branches are now in synch with the upstream.

 ![stop](images/stop.png "stop")Checkpoint![stop](images/stop.png
"stop") 

### Delete a Feature Branch

Once the changes made in a feature branch have been merged into the upstream there is no need to keep the feature branch around. Thus, the feature branch can be deleted from your local and origin repositories.

Delete the feature branch from your local and origin:

1. `git branch -d round1fix`
1. `git branch`
   * Verify that the `round1fix` branch is no longer in your local
     repo.
1. Notice that the `round1fix` branch still exists in your origin on
   your GitHub.
1. `git push origin :round1fix`
   * Notice the ":" before `round1fix`!
   * Reload your GitHub origin repository page in the browser and
     verify that the `round1fix` branch has been deleted.

![stop](images/stop.png "stop")Checkpoint![stop](images/stop.png
"stop")
