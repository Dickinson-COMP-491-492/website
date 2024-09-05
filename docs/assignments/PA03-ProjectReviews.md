## PA03 - Project Reviews

### Introduction

In the [Project Exploration assignment](PA02-ProjectExplorations.md) you collected basic information about some projects to which you might be interested in contributing. In this assignment you will build on that background by gathering more in depth and detailed information about a few of the projects that you are most interested in. This will include assessing how welcoming a community is to newcomers, how responsive they are to questions, how well documented and organized the project is, and thinking about what you'll need to learn to get started. Collecting this additional information will take some time and effort, but it will be very helpful in making a well informed decision in the next activity, which asks you (and your teammates) to select the project community with which you will work for the remainder of the year.  You should plan to spend approximately 3 hours on each Project Review.

### Assignment

Students pursuing a FOSS Project must complete an H/FOSS Project Review for 2 H/FOSS projects of interest. Students pursuing Research/Honors Projects must complete the an H/FOSS Review for 1 H/FOSS project. Ideally, your project reviews will build upon your project explorations. However, they may also be projects that were explored by others (see the [Course Repo](https://github.com/Dickinson-COMP-491-492/AY24-25)) or they could include a newly discovered project. If you elect to review a project that you did not explore, you will need to complete a [Project Exploration](PA02-ProjectExplorations.md) for the new project before completing a Project Review for it.

Before starting your project reviews:
1. Synchronize the `main` branch of your course repo with the upstream.
2. Create a new feature branch from `main` for your project reviews.
3. Switch to your new feature branch.

#### Project Reviews

Complete your project reviews by:
1. Select 2 projects to review (1 for students doing an individual research or honors project) that seem most promising to you.
   - If you select a project that you did not explore in the previous assignment, complete a [Project Exploration](PA02-ProjectExplorations.md) for the project before continuing.
2. Open the `.md` file in your directory for the Project Exploration that you did for the project that you are now reviewing.
3. Add the following sections and content to the `.md` file below the Project Exploration:
   - **Project Review:** Add top level section heading at the bottom of the document with the text "Project Review".

   - **Getting Started:** In this section you will explore what resources are available to new developers looking to join the community. It will give you an idea of what it might be like if you decide to work on this project.  Be sure to look at the project's web site, its repositories and any other sources they provide.
     - **Documents:** Identify and give a link to any document that is particularly relevant to newcomers to the project (e.g. installation, getting started, how to contribute, newcomer threads in communication channels, etc.). Skim each one fairly quickly and give your assessment of it as very clear, clear, confusing, or useless.
     - **Code of Conduct:** Give a link to the project's code of conduct, if it has published one. If there is a code of conduct, review it and give your thoughts on working in a project where conduct is governed by this code.
     - **User Installation:** Give a link (or links) to the information that a user would need in order to install or use the project's product. This may be a set of instructions for building the application from source, it may be a page that provides downloads of the executable program, or it may be a live demo site that can be accessed on line. Briefly skim this information and give your assessment of how difficult it would be to become a user of the product as impossible, difficult, reasonable, easy, trivial.  Give a short justification for your assessment.
     - **Developer Installation:** Give a link (or links) to the information that a new developer would need in order to get setup to begin working on the project. This will typically be a set of instructions for setting up a development environment and will often be contained within the project's organization or repository. Note that occasionally projects will reorganize and/or move between repository hosting sites (GitHub, GitLab, SourceForge, etc.). So, be sure that you are considering the most current repository or organization. Briefly skim this information and give your assessment of how difficult it would be to setup the development environment for the project as impossible, difficult, reasonable, easy, trivial.  Give a short justification for your assessment.
     - **Organization:** Give an overall assessment of the organization of the project. Some things to consider when making your assessment include:
       - Were the documents you found easy to find?
       - Was it clear which documents would be useful to you? 
       - Is the amount of information helpful without being overwhelming? 
       - Is there out of date or redundant information that may be confusing?
     - **Summary:** Based on your review, summarize your overall thoughts on what you think it would be like to get started working on this project. Some things to consider include: Does the documentation suggest that the project is welcoming to newcomers? Do you think you will be able to find the information need? Is the documentation written at a level that you can understand?

   - **Community Communication:** In this section you will explore how active and responsive the project community is. It will give you an idea of what it would be like to try to ask questions or engage in discussion with the community.

     Most projects will have several communication channels (e.g. IRC/Gitter/Slack/Discord/Mailing List/Forums/etc.), with each serving a different purpose for the community (team meetings, Q and A, knowledge base, live help, user forums, developer chat, community building, etc., etc.). Identify the main channels that are used by this project. Note that while Pull Requests and the Issue Tracker are communication channels they will be addressed separately, so you should not include them here. 
     
     - For each of the communication channels that you identify, include the following information:
       - **Channel:** Give the name of and a link to the main page for the communication channel.
       - **Purpose:** Each communication channel will have a different purpose. Describe as best you can how the community uses this particular communication channel. Note that the channel may not tell you its purpose, you may need to read other project documentation or some of the channel messages to figure this out. 
       - **Currency:** Give the date of the most recent information added to this channel.
       - **Activity:** Give estimates for how many new messages have been posted in the last day, week or month. Briefly describe how you made your estimate.
       - **Responsiveness:** Review the recent communications in the channel and categorize the chances of receiving a response to a message as: very likely, probably, maybe, or never. Briefly describe why you chose the category that you did.
       - **Response Time:** Indicate the shortest amount of time that it took for a recent message to get a response. Give a rough estimate of the typical amount of time it has taken for recent messages to get a response. 
       - **Members:** List a few the community members that are most active on this channel (nicknames or handles are fine).
       - **Tone:** Give your assessment of the tone of the communications on this channel. For example, do  you find it welcoming, informal, formal, rude, terse, highly technical, helpful, etc.?  Give a brief justification for your assessment. If you have a particularly strong impression of the channel, you might include a few quotes to support your assessment.
     - **Summary:** Based on your review of the individual communication channels, summarize your overall thoughts on how you feel about communicating with this community. Some things to consider include: Are the communication's channels active? Are questions like those you might imagine asking getting answers quickly? Do the comminations seem welcoming and helpful?

  - **Repositories:** In this section you will explore the project's repositories in detail to get a better idea of how active the project is and how open it is to contributions from newcomers. 

    Many projects are contained within a single repository, but others may have 10's or even 100's of repositories. If your project has multiple repositories briefly review them and select 3-5 that seem the most interesting to you.

    - Include the following information for each repository that you identify. 
      - **Repository:** Give a link to the repository.
      - **Purpose:** Briefly describe the role or purpose of the repository within the project.
      - **Origins:** Give the date on which the repository was created.
      - **Last Commit:** Give the date on which the last commit was made to this repository.
      - **License:** Indicate the open source license(s) that apply to the code in the repository.

  - **Issue Tracking:** In this section you will explore how issues in this project are reported/tracked/discussed by the community. It will give you an idea of the types of issues that the project is currently working on and what it will be like to work on bugs/features within the project. Note: Using the issue tracker's sort and filter features will be helpful.
    - **Issue Tracker:** Give a link to the repository's issue tracker.
    - **Volume:** Give the number of open issues are currently in the issue tracker.
    - **Currency:** Estimate the number of open issues that were created over the following time frames: the last week, the last month, the last 6 months, the last year.  For very active projects feel free to use "too many to count" for the last 6 months and/or the last year if appropriate.
    - **Activity:** Estimate of the number of open issues that have had comments added to them over the following time frames: the last week, the last month, the last 6 months, the last year. Note: Most issue trackers will allow you to sort by the date of the last activity. For very active repositories feel free to use "too many to count" for the last month, last 6 months and/or the last year if appropriate.
    - **Beginner Issues:** Most issue trackers allow issues to be tagged/labeled. Projects that are particularly interested in helping new contributors join the project will use tags/labels to indicate issues that would be good for new developers (e.g. "Good first issue", "Easy", "Good second issue"). 
      - **Labels:** List any labels that the project uses to indicate issues that may be a good place to start.
      - **Volume:** Give the number of currently open issues that are tagged/labeled in this way.
      - **Currency:** Estimate the number of currently open issues tagged/labeled in this way that were opened over the following time frames: the last week, the last month, the last 6 months, the last year.
      - **Resolution:** Estimate the number of issues tagged/labeled in this way that have been closed by a pull/merge request over the following time frames: the last week, the last month, the last 6 months, the last year.
      - **Approachability:** Read a few of these issues and the comments and discussion associated with them. Give your assessment of whether you think that these issues would be something that you believe you could work on once you have a little experience with the project. Consider whether they are clearly written, include enough information to get started, have received helpful comments, etc. If you have a particularly strong impression of these issues, you might include a few quotes to support your assessment.
    - **Summary:** Based on your review, summarize your overall thoughts on what it would be like interacting with this project's issue tracker. Some things to consider include: Are there good beginner issues? Are you able to generally understand the good beginner issues? Are comments on issues receiving helpful feedback?
    
  - **Pull/Merge Requests:** In this section  you will explore how contributions that are received are handled by the project. It will give you an idea of how contributions are treated by the community and what the process of making a contribution might be like. Note: Using the sort and filter features for pull/merge requests will be helpful.
    - **Volume:** Give the number of open pull/merge requests in the project.
    - **Currency:** Estimate the number pull requests (both open and closed) that were created over the following time frames: the last week, the last month, the last 6 months, the last year.  For very active projects feel free to use "too many to count" for the last 6 months and/or the last year if appropriate.
    - **Activity:** Estimate of the number of pull requests (both open and closed) that have been updated (e.g. had commits or comments added to them) over the following time frames: the last week, the last month, the last 6 months, the last year. For very active repositories feel free to use "too many to count" for the last month, last 6 months and/or the last year if appropriate.
    - **Resolution:** Estimate the number of pull requests that have been merged into the project over the following time frames: the last week, the last month, the last 6 months, the last year.  For very active projects you can use "too many to count" for the last 6 months and/or the last year if appropriate.
    - **Contributors:** Estimate how many different people have contributed to this repository over the following time frames: the last month, the last year.
    - **New Contributors:** Estimate how many different people have made their first contribution to this repository over the following time frames: the last month, the last year.
    - **Top Contributors:** List the top 3-5 contributors to this repository and the number of commits each has made in the last year.
    - **Summary:** Based on your review, summarize your overall thoughts on what it might be like to try to contribute to this project. Some things to consider include: Is the project being actively worked on by contributors and managed by maintainers? Are things happing too fast or too slow? Are newcomers being successful in making contributions?

  - **Tools/Languages/Libraries/Frameworks:** In this section you will look at the project specific tools, programming languages, libraries and/or frameworks that are used by the project. This will give you an idea of how well the project is matched to your current skills, the skills you would like to learn and how much you will need to learn. You may need to use the project's web page, repositories, communication channels, etc. to find the information requested in this section.
    - **Tools:** List the specialized tools are used to run, create, build the project (e.g. docker, linters, formatters, maven, npm, node, etc.)?  For each tool, indicate your familiarity with it as expert, used it, heard of it, unfamiliar.
    - **Languages:** List the the main languages used in the project and give the approximate percentage of the code that is in each language.  For each language, indicate your familiarity with it as expert, used it, heard of it, unfamiliar.
    - **Application Libraries/Frameworks:** List any libraries and/or frameworks are used in the main project code (e.g. React, Spring, Django, Flask, Express, Bootstrap, etc.). For each library or framework, indicate your familiarity with it as expert, used it, heard of it, unfamiliar.
    - **Testing Libraries/Frameworks:** List any libraries and/or frameworks are used for testing in the project (e.g. JUnit, PyUnit, Jest, Mocha, Cypress, etc.). For each library or framework, indicate your familiarity with it as expert, used it, heard of it, unfamiliar.
    - **Summary:** Based on your review, summarize your overall thoughts about working with the tools, languages, libraries and frameworks used by the project. Some things to consider include: How much of the project technology are you already familiar with? How much new technology will you need to learn? Are you excited about and interested in learning them? How hard do you think they will be to learn? 

  - **Assessment**: Give an overall assessment of the project based on your review.  Be sure to comment on why you are more (or less) interested in the project, what you believe would facilitate or make it difficult to contribute to this project, and what concerns you have about joining this project.

### Acknowledgements

This assignment builds from and adapts ideas and content from the following activities created by others:

* https://github.com/ChrisMurphyOnline/open-source-software-development-course/blob/master/activities/foss-evaluation-activity.txt
* http://foss2serve.org/index.php/Intro_to_FOSS_Project_Anatomy_(Activity)
* http://foss2serve.org/index.php/FOSS_Field_Trip_(Activity)
* http://foss2serve.org/index.php/Project_Evaluation_Activity_V2
* https://github.com/ChrisMurphyOnline/open-source-software-development-course/blob/master/activities/foss-get-involved.txt

---

![Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png "Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License") All textual materials used in this course are licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/)

![GPL V3 or Later](https://www.gnu.org/graphics/gplv3-or-later-sm.png "GPL V3 or later") All executable code used in this course is licensed under the [GNU General Public License Version 3 or later](https://www.gnu.org/licenses/gpl.txt)
