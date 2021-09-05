# Git and GitHub Workflow activity

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
* [Part 3 - Before the Second Class](#part-3-before-the-second-class):
  You will complete this part following the first class period and
  before the second. In it you will repeat the process of claiming an
  issue, creating a branch, making a fix, pushing the fix to your
  GitHub repo and making a pull request.
* [Part 4 - Hands-On in the Second Class](#part-4-hands-on-in-the-second-class): You will complete this part
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

There are a few settings in the Git configuration that need to be set
before we begin. Note that these commands will only need to be issued
once on each machine where you use Git. Issue the following commands
in a terminal (customizing as appropriate) to setup the Git
configuration:

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
     in GitHub. For this activity you will need to clone the [Dickinson-COMP-491-492/github-issues-activity](https://github.com/Dickinson-COMP-491-492/github-issues-activity)
     repository.
1. Click on the "Fork" button in the upper right hand corner.
1. If a pop-up dialog appears, select your GitHub account from those
   shown.
1. Look at your repositories in GitHub and verify that you have a fork
   of the `git-hub-issues-activity` repository.

### Cloning your Origin

The fork of the upstream repository in your GitHub account is called
your *origin repository*. Because this repository is in your GitHub
account you will be able to both read and write to this repository. It
will provide cloud storage for all of the work you do on the project
and will also be the means for contributing code back to the main
project through pull requests. To work on the code however, you will
*clone* your origin repository onto your local machine making a copy
of it into a *local repository*.

To clone your origin repository:

1. From the github-issues-activity repository click the green "Code" button.
1. Make sure that the URL shown has your GitHub user name in it.
1. Click the little clipboard icon to copy your Origin Repository URL. 
   * There are several different options here, but we want the URL
     corresponding to the "HTTPS" method, which is usually the
     default.
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
1. Use the "Code" button to copy the upstream repository URL (again
   choosing the HTTPS option).
1. Use the command: `git remote add upstream <Upstream Repository URL>`
1. Use the command: `git remote -v`
   * You should now see four lines (2 for origin and 2 for
     upstream). The lines for upstream should contain the course
     GitHub URL and those for origin should contain your GitHub
     username. So something like:
   ```
   origin https://github.com/braughtstu/github-issues-activity.git (fetch)
   origin https://github.com/braughtstu/github-issues-activity.git (push)
   upstream https://github.com/Dickinson-COMP-491-492/github-issues-activity.git (fetch)
   upstream https://github.com/Dickinson-COMP-491-492/github-issues-activity.git (push)
   ```

### Snapshot

Make a snapshot of your virtual machine.

![stop](images/stop.png "stop")Checkpoint![stop](images/stop.png
"stop")


