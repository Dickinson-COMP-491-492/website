# Unix Tool Challenge Activity

Complete each of the following challenges and append the commands that
you use to the Live-log used for the Linux Tutorials homework. These
are best completed using your Ubuntu install in VirtualBox. A solution
to each challenge is given at the bottom of this webpage. Note that
there are multiple possible ways to accomplish each of these
challenges. If your solution is different, try running the instructor's
solution and see if it gives the same results as yours.

1. Give a command line using the `ps` command that displays all processes that are running on the system (should be more than a hundred).

1. Give a command line using the `ps`, `tail` and `wc` commands, with pipes, to display just the number of processes that are running in the current terminal session (use `ps` alone to check your results).

1. Give a command line using `grep` with your solution to the previous challenges to display the number of processes that are running whose programs live in the `/usr/bin` directory.

1. Open a new terminal window and run the `xeyes` command. Give a command line that will terminate (i.e. kill) the `xeyes` process when executed in a separate terminal window.

1. Learn about the `find` command using its man page.

1. Give a command line using `find` that displays the location of all files named `passwd` that reside within a depth of 5 sub-directories of the machine's root directory.

1. In the last challenge, there are many `permission denied` error messages written to standard error (similar to standard output and appears on the console). Give a command line that redirects standard error to the file `/dev/null` so that these error messages are discarded and the results can be seen more easily. Note: `/dev/null` is a pseudo file on Unix systems that simply discards all data written into it.

1. Consider the `passwd` file in the `/etc` directory from the previous exercise. This file contains one line for each valid user in the system (use `cat` to examine it). Each line has a number of fields delimited by `:` characters. The next to the last field gives the path to the user's home directory (e.g. `/home/braught`). Give a command line that will write the path to the home directory for the `root` user into a file named `userhome.txt` in the `/var/tmp` directory. Hint: `man cut`. Note: `/var/tmp` is a directory on Unix machines that all users can write to and is usually used for temporary files.

1. Give a command line that will append the path of the home directory of your user to the `userhome.txt` file.

1. If there is more time remaining, try some of the following Hacker Rank challenges (you may need to learn about some additional Unix commands as you go):
   1. [The Middle of a Text File](https://www.hackerrank.com/challenges/text-processing-in-linux---the-middle-of-a-text-file)
   1. [tr Command #1](https://www.hackerrank.com/challenges/text-processing-tr-1)
   1. [sort Command #7](https://www.hackerrank.com/challenges/text-processing-sort-7)
   1. [uniq Command #3](https://www.hackerrank.com/challenges/text-processing-in-linux-the-uniq-command-3)
   1. [paste Command #2](https://www.hackerrank.com/challenges/paste-2)
   1. [grep Command #5](https://www.hackerrank.com/challenges/text-processing-in-linux-the-grep-command-5)
   1. [sed Command #3](https://www.hackerrank.com/challenges/text-processing-in-linux-the-sed-command-3)
   1. [awk Command #1](https://www.hackerrank.com/challenges/awk-1)
   1. [awk Command #2](https://www.hackerrank.com/challenges/awk-2)


## Challenge solutions

The solutions are padded with plenty of space to make it less likely
that you will accidentally see the answer to challenge n+1 when
consulting the answer to challenge n.

1. `ps -aux` <br><br><br><br><br><br><br><br><br><br><br>

1.  `ps | tail -n +2 | wc -l` <br><br><br><br><br><br><br><br><br><br><br>

1.  `ps -aux | tail -n +2 | grep "/usr/bin" | wc -l` <br><br><br><br><br><br><br><br><br><br><br>

1.  `ps -aux | grep "xeyes"` (to find the process id (PID) for xeyes)
    `kill -KILL <PID>` <br><br><br><br><br><br><br><br><br><br><br>

1.  none

1.  `find . -maxdepth 5 -name "passwd" -print` <br><br><br><br><br><br><br><br><br><br><br>

1.  `find . -maxdepth 5 -name "passwd" -print 2> /dev/null` <br><br><br><br><br><br><br><br><br><br><br>

1.  `grep -a "root" /etc/passwd | cut -f6 -d':' > /var/tmp/userhome.txt` <br><br><br><br><br><br><br><br><br><br><br>

1.  `grep -a "myuser" /etc/passwd | cut -f6 -d':' >> /var/tmp/userhome.txt`

