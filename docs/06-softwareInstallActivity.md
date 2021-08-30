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
   find and install GIMP (Graphics Image Manipulation Program),
   a FOSS package for editing images. Run the
   GIMP application to verify that it works.

1. **Snapshot**: Make another snapshot of the system with GIMP
   installed.

1. **Eclipse install, first attempt**:

   * **Confirm No Java**: By default, Ubuntu does not come with Java
      installed. You can confirm this by typing `java` on the command
      line. Note that when you do, Ubuntu will tell you that java is
      not installed and make some suggestions as to which packages you
      might install (using `apt`) to get it. Don't install Java yet,
      just make a note of the suggestions.

   * **Confirm No Eclipse**: Similarly, Ubuntu does not come with
      Eclipse installed. Confirm this by running `eclipse` from the
      command line. Make a note of any suggestions but do not install
      anything yet. The system probably recommended using yet another
      installation program called `snap`. We won't study any details
      of snap here, but you can feel free to use snap as one of your
      install methods in the next part of this activity.

   * **Research Eclipse and Java install**: Use a search engine to
     find some advice on how to install Eclipse and/or Java on Ubuntu
     or more generally on Linux. Make a note of at least two
     approaches that seem promising. Use your best judgment in
     deciding how much time to spend on research; between five minutes
     and 15 minutes is probably suitable.

   * **Install Eclipse**: Your objective here is to get Eclipse
     installed and then compile and run a 'hello world' Java program
     in Eclipse. Choose one of the approaches that you researched in
     the previous part of this activity. Complete the installation.
     Test it by attempting to create and run a 'hello world' project
     in Eclipse.  Make a note of any problems you encountered or
     anything that is not working as expected.

   * **Snapshot**: Make a snapshot of the system now that you have
     completed your first Eclipse installation.

1. **Eclipse install, second attempt**: Even if your installation of
   Eclipse worked perfectly, let's assume that something went wrong so
   that you can practice snapshotting. Recall that in an earlier part
   of this activity, you made a note of at least two approaches to
   installing Eclipse. So far you have implemented only one of those
   approaches.

   * Roll back to an earlier snapshot, then try a second, different
   approach to installing Eclipse. Again attempt to create a 'hello
   world' project and run it.

   * Create another snapshot after this installation.

   * Decide which of your two installations was more successful. If
     your first installation was more successful, switch back to that
     snapshot.

1. *Git**: In order to interact with GitHub for things like
   retrieving code from, or contributing changes to an source project
   you will need to use the `git` command line tool. We won't be using
   this today, but we'll need it for our class on version
   control. So we'll go ahead install it now. Figure out how to use
   apt from the command line to install git. Run `git` from
   the command line to ensure that it has been installed. If it has
   been successfully installed you should see a help screen showing
   the "usage: " of Git and a long list of the "common Git commands."

1. **Snapshot**: Make another snapshot of the system now that you have
   Git installed.

1. **Meld**: When using Git and GitHub for team development,
   situations will arise when two people have changed the same file in
   incompatible ways. When this happens it will be necessary to merge
   the changes manually. A graphical tool for displaying the changes and
   allowing you to choose which change to accept makes this job a lot
   easer. Meld is just such a tool.  Like Git, we won't be using Meld
   today, but let's go ahead and install it so its ready when we need
   it. Figure out how to install Meld. Once you have it installed you
   can verify that it works by typing `meld` on the command line. If
   everything is good then the GUI tool should appear.

1. **Snapshot**: Make another snapshot of the system now that you have
   Meld installed.
