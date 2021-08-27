# Software Installation Activity

## Introduction

Using, working with or contributing to an H/FOSS project will
invariably require you to install some additional software on your
computer. There are three primary ways of accomplishing this on
Linux. There are graphical software managers, like the Ubuntu Software
app (often referred to as Ubuntu Software Center), that allow you to
browse and install available software in a GUI. There are also tools,
like `apt`, `dkpg` and `yum`, that install software from the command
line. Finally, it is also possible to download, build and install
software from its source code. The exercises below will guide you
through the process of installing some software onto Ubuntu using the
graphical Ubuntu Software app and also the `apt` command line
tool. We'll build and install a program from source in another
exercise later in the semester.

## Prerequisites

It is assumed you have already watched the videos assigned as required
preparation for [today's class](06-LinuxSysAdmin.md).

## Exercises

Complete each of the following exercises:

1. **Snapshotting**: Any time you are doing system configuration or
   installs, it is a good idea to take a snapshot. Sometimes an
   install will not work or you'll try several things before getting
   it to work. This can leave unnecessary changes or files on the
   machine. If you have a *snapshot*, you can roll back to the state
   before you started and do a clean install once you have it all
   figured out. Also, if something were to go horribly wrong, you can
   roll back to a known stable state. Make a snapshot of your current
   VM state in Virtual Box and give it a descriptive name.

1. **Software Manager**: `apt`, and similar tools (e.g. `snap`, `yum`,
   `dnf`, `pkg`) used by different Linux flavors, provide powerful
   ways to install software from the command line. However, if you do
   not know exactly what you want to install, a graphical tool that
   allows you to browse the available software may be preferable. In
   Ubuntu, the Ubuntu Software application (usually visible as a the
   suitcase icon) is such a tool. Use the Ubuntu Software app to
   find and install GIMP, a FOSS package for editing images. Run the
   GIMP application to verify that it works.

1. **Snapshot**: Make another snapshot of the system with GIMP
   installed.

1. **Confirm No Java**: By default, Ubuntu does not come with Java
   installed. You can confirm this by typing `java` on the command
   line. Note that when you do, Ubuntu will tell you that java is not
   installed and make some suggestions as to which packages you might
   install (using `apt`) to get it. Those suggestions will install the
   OpenJDK and we will need to install the Oracle JDK instead. So
   don't follow those suggestions, go onto the next step...

1. **Oracle JDK Install**: Linux suggests installing the Open JDK. This
   is a good alternative to the Oracle JDK in a lot of cases. However,
   the Oracle JDK is still the gold standard and is preferred (or
   needed) by many applications. Figure out how to use apt from the
   command line to install the latest Oracle Java Developer Kit
   (JDK). Once you have installed it, use the command java -version to
   verify it. The output should include something similar to "Java(TM)
   SE Runtime Environment ... (build ...)", the exact build number
   will differ but should correspond to the latest JDK. Also run javac
   -version to verify that the Java compiler is also present in
   addition to the runtime environment.

1. **Snapshot**: Make another snapshot of the system now that you have
   Oracle Java installed.

1. **Eclipse Install (take 1)**: The eclipse IDE is not installed in
Ubuntu by default, but may be something useful to have. Type eclipse
on the command line to verify that it is not installed. Note, that as
with the java command above, Ubuntu is quite helpful here and tells
you what package to install to get eclipse.  Use apt from the command
line to install eclipse.

Notice that when you run apt to install eclipse it lists a large number of other packages to install or upgrade. One of the great features of package managers such as apt is that they will not only install the package you ask it to, but also any other packages that it needs to run (i.e. on which it depends). So in this case, installing eclipse also installed a wide range of other packages on which eclipse depends, saving you a lot of work!

Try to run eclipse from the command line.

You'll notice that it does not work! Apt attempted to install eclipse 3.8.1 which has an incompatibility with some of the installed libraries. This is something you will encounter fairly regularly in the Linux world.

Also run java -version again. You'll notice that apt switched the the default version from the Sun Java to the Open JDK that was installed as a dependency of eclipse. You'll also need to be careful of things such as this when doing system administration tasks in Linux. We could attempt to fix this issue by doing installs of different libraries and dependencies and we may eventually get eclipse to run. But it turns out there is a newer version of eclipse that can be installed with the snap command which will function properly.


1. **Roll Back**: You could simply try the snap command to install
eclipse, however it if works you will be left with all of the extra
dependencies installed by the apt command. So instead, we will roll
back to the snapshot you created before trying to install eclipse and
try again from that point.  Shut down your virtual machine and restore
to the snapshot from before you attempted to install eclipse. Confirm
that you have rolled back by trying to launch eclipse from the command
line. You should again see the messages about using snap or apt to
install eclipse.

1. **Eclipse Install (take 2)**: Use the snap command suggested by
   Linux to install eclipse 4.8.0. Confirm that snap did not modify
   the default java version. Then run eclipse from the command line
   and lock it to the launcher.

1. **Snapshot**: Make another snapshot of the system now that you have
   Eclipse installed.

1. **git**: In order to interact with GitHub for things like
   retrieving code from, or contributing changes to an source project
   you will need to use the git command line tools. We won't be using
   these today, but we'll need them for our class on Version
   Control. So we'll go ahead install them now. Figure out how to use
   apt from the command line to install the git tools. Run git from
   the command line to ensure that it has been installed. If it has
   been successfully installed you should see a help screen showing
   the "usage: " of git and a long list of the "common Git commands."

1. **Snapshot**: Make another snapshot of the system now that you have
   git installed.

1. **Meld**: When using git and GitHub for team development,
   situations will arise when two people have changed the same file in
   incompatible ways. When this happens it will be necessary to merge
   the changes manually. A good tool for displaying the changes and
   allowing you to choose which change to accept makes this job a lot
   easer. Meld is just such a tool.  Like git, we won't be using Meld
   today, but let's go ahead and install it so its ready when we need
   it. Figure out how to install Meld. Once you have it installed you
   can verify that it works by typing meld on the command line. If
   everything is good then the GUI tool should appear.

1. **Snapshot: Make another snapshot of the system now that you have
   Meld installed.
