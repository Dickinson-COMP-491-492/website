## Ubuntu Install

### Introduction
For the first several weeks of the semester you will be completing tutorials, in-class exercises and homework assignments to help familiarize you with some of the types of tools and techniques that are commonly used in H/FOSS projects. We, of course, can't cover them all. However, the experiences of learning new tools and techniques should translate well into learning others that you will inevitably need as you get into your selected H/FOSS project.

All of the tutorials, in-class exercises and homework assignments will use the Ubuntu Linux operating system. In addition, because the vast majority of H/FOSS projects are created and run under Linux based operating systems, learning a bit about it will likely be useful. So the first task will be to get a Ubuntu up and running so that you can use it.

### Prerequisites

Before starting you should read a bit about Linux and Virtual Box. The following sites are good starting points:

- [What is Linux?](https://opensource.com/resources/what-is-linux)
- [Virtual Box: Virtual Machines](https://www.virtualbox.org/wiki/Virtualization)

### Getting Started

For this assignment you will work in pairs to install Ubuntu Linux in Virtual Box. While doing so you will keep a live-log in a Slack channel to document your time and effort on this assignment. To get started:

- One partner must create a new Slack channel:
  - The channel should be private.
  - The channel should be named using your initials and the assignment name (e.g. "gb-zz-ubuntu-install")
  - Invite your partner and your instructor to join this channel.

As you progress through the assignment, use this channel to live-log your activities. Enter questions you have, answers you find, where you found them, steps you've taken, mistakes you've made, how you've corrected them, etc. The idea is for you to paint a picture for me and a record for you of what you've done. Because Slack is indexed and searchable, live-logs of your work can be a great time saver helping you to (re)find answers, reconstruct actions, and avoid repeating mistakes that you've made before. Live-logs will also provide a means for me to assess your time and effort investment on assignments (see the Syllabus).

You can review the #sample-live-log channel in our Slack Organization to see a small example of what a live-log might look like.

One way to work would be for one partner control the computer on which the work is occurring while the other partner keeps the live-log on another computer. If you frequently switch roles then both partners gain experience with the assignment and with live-logging.

### Virtual Box

[Virtual Box](https://www.virtualbox.org/wiki/VirtualBox) is a "a general-purpose full virtualizer for x86 hardware." In other words, Virtual Box is a program that acts like it is a full machine. It allows you to run a full "guest" operating system (OS) and associated software inside a window on a "host" computer (e.g. Linux (guest) in a window on a Mac (host)). Some advantages of this arrangement include:

- You can have administrative privileges on the guest OS without having them on the host OS (e.g. in a departmental lab). This is useful because many installations and configurations require admin privileges.
- The guest OS can be started up, shut down and rebooted much more quickly than the host machine. This is useful because many installs and configuration changes require reboots.
- You can take snapshots of the system state at any point and restore them at any point. This is useful because it is not unusual to "muck up" the system when first learning about installation and configuration of systems. This is compounded by having admin privileges (as discussed above)! But, as long as you have a clean snapshot, you can easily go back and try again if (when!) something gets "mucked up".

You have two options for using Virtual Box:
- Lab Machines: Virtual Box is pre-installed on the lab computers and can be found in the "Applications" folder or via the Spotlight search tool.
  - If you install on a lab machine it is recommended that you store the virtual machine files on OneDrive so that you can use them from any lab computer.  Note however, that moving to a new machine will require that these files synch to that machine which is slow the first time because they are large.  Thus, it is advantageous to use the same machine each time.
- Personal Machine: You may download and install Virtual Box on your own computer from the Virtual Box Downloads page. To take this approach you must have an Intel processor, at least 8GB of RAM (16GB preferred) and a least 75GB of free disk space.  If your computer does not meet those specifications it is recommended that you use a lab computer.  Note: VirtualBox will not run on M1 base Macs.  _If you are feeling ambitious you could try [UTM](https://mac.getutm.app/), however the department faculty will not be able to provide the same level of assistance and support with that platform.  If you are going this route please discuss it with your instructor in advance._

Be sure you are able to launch Virtual Box (either on a lab machine, or your machine) before proceeding to the next section.

### Ubuntu Linux

[Ubuntu](http://www.ubuntu.com/) is a popular flavor of the linux operating system and is what we'll use for the next several weeks. Many of you may then find that it is also a good choice for working with your H/FOSS projects. Though, once you get a feel for Ubuntu, it is relatively easy to move to other flavors of linux if they are a better match to your project.

#### Tasks:

1. Download Ubuntu 20.04 Desktop
2. Install Ubuntu 20.04 into a Virtual Box virtual machine.
   - When doing the install some system specifications will need to be set. The following seem to work well.
     - Allocate the virtual machine about half of the physical RAM (but no less than 4GB of RAM.)
     - Allocate a virtual disk at least 40GB.
     - Maximize the amount of video memory available to the virtual machine (128 MB).
     - Create whatever username and password you like - but you'll need to remember and type it!
     - If you are working on a Mac with a retina display (in the lab or your own) you'll want to configure [VirtualBox to be launched in Low Resolution Mode](https://forums.virtualbox.org/viewtopic.php?f=8&t=90446&start=75#p470879)

   - How do you install? Use your favorite search engine to find some installation instructions. I'd suggest something like the following:
     - Search for "Ubuntu Virtual Box Install" and see what comes up.
     - You may need to browse through a number of pages to find something that matches reasonably close to what you are doing (i.e. right version numbers, host os, etc). If there is an exact match for what you want to do and it looks doable - great. If not, browse around until something looks pretty close and resonates with how you think and work.
     - Give it a go. But remember, don't panic and don't be afraid to try things, you are working in a virtual machine, so if you muck it all up, just create a new one and try again!
     - When you get stuck or have questions... search some more, ask a classmate, ask the professor. Remember, getting stuck, confused and learning new stuff is all part of what's expected in this class. So don't hesitate to ask questions!!!
3. Install the VirtualBox Guest Additions for Ubuntu. These additions greatly improve the interaction between the host operating system (e.g. MacOS) and the guest operating system (e.g. Ubuntu). This includes better graphics performance, the ability to copy and paste into and out of the VM, and a host of other smaller features. Once you have the guest additions installed try to copy and paste from the guest to the host and vice versa to confirm that they are working (note: Getting this to work will also require a small configuration adjustment).
   - How? Use your favorite search engine to find some instructions.
4. Once your virtual machine is up and running and you can log in, create a VirtualBox snapshot of its current state.  This will allow you to reset to this state, rather than re-installing, if something goes wrong in the future.
   - How? Use your favorite search engine to find instructions for creating snapshots in VirtualBox.  
5. With Ubuntu running, open a text editor and type in your name and your partner's name and "COMP491 Fall <YEAR>". Then take a screen shot of the VirtualBox window and include it in your Live-log.
   - How do you take a screen shot? You guessed it... use your favorite search engine...

---

Acknowledgements: This assignment builds from and adapts ideas and content from the following activities created by others:
- http://foss2serve.org/index.php/Installing_a_Virtual_Machine
