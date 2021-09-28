# Bug Gardening Activity

## Introduction
In the [User Install](projUserInstall.md) and [Developer Install](projDevInstall.md) Activities you became familiar with your project from the user, developer and documentation contributor perspectives. In this activity you will become more familiar with the project as a software tester and developer by investigating bugs.

## Assignment

In this activity you will:
- Develop an understanding of your project's process for dealing with bugs/issues (Bug Information);
- Investigate bug/issue tickets to help with the maintenance of your project's bug/issue tracker (Bug Gardening);

Track and document what you do using your sub-team's Slack live-log. Work on the activities will be assessed via the Project Checkpoints as described in the [Course Syllabus](syllabus.md). When your sub-team believes it has satisfied the Completion Criteria, schedule an appointment with the course faculty for review.

## Getting Started:

For this activity there will be a number of deliverables that will be collectively produced by the project team / sub-teams and posted to the team Wiki page (See the Completion Criteria below) So before going further, ensure that a link for a new Wiki page for the Bug Activities has been added to your team's Wiki page. The project sub-teams will each be adding to this new Wiki page throughout this activity. It is the full team's responsibility to keep this new Wiki page well organized and nicely formatted.

# Bug Information:

Every H/FOSS project worth its salt will have a bug/issue tracker. In addition to that many projects also have resources (documents/communication channels/etc) that describe the processes and expectations for reporting/triaging/fixing bugs or provide ways to discuss bugs.

Find and read all of the bug-related resources that your project provides. Under a heading of "Bug Resources" on your team's Bug Activities Wiki page create, collectively as a team, an annotated list of the useful bug-related resources that you found. Be sure to include the bug/issue tracker itself, information about how developers claim bugs on which they plan to work, and how bug fixes are contributed back to the project. This list should be a one-stop shop for all of the information you need about dealing with bugs in your project. Entries in the list should be of the form:

- [Title as Link to Resource]: Short description of the resource and how it may be useful.

Finally, before continuing read Simon Tatham's article on [How to Report Bugs Effectively](http://www.chiark.greenend.org.uk/~sgtatham/bugs.html).

## Bug Gardening:

Bug gardening is a name often given to the task of maintaining the bug/issue tracker in a project. This will include things such as assigning tags and/or priorities to tickets, confirming the existence of reported bugs, requesting additional information on submitted tickets, adding useful information to existing tickets, eliminating duplicate tickets, connecting potentially related tickets, closing completed or out of date tickets, etc. In this part of the activity you will try to help your project by doing some bug gardening.

