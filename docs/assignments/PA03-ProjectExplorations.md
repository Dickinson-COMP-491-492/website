## PA03: Project Explorations

### Introduction

In the [Candidate Projects assignment](./PA02-CandidateProjects.md) you identified a collection of projects that you were interested in and that were at least minimally suitable (i.e. are active, have a license, and have basic documentation). In this assignment you will explore a subset of those projects more deeply to get a better feel for what it might be like to work on them. 

### Recommended Background Reading

Before beginning it is recommended that you read [What you actually need to know about open source to get started](https://opensource.com/article/22/11/get-started-open-source) and [Open-Source Contribution: The Ultimate Guide](https://builtin.com/software-engineering-perspectives/open-source-contribution) to get a feel for the kinds of things you'll want to be thinking about as you explore your candidate projects more deeply in this assignment.

#### Project Explorations

1. Synchronize your course repo with the upstream.
   1. Ensure that you are on the `main` branch. 
   2. Set the upstream remote of your clone to point to the [Dickinson-COMP-491-491/AY26-27](https://github.com/Dickinson-COMP-491-492/AY26-27) repository.
      - `git remote add upstream <URL>`
   3. Pull the upstream `main` branch to synchronize with the upstream.
   4. Create a new feature branch from `main` for this assignment.
2. Select at least 4 of your candidate projects that seem most promising to you.
3. Add a bullet for "Project Explorations" in the "Assignments" section of your `README.md` file.
4. For each candidate project that you selected you should spend approximately 30-45 minutes exploring it and documenting what you find as follows:
   1. Create a new `.md` file with an appropriate name for the project exploration in your directory.
   2. Add a sub-bullet under "Project Explorations" that gives the name of the project that you are exploring and link it to the `.md` file that you just created.
   3. Add the following sections and create the indicated content in the `.md` file for the project exploration:
      - **Project Exploration:** A top level section heading with the text "Project Exploration".
      - **Project Title:** The title of the project.
      - **Project Repository:** The URL of the repository (or repositories, or organization) where the latest version of the source code is located.
      - **Project Homepage:** The public-facing homepage for the project. For many projects this will be different from the repository. Some smaller projects may keep everything in the repository. Use "N/A" here if there is no homepage. 
      - **Product:** Summarize in a paragraph what the software product does.
      - **Target User Community:** Summarize in a paragraph: (i) Who is the user community for the software product? (ii) What need(s) of this user community does the software address? Briefly explain how the software addresses those needs.
      - **Activity:** Give some things that you noticed that indicate that the project is active, has some developer community around it, and is supportive of outside contributions. The more evidence you can find that the project is alive, thriving, and open the better. You should at least consider things like the volume of recent activity on the issue tracker or message forums, the frequency of creation and merging of pull requests.
      - **Getting Started:** Imagine that you have been assigned to start working on this project as a developer. Explore the project repository and homepage looking for resources that would help you get started (e.g. how to install the developer environment, how to contribute, how to communicate with the community, etc). Give your impression of the things that would make it easy or difficult to get started on the project (e.g. was documentation easy to find? does it seem complete? is it written clearly and at a level you can follow?) Support your impression with details from your research and include links to resources as appropriate.
      - **Welcoming to Newcomers:** Briefly document what you find (or do not find) that indicates that the community is welcoming and supportive of newcomers. You should briefly scan documentation, the issue tracker and any open communication channels for the project. Look for things like "Getting Started" documents, message board threads where newcomers or students introduce themselves, tags on issues such as "Good First Issue" or "First Timers," and comments/feedback on appropriately tagged issues. You might also consider the "tone" in the communications that you find.
      - **Skills Match:** Briefly identify the main languages / frameworks / tools that the project uses and describe how well they match or do not match your current knowledge and skill set.
      - **Personal Interest:** Briefly describe the reasons that led you to chose to explore this project. Discuss anything that you learned during the exploration that increased or decreased your interest in engaging with this project. State whether you are interested in continuing to consider this project and why or why not.
      - **Other:** Add any additional thoughts that you would like to record about the project.  Include things that you think may be helpful later as you continue to narrow down the projects you are considering and ultimately decide which project to engage with.
   4. Commit your changes to your feature branch. Note that each project exploration should be in a separate commit.
4. Turn in your work.
   1. Push your feature branch to GitHub.
   2. Create a pull request to the upstream course repo for your changes.

## Acknowledgements

This assignment builds from and adapts ideas and content from the following activities created by others:

- This version incorporates some nice revisions to an earlier version that were made by John MacCormick in [2023](https://dickinson-comp491-fall2023.github.io/comp491-fa2023-web/hw/HW2-project-exploration.docx).
- https://github.com/ChrisMurphyOnline/open-source-software-development-course/blob/master/activities/foss-evaluation-activity.txt
- http://foss2serve.org/index.php/Project_Anatomy_Activity
- http://foss2serve.org/index.php/FOSS_Field_Trip_Activity
- http://foss2serve.org/index.php/Project_Evaluation_Activity_V2
- https://github.com/ChrisMurphyOnline/open-source-software-development-course/blob/master/activities/foss-get-involved.txt

---

![Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png "Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License") All textual materials used in this course are licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/)

![GPL V3 or Later](https://www.gnu.org/graphics/gplv3-or-later-sm.png "GPL V3 or later") All executable code used in this course is licensed under the [GNU General Public License Version 3 or later](https://www.gnu.org/licenses/gpl.txt)
