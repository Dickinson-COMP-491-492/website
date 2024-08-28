# Bug/Issue Fixes

## Introduction

In the [Bug Gardening Activity](./A04-BugGardening.md) you became more familiar with your product and project by investigating bugs/issues that appeared in the issue tracker. In this activity you will attempt to fix bugs or address issues that appears in your project's issue tracker.

## Assignment

In this activity you will:
- Identify bug(s)/issue(s) to work on.
- Document your efforts in working on the bugs/issues in three ways:
  - On a "Bugs/Issues Addressed" page on your team's "Project Deliverables" wiki page (described below)
  - In real-time using Slack Live-logs (see [A05-Tech Spikes Activity](./A05-TechSpikes.md)).
  - Weekly using 5-15 reports (described below).
- Give a team presentation of your work.

Additional details on all of these elements are given below.

### Identifying Bugs/Issues

Most larger well-organized H/FOSS projects will have a collection of bugs/issues that have been tagged as "good first issue", "beginner", "introductory", "easy", etc. The developers have identified these as issues that have, in their opinion, a reasonably low barrier to entry and make good places to start. If your project does not have such a list you should search the issue tracker and find a bug that is well specified and seems approachable. If there is an appropriate communication channel for your project, you might also consider asking the community if they have any suggestions for bugs or issues that might be good for a newcomer to the project.

Many communites use specific proceedures for assigning bugs/issues to individuals. Other communities do not assign bugs/issues at all. Be sure to identify how your community handles (or does not) the assignment of issues and follow their proceedures.  In particular, once you identify a bug/issue to work on, be sure to inform the community via the appropriate mechanism (if there is one) that you are working on it. If you ultimately fix the bug, or abandon work on it, again be sure to also inform the community via the appropriate mechanisms.

### Documenting Your Efforts

You will document your efforts and results for this activity in three ways.  Each team will collaboratively maintain a Bugs/Issues Wiki page that provides an overview of the work done by the entire team. You will continue to Live-log your indivial and sub-team work sessions in Slack to provide real-time information about when you have worked and the details of what you have done. Finally, you will write weekly 5-15 reports that summarise what you have accomplished, set goals for future work and reflect on your effectiveness and ways you can improve. 

#### The Bugs/Isssues Addressed Wiki Page

1. Create a link to a new wiki page named "Bugs/Issues Addressed" on your team's "Project Deliverables" page.
2. Give some header information on the new Wiki page that identifies your team and this activity.
3. Create a table on the new Wiki page simialr to the one shown below:


