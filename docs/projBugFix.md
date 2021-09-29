# Bug Fix Activity

## Introduction
In the [Bug Gardening Activity](projBugGardening.md) you became more familiar with your product and project by investigating issues that appeared in the issue tracker. In this activity you will attempt to fix a bug that appears in the issue tracker.

Many larger well-organized H/FOSS projects will have a collection of bugs/issues that have been tagged as "beginner", "introductory", "easy", etc. The developers have identified these as issues that have, in their opinion, a reasonably low barrier to entry and make good places to start. If your project does not have such a list you should search the issue tracker and find a bug that is well specified and seems approachable. If there is an appropriate communication channel for your project, you might also consider asking the community if they have any suggestions for bugs that might be good for a newcomer to the project. However you identify bugs to work on, be sure to inform the community via the appropriate mechanism that you are working on the bug. If you ultimately fix the bug, or abandon work on it, be sure to also inform the community via the appropriate mechanisms.

## Assignment

For this activity each sub-group will identify at least one active bug in the issue tracker and attempt to fix it. Sub-teams are expected to work on this part of the activity for a minimum of two weeks. Work on this activity may require side tracks to learn more about the project, to complete additional tutorials, to discuss the issue with the community, etc. If a bug is identified and fixed in less than two weeks time, sub-teams should select additional bugs to work on.

Track and document what you do using your sub-team's Slack live-log. Work on the activities will be assessed via the Project Checkpoints as described in the [Course Syllabus](syllabus.md). When your sub-team believes it has satisfied the Completion Criteria, schedule an appointment with the course faculty for review.

All of the bugs that the team has attempted to fix must be collected together and documented under the heading "Attempted Bug Fixes" on your team's Bug Activities Wiki page. This section of the Wiki page should include a table with one row for each attempted bug. The information in this table should be brief, full details are of course contained in your Slack live-logs. The table below shows the required columns and a few sample rows:

| __Bug ID__ | __Sub-Team__ | __Description__	| __Confirmed__ | __Result__ |
|------------|--------------|-----------------|---------------|------------|
| _The identifier for the bug as a link into the issue tracker_ | _Initials of sub-team members_ | _A short description of the bug_ | _Yes/No/Unknown - does the bug exist in the current development version._ | _Description of any action taken on the bug. Include links to any artifacts that document your actions._ |
| [7890](http://example.com/link7890.html) | GB/XY | Withdraw field allows zero amount.	| No. | Appears to have already been fixed. Commented on the ticket suggesting it be closed. |
| [AB392c](http://example.com/linkAB392c.html) | GB/XY |Program crashes on dates before 1970.	| Yes | Claimed in issue tracker. Abandoned and released in issue tracker. After a few hours, this appears to be too complex for our current level of familiarity. |
| [X5432b](http://example.com/linkX5432b.html) | JP/PQ | UI unresponsive when sorting data. | Yes | Assigned to self in issue tracker. Recoded using Quicksort instead of Bubble Sort. Issued a pull request. Pull request was merged! |

It is important to document all of the bugs that you attempt to work on, regardless of the outcome. This will ensure that all sub-teams can learn from each other and do not duplicate work.

## Completion Criteria

The completion criteria that each sub-team must demonstrate for this activity are:

The team's Bug Activities wiki page must be updated to include the following sections and information:
- __Attempted Bug Fixes:__ The table of information about the bugs that the team attempted to fix as described above. Links in this table that qualify as Interactions or Contributions should also be linked in the sub-sections below. Yes, this is repeated information, but the separate organization is helpful to your instructor.
- __Interactions:__ Add to the annotated list, with links if possible, any interactions that your team or sub-team had with the community during this activity (e.g. message board posts, mailing list messages, comments in the issue tracker, etc.). Please indicate the date of the interaction and the sub-team that had the interaction. Note: Interactions are not required for this activity. However if they occur, please link them here for reference.
- __Contributions:__ Add to the annotated list, with links if possible, any contributions that your team or sub-team made to the project during this activity (e.g. corrections/clarifications/additions to documentation, closed issues, merged pull requests, etc.). Please indicate the date of the contribution and the sub-team that made the contribution. Note: Contributions are not required for this activity. However if you discover interesting information about a bug or fix the bug, you are highly encouraged to contribute what you find back to the community. Further, any accepted bug fix will guarantee an automatic exceptional (3) rating in the Effectiveness category on the Project Checkpoint rubric.

Each team member must be able to:
- Participate competently in a discussion of bug fixes that were attempted.
- Show and competently discuss the issue ticket for the bug that was fixed.
- Walk through a demonstration of the bug before the fix was completed (use git to checkout an older commit or use snapshots).
- Competently discuss what was done to fix the bug and test that it was fixed. This will include showing the modifications made to the code.
- Demonstrate how it is known that the bug was fixed including running the product and the test suite(s).
- Show the steps that have been taken to contribute the bug fix back to the community.

---

Acknowledgements: This assignment builds from and adapts ideas and content from the following activities created by others:
- http://foss2serve.org/index.php/Bug_Gardening
- http://foss2serve.org/index.php/Bug_Selection
- http://foss2serve.org/index.php/Research_Bug_Activity
- http://foss2serve.org/index.php/Solving_A_Bug
- http://foss2serve.org/index.php/Writing_a_bug_report
