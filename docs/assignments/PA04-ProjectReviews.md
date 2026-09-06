## PA04 - Project Reviews

### Introduction

In the [Project Exploration assignment](PA03-ProjectExplorations.md) you collected basic information about some projects to which you might be interested in contributing. In this assignment you will build on that background by gathering more in depth and detailed information about a few of the projects that you are most interested in. This will include assessing how welcoming a community is to newcomers, how responsive they are to questions, how well documented and organized the project is, and thinking about what you'll need to learn to get started. Collecting this additional information will take some time and effort, but it will be very helpful in making a well informed decision in the next activity, which asks you (and your teammates) to select the project community with which you will work for the remainder of the year.  You should plan to spend approximately 3 hours on each Project Review.

### Assignment

In this assignment you will complete an H/FOSS Project Review for at least 2 H/FOSS projects of interest. Ideally, your project reviews will build upon your project explorations. However, they may also be projects that were explored by others (see the [Course Repo](https://github.com/Dickinson-COMP-491-492/AY26-27)) or they could include a newly discovered project. If you elect to review a project that you did not explore, you will need to complete a [Project Exploration](PA03-ProjectExplorations.md) for the new project before completing a Project Review for it.

#### Setup

Before starting your project reviews:

1. Synchronize the `main` branch of your course repo with the upstream.
2. Create a new feature branch from `main` for your project reviews.
3. Switch to your new feature branch.

#### Project Reviews

Complete your project reviews by:
1. Select at least 2 projects to review that seem most promising to you.
   - If you select a project that you did not explore in the previous assignment, complete a [Project Exploration](PA03-ProjectExplorations.md) for the project before continuing.
2. Open the `.md` file in your directory for the Project Exploration that you did for the project that you are now reviewing.
3. Add a top level heading for the "Project Review" below the Project Exploration.
4. Add a second level heading for each of the following topics and add content to the sections as described.

   - **Standard Documentation:** Most open source projects will provide a collection of standard documentation. These standard documents lay out the project's policies and help to orient new contributors to the project. Reviewing these documents will give you a sense of how well the project is documented, how the community governs itself and the thought that they have put into how newcomers join project.
     - In this section **rate the project's standard documentation from your perspective as excellent, good, adequate, poor, or terrible and explain your reasoning in some detail.** 
     - To develop your rating and reasoning:
       - Look for documentation of the following:
         - A project introduction giving an overview of the project and where to find other resources. This documentation is often in a `README` file, but may appear in other locations as well.
         - The project's license(s) indicating the conditions and obligations for use of the product. This documentation is often in a `LICENSE` file, but may appear in other locations as well.
         - A contributing guide describing ways to contribute to the project and laying out the process of making contributions (i.e. a workflow). This documentation is often in a `CONTRIBUTING` file, but may appear in other locations as well.
         - An installation guide that gives instructions for how to setup the development environment and install the product. This documentation is often in an `INSTALL` file, but may appear in other locations as well.
         - A code of conduct that establishes expectations for how community members will behave and interact and the sanctions for violations of those expectations.  This documentation is often in a `CODE_OF_CONDUCT` file, but may appear in other locations as well.
         - An AI use policy indicating how AI tools may and may not be use and establishing expectations and mechanisms for the disclosure of AI use. This documentation is often in an `AI_POLICY` file, but may appear in other locations as well.
         - Any other documentation that you find that looks particularly useful to newcomers to the project.
       - Read enough of each of the documents to be able to assess things including:
         - your ability to make reasonable sense of the contents.
         - the acceptability of the licensing, code of conduct, and AI use policies.
         - the clarity and level of detail, particularly in the install and contributing documents.

   - **Communication Channels:** Most projects will have several communication channels (e.g. IRC/Gitter/Slack/Discord/Mailing List/Forums/etc.), with each serving a different purpose for the community (team meetings, Q and A, knowledge base, live help, user forums, developer chat, community building, etc., etc.). Reviewing the communications channels will give you an idea of what it would be like to try to ask questions or engage in discussion with the community. (Note that while Pull Requests and the Issue Tracker are also communication channels they will be addressed separately, so you should not include them here.)
     - In this section **rate the project communications from your perspective as excellent, good, adequate, poor, or terrible and explain your reasoning in some detail.**
     - To develop your rating and reasoning:
       - Identify the main channels that are used by the project.
       - Read enough content on each channel to get a feel for its use and purpose.
       - Some things you should pay particular attention to include:
         - the tone of communications.
         - whether the discourse is at an approachable level.
         - the frequency and currency of messages.
         - whether questions that are posted are answered in a helpful and timely manner.
         - any communications specifically with students or other newcomers.
  
   - **Issues:** Most projects will use an issue tracker to report, organize and track tasks, bugs and feature requests. Reviewing the issue tracker will give you an idea of the types of issues that the project is currently working on, the availability of approachable issues and what it will be like to work on bugs/features within the project. 
     - In this section **rate the project issue tracker from your perspective as excellent, good, adequate, poor, or terrible and explain your reasoning in some detail.**
     - To develop your rating and reasoning:
       - Find the issue tracker that is used by the project.
       - Read enough issues (open and closed) to get a feel for the types of tasks, bugs, and feature request that exist in the project.
       - Using the issue tracker's sort and filter features can be very helpful.
       - Some things you should pay particular attention to include:
         - issues with labels indicating that they are good for newcomers (e.g. "Good first issue", etc.).
         - the approachability of the open issues.
         - the number of open issues there are.
         - the rate at which new issues are being added.
         - the responsiveness and helpfulness of conversations in the issue comments.
         - the typical time from when an issue is created to when it is assigned to when it is closed.

   - **Pull Requests:** Most projects will use pull requests (a.k.a. merge requests) to accept code contributions. Reviewing the project's pull requests will give you an idea of how contributions are received are handled by the community and what the process of making a contribution might be like. 
     - In this section **rate the project's pull requests from your perspective as excellent, good, adequate, poor, or terrible and explain your reasoning in some detail.**
     - To develop your rating and reasoning:
       - Find the pull requests for the project.
       - Read enough pull requests (open and closed) to get a feel for what it requires to open, refine and get a pull request merged.
       - Using the sort and filter features for pull requests can be very helpful.
       - Some things you should pay particular attention to include:
         - pull requests linked to issues with labels indicating that they are good for newcomers (e.g. "Good first issue", etc.).
         - the number of open pull requests there are.
         - the responsiveness and helpfulness of conversations in the pull request comments.
         - the typical time from when recent pull requests were opened until they were merged.

   - **Contributors:** Most active projects will have from a few to dozens of contributors and possibly hundreds if everyone who has come and gone over a number of years is counted. Reviewing the contributors for a project will give a sense of who the key contributors are and how open the project is to new contributors.
     - In this section **identify the key recent contributors to the project and assess whether the project has accepted recent contributions from newcomers..**
     - To develop your description:
       - Find the information about the contributors (GitHub & GitLab make this pretty accessible. If you are on another platform you may have to look at the actual commits via `git log` or whatever GUI means the repository hosting platform provides).
       - Some things you should pay particular attention to include:
         - the total number of contributors.
         - the most prolific contributors.
         - the number of different contributors in the last year or so.
         - the number of first time contributors in the last year or so.
         - whether contributors tend to come and go over time.

   - **Technical Stack:** Every project will have a technical stack including the languages, frameworks and tooling that they use for development. In addition, the computational needs for running different projects can vary widely. Reviewing the technical stack will help to assess more fully asses the match between the project and your skill set, your learning goals, and your access to computational resources.
     - In this section **rate the projects technical stack from your perspective as excellent, good, adequate, poor, or terrible and explain your reasoning in some detail.**
     - To develop your rating and reasoning:
       - find as much information as you can about the project's tech stack. (You will need to dig deeper than the "Languages" box on the repository page on GitHub or GitLab.)
       - Some things you should pay particular attention to include:
         - the programming language(s) used for implementation.
         - frameworks or libraries used for implementation.
         - frameworks or libraries used for testing.
         - package managers and build tools. 
         - any other tooling that the project uses.
         - any specific computational demands (GPU's, RAM, etc.) that the project requires.

   - **Overall Assessment**: Give an overall assessment of the project based on what you have found in your review.  Be sure to comment on why you are more (or less) interested in the project, what you believe would facilitate or make it difficult to contribute to this project, and any concerns you would have about joining this project. Reference findings from the other sections to support your assessment.

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