| __Bug ID__ | __Team Members__ | __Description__	| __Confirmed__ | __Actions__ |
|------------|------------------|-----------------|---------------|-------------|
| _The identifier for the bug as an active link into the issue tracker_ | _Initials of team member(s) working on the issue_ | _A short description of the bug_ | _Yes/No/Unknown - does the bug exist in the current development version_ | _Chronological list of each action taken on the bug with dates and active links whenever possible._ |
| [7890](http://example.com/link7890.html) | GB/XY | Withdraw field allows zero amount.	| No. | 11/1/22 - Appears to have already been fixed - [Commented on the ticket suggesting it be closed](http://example.com/7890-close.html). |
| [AB392c](http://example.com/linkAB392c.html) | GB/XY |Program crashes on dates before 1970.	| Yes | 11/2/22 - [Claimed in issue tracker](http://example.com/claimAB392c.html)<br>11/5/22 - [Released in issue tracker](http://example.com/releaseAB392c.html) - Appears to be too complex for our current level of familiarity. |
| [X5432b](http://example.com/linkX5432b.html) | JP/PQ | UI unresponsive when sorting data. | Yes | 11/5/22 - [Assigned to self in issue tracker](http://example.com/claim5432b.html)<br>11/6/22 - [Proposed using Quicksort as a fix](http://example.com/comment5432b.html)<br>11/9/22 - [Made pull request](http://example.com/pr5432b.html)<br>11/11/22 - [Received request for changes on PR](http://example.com/prcomment5432b.html)<br>11/13/22 - [Pushed changes to PR](http://example.com/prupdate5432b.html)<br>11/15/22 - [Pull request merged!](http://example.com/prmerge5432b.html) |

The table should:
- Document every bug/issue that your team attempts to work on, regardless of the final outcome.
- Include a list item for each _significant_ event that occurs when working on the bug/issue.  Significant events would be things such as:
  - Starting work on the issue or claiming the issue.
  - Any communications with the community on the issue tracker or otherwise. These should include live direct links to the communication whenever possible.
  - Completion of work on the bug/issue, regardless of the final outcome.

#### Slack Live-Logs

As with your work on the [A05-Tech Spikes Activity](./A05-TechSpikes.md) you are expected to document your efforst in real-time using Slack Live-logs as you work. You should make Live-log entries during every work session.  These should document what you are doing, things you have tried, communications you have had with your project community (paste links), and resources you have used. Good live logs will reflect an effective, sustained effort of approximately 10 hours per week spread across multiple working sessions.

#### 5-15 Reports

Approximately every week week you will produce a 5-15 report, either as a team or individually. A [five-fifteen report](https://www.contractingbusiness.com/archive/article/20864629/the-fivefifteen-report) is a short weekly templated report that is designed to enhance communication, reflection, prioritization, goal setting and time management without being time consuming. The name five-fifteen reflects that **the report should take no more than five minutes to read and no more than fifteen minutes to write.**

A key quality of good 5-15s is that each successive 5-15 clearly relates back to the prior 5-15s to document progress and identify persistent issues.  Reading your 5-15s should make it make clear how:
- things that were planned turned into actions and eventually accomplishments.
- thoughts on ways to improve individual or team performance were enacted.
- how challenges/roadblocks were addressed and eventually overcome.
- etc.

##### Team 5-15

1. Create a link to a new wiki page named "Team 5-15s" on your team's "Project Deliverables" page.
2. Give some header information on the new Wiki page that identifies your team and indicates that the page contains your 5-15s.
3. Each Team 5-15 must have the headings given below and each must be followed by a few sentences or an annotated list providing the relevant information.
   - **Period Ending:** (mm/dd/yyyy)
   - **Accomplishments:** 
     - List and briefly describe the team's accomplishments since the prior 5-15. Credit should be given to individuals when they have been instrumental in an accomplishment. You should explicitly connect back to goals that were set and challenges that were identified in prior 5-15's.
   - **Team Function:** 
     - Breifly describe how the team is functioning, any challenges it is facting and how the team function might be improved. You should explicitly connect back to challenges and ideas for improvement that were identified in prior 5-15's.
   - **Blockers:**
     - Briefly describe any technical challenges/roadblocks is the team currently facing.
   - **Action Plan:**
     - Identify the items that the team will work on between now and the next 5-15 report. These might include new tasks, things ongoing from prior 5-15s and efforts to address the blockers that have been identified. Specific actions should be proposed and responsibility for them assigned to individuals or sub-teams.

##### Individual 5-15

1. Create a link to a new wiki page named "Individual 5-15s" for yourself on the "Useful Information about Class Members" page (i.e. Where your blog and github are linked).
2. Give some header information on the new Wiki page that identifies you and indicates that the page contains your 5-15s.
3. Each Individual 5-15 must have the headings given below and each must be followed by a few sentences or an annotated list providing the relevant information.
   - **Period Ending:** (mm/dd/yyyy)
   - **Contributions:**
     - Briefly describe what you did individually or collaboratively to contribute to your team's accomplishments since you last individual 5-15. The items you discuss should clearly connect to your team's accomplishements as documented in your Team 5-15s.
   - **Growth:**
     - Briefly describe what you have leared and the ways in which you have improved the way your work, collaborate, support your team, etc... since your last 5-15.  The things that you discuss should generally connect to the goals that you set in your prior 5-15s.
   - **Goals:**
     - Briefly describe what you plan to do, learn, practice, change between now and your next 5-15 to improve your work, knowldge collaboration, teamwork, etc.  Give specific actions that you will take to acomplish your goals.

#### Presentation

Each team will give a presentation of your work on the project.  Your presentation should:
  - Introduce your project assuming that the audience is not familiar with it.  This should include:
    - The mission of the project, what the product does, where it has been used, by whom and for what purposes.
  - Describe / illustrate / demonstrate the bug(s) or issue(s) being addressed.
  - Explain / illustrate / demonstrate what has been accomplished, how it has been done and why it was done that way.  This should include:
    - Relevant communications with the community
    - Code/test implementations
    - Demonstrations 

Prepare this presentation for an audience of your peers (advanced undergraduate computer science majors). You may assume that they know a good bit about computer science and free and open source software. However, you should not assume that they know anything about the specific project your team is working on or the specific technologies that it uses. When discussing topics that are outside of the audience's assumed knowledge, context and background sufficient for the audience to follow the presentation should be provided.

## Grading

The Project Work assignment will be assessed using the rubric below.

_Click rubric to enlarge image._<br>
[![Project Work Rubric. Team Documentation and Effectiveness: 3 pts - On time; Bugs/Issues Addressed Wiki contains all required information; Issues and actions are correctly linked, neatly formatted and easy to read;  List of actions is sufficiently detailed and complete; Team 5-15's are complete, thoughtful, insightful, accurate and provide continuity from one to the next; Writing is clear, concise, well organized and neatly formatted; Clear from 5-15s and instructor observation that the team has been highly effective. 2 pts - On time; Bugs/Issues Addressed Wiki contains all required information; Issues and actions are mostly linked, neatly formatted and easy to read;  List of actions is included; Team 5-15's are complete, but may be perfunctory and may have limited continuity from one to the next;  Writing has minor organizational, conciseness, clarity or formatting issues that do not distract significantly from meaning or understanding; Clear from 5-15s and instructor observation that the team has been effective. 1 pt - On time; Bugs/Issues Addressed Wiki is cursory or missing information; Issues and actions are not linked, are poorly formatted and are not easy to read;  List of actions is insufficient and lacking in detail; Team 5-15's are cursory, missing information and do not provide continuity from one to the next; Writing has organizational, conciseness, clarity or formatting issues that distract significantly from meaning or understanding; Clear from 5-15s and instructor observation that the team has not been operating effectively. 0 pts - Late, missing or substantially incomplete; Clear from 5-15s and instructor observation that the team has made little to no investment in the assignment. Individual Documentation and Effectiveness: 3 pts - On time; Individual 5-15's are complete, thoughtful, insightful, accurate and provide continuity from one to the next; Individual's contributions to Live-Logs are detailed and clearly demonstrate sufficient, regular and sustained time and effort; Writing is clear, concise, well organized and neatly formatted; Clear from 5-15s, Live-Logs and instructor observation that individual has been responsible and highly effective individually and essential as a team member. 2 pts - On time; Individual 5-15's are complete, but may be perfunctory and may have limited continuity from one to the next; Individual's contributions to Live-Logs demonstrate investment of time and effort. Writing has minor organizational, conciseness, clarity or formatting issues that do not distract significantly from meaning or understanding; Clear from 5-15s, Live-Logs and instructor observation that individual has been responsible and active individually and has participated as a team member. 1 pt - On time; Individual 5-15's are cursory, missing information and do not provide continuity from one to the next; Individual's contributions (or lack there of) to Live-Logs demonstrate insufficient investment of time and effort; Writing has organizational, conciseness, clarity or formatting issues that distract significantly from meaning or understanding; Clear from 5-15s, Live-Logs and instructor observation that individual has lacked responsibility, has been inactive individually and/or has not participated as a team member. 0 pts - Late, missing or substantially incomplete; Clear from 5-15s and instructor observation that individual has made little to no investment in the assignment. Presentation: 3 pts - Presentation was interesting, engaging and told a cohesive story;  All required information was clearly presented in a well organized and easy to follow manner; Language, terminology and explanations were appropriate to the target audience; Use of media (slides, etc.) was visually appealing and enhanced the presentation; Demonstrations were used effectively; Presentation provided clear and compelling evidence of appropriate and effective work on the project including community engagement; Participation was well balanced across team members;  Presentation was at the target length. 2 pts - Presentation was generally well organized and included all required information; Language, terminology and explanations were generally appropriate to the target audience; Use of media effectively supported the presentation; Demonstrations were included; Presentation provided evidence of work on the project including community engagement; Participation by individual team member was mildly unbalanced (more or less) as compared to others;  Presentation was  moderately shorter or longer than the target length. 1 pt - Presentation was difficult to follow and/or was missing some required information; Language, terminology and explanations missed the target audience at numerous points; Use of media was ineffective or distracting; Demonstrations were ineffective;  Presentation provided insufficient evidence of work on the project and a lack of community engagement; Participation by individual team member was moderately to heavily unbalanced (more or less) as compared to others;  Presentation was  significantly shorter or longer than the target length. 0 pts - Presentation was substantially incomplete; Clearly demonstrates little to no investment in the assignment; Individual team member did not participate.](images/BugFix-Rubric.jpg)](images/BugFix-Rubric.jpg)

---

![Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png "Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License") All textual materials used in this course are licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/)

![GPL V3 or Later](https://www.gnu.org/graphics/gplv3-or-later-sm.png "GPL V3 or later") All executable code used in this course is licensed under the [GNU General Public License Version 3 or later](https://www.gnu.org/licenses/gpl.txt)