Each sub-team should investigate the existence of at least 3 suspect bugs in the bug/issue tracker for your project. The bugs investigated by each sub-team should be different from those of the other sub-groups. A suspect bug is one that has not been closed but that may not actually exist in the current development version of the product. Suspect bugs can arise in a variety of ways. Someone may simply have forgotten to close the ticket, Someone may have re-discovered and fixed this bug while working on another ticket or the relevant features may have been eliminated from the product. To identify suspect tickets, you might look at old tickets, tickets with version numbers that do not match the current version, and older tickets marked as low priority. Any information that you were able to identify earlier about how the project handles/processes bugs may also help in finding suspect bugs (e.g. if the project uses an in-progress tag for tickets undergoing active work, a ticket tagged in-progress but that hasn't been updated in a long time might be suspect). The best suspect bugs to investigate will the those with a detailed list of steps for replicating the bug. If you have trouble identifying suspect bugs, you might explain (briefly) to the community what you are doing. They may then have suggestions for how to identify suspect bugs in the project or suggestions for other related things you might do to help maintain the issue tracker. If the community has other suggestions, please discuss them with the course faculty to possibly arrange alternative completion criterion as appropriate.

All of the suspect bugs investigated by the full project team should collected together and documented under the heading "Suspect Bugs" on your team's Bug Activities Wiki page. This section of the Wiki page should include a table with one row for each suspect bug. The information in this table should be brief, full details will be contained in your Slack live-logs. The table below shows the required columns, gives a short explanation of each column and a few sample rows:


| __Bug ID__	| __Sub-Team__ | __Description__ | __Why Suspect__ | __Exists__	| __Actions__ |
|-------------|--------------|-----------------|---------------------|-------------|-------------|
| _The identifier for the bug as a link into the issue tracker_ | _Initials of sub-team members_ | _A short description of the bug_ | _A short explanation of why the bug suspect_ | _Yes if able to confirm existence of the bug in the latest dev version, No if able to confirm it does not exist. Uncertain, if neither yes or no. Along with brief comments._ | _Description of any action taken on the bug. Include links to any artifacts that document your actions._ |
| [1234] | GB/XY| Deposit field allows negative amounts. |	Ticket dated 2008, latest version released 2016. |	No. | Followed steps in ticket to reproduce and negative amount was rejected. |	Commented on the ticket suggesting it be closed. |
| [X5432b] | 	GB/XY	| UI unresponsive when sorting data.	| Ticket posted for version 1.3, latest product version is 2.7.	| Yes. | Confirmed unresponsiveness when sorting the very large test data set.	| Commented on the ticket indicating problem was seen in Version 2.7 using the large test data set, but was not noticeable with the small test data set. |
[AB392c] | JM/PQ | Program crashes on dates before 1970.	| Ticket posted for version 1.3, latest product version is 2.7.	| Uncertain. | Unable to replicate bug because steps for replication were incomplete/unclear with regard to version 2.7. | Commented on the ticket explaining source of confusion and asking for clarification. |

If a sub-team happens to identify a new bug that does not already appear in the issue tracker they may open a new ticket for the bug in lieu of one of the suspect bug reports. The corresponding row in the table above should link to and describe their new issue ticket.

## Completion Criteria

The completion criteria that each sub-team must demonstrate for this activity are:
- A link on the team wiki to a Bug Activities page.
- A single, nicely formatted Bug Activities page built collaboratively by all sub-teams on the project. This page must include the following sections and information:
  - __Bug Resources:__ An annotated list of all of the bug related resources for the project.
  - __Suspect Bugs:__ The table of suspect bugs that were investigated along with the actions that were taken as described above. Links in this table that qualify as Interactions or Contributions should also be linked in the sub-sections below. Yes, this is repeated information, but the separate organization is helpful to your instructor.
  - __Interactions:__ An annotated list, with links if possible, of any interactions that your team or sub-team had with the community during this activity (e.g. message board posts, mailing list messages, comments/clarifications on issues, etc.). Please indicate the date of the interaction and the sub-team that had the interaction. Note: Interactions are not required for this activity. However if they occur, please link them here for reference.
  - __Contributions:__ An annotated list, with links if possible, of any contributions that your team or sub-team made to the project during this activity (e.g. corrections/clarifications/additions to documentation, closed issues, etc.). Please indicate the date of the contribution and the sub-team that made the contribution. Note: Contributions are not required for this activity. However if you discover interesting information about a bug, you are highly encouraged to contribute what you find back to the community. If you do comment on an issue ticket, please include the link here for reference.

Each team member must be able to:
- Participate competently in a discussion of the bug resources for the project.
- Show and competently discuss the issue ticket for one suspect bug (e.g. What is the issue? Why is it suspect?) Each sub-team member must select a different suspect bug.
- Walk through a demonstration of what was done to investigate the suspect bugs.
- Competently discuss the actions that were taken and show any artifacts (i.e. interactions or contributions) related to the actions.

---

Acknowledgements: This assignment builds from and adapts ideas and content from the following activities created by others:
- http://foss2serve.org/index.php/Bug_Gardening
- http://foss2serve.org/index.php/Bug_Selection
- http://foss2serve.org/index.php/Research_Bug_Activity
- http://foss2serve.org/index.php/Solving_A_Bug
- http://foss2serve.org/index.php/Writing_a_bug_report
