## PA02: Candidate Projects

### Introduction

Selecting the H/FOSS (FOSS or humanitarian FOSS) project on which you will work is a four step process. This assignment, **PA02 - Candidate Projects** is the first step. In this step you will explore a variety of H/FOSS projects to learn what they do and quickly assess their suitability for this course. In the next assignment, **PA03 - Project Explorations** you will dig deeper into some of the candidate projects that you identified, to determine things such as whether they are active and open to contributions, and how approachable they seem to be.  **PA04 - Project Reviews** asks you to become more informed about the projects in which you are most interested. Then in **PA05 - Project Ranking and Selection** we will form teams around commonalities in the projects that were reviewed and each team will work together to select the project on which they will work.

### Recommended Background Reading

Before beginning it is recommended that you read [What you actually need to know about open source to get started](https://opensource.com/article/22/11/get-started-open-source) and [Open-Source Contribution: The Ultimate Guide](https://builtin.com/software-engineering-perspectives/open-source-contribution) to get a feel for the kinds of things you'll want to be thinking about as you browse projects looking for ones that you might be interested in working on.

### Assignment

Use the steps outlined below to build the list of *candidate projects* to which you might be interested in contributing.

1. Browse the resources in the [Finding H/FOSS Projects](#finding-hfoss-projects) section looking for projects that interest you. It is recommended that you consider projects from across a range of your different interests.  Eventually we will be forming teams around areas of common interest.  So having considered projects across a range of interests increases the likelihood that you will find a team with some shared interests.
2. From the projects that interest you, identify at least 10 candidate projects that you are interested in exploring more deeply. Candidate projects must:
   - be under active development (recent commits, issues, pull requests, etc).
   - have a stated license (without one it can't be used for this course).
   - have at least some basic documentation (e.g. README, INSTALL, CONTRIBUTING, etc).
3. Using your clone of the course repository:
   1. Ensure that you are on the `main` branch.
   2. Set the upstream remote of your clone to point to the [Dickinson-COMP-491-491/AY26-27](https://github.com/Dickinson-COMP-491-492/AY26-27) repository.
      - `git remote add upstream <URL>`
   3. Pull the upstream `main` branch to synchronize with the upstream.
   4. Create a new feature branch from `main`.
   5. In your directory (i.e. the one with your name):
      1. Create a new file in your directory to hold information about your candidate projects.
      2. Create a link to this new file under the "Assignments" heading in your `README.md` file.
      3. Create nicely formatted content in the new file for each candidate project including:
         - the name of the project
         - a link to its home page and/or repository.
         - 1-2 sentences description of the purpose of the project and the community it serves. 
         - 1-2 sentences summarizing of your interest level in the project and your impression of the suitability of the project for this course. 
   6. Commit your changes to your feature branch.
   7. Create a pull request to the upstream for your feature branch.
   8. Check the changes in your pull request on GitHub to ensure that they are correct.

### Finding H/FOSS Projects

There are literally millions of open source projects out there. However, not all open source projects are equally good candidates for engagement. You will, of course, want to find projects that you are interested in. But you'll also want to find projects that are active, technically approachable, have a variety of ways to contribute and have a welcoming developer community that will help you get started and that you can go to when you have questions. Below are resources that may help you find suitable candidate projects.

#### Humanitarian FOSS (HFOSS) Projects

As you know, HFOSS is an acronym for humanitarian free open source software. We encourage you to explore at least a few *humanitarian* FOSS (HFOSS) projects because they reflect the potential for computing to benefit society and thus will align your major well with the broader mission of Dickinson College. In addition, past students and faculty from this course, and other courses similar to ours, report that HFOSS project communities tend to be friendly, supportive and open to helping new contributors come on board. That said, you should explore and select projects according to all relevant factors, including your own personal interest and you are not required to pursue any humanitarian projects.

The following lists are good places to find humanitarian projects that might be of interest:
- [HFOSS Projects](https://teachingopensource.org/HFOSS_Projects) NOTE: Be sure to examine the whole page, not just the table at the top. The bullet point lists contain projects that are not in the table at the top of the page.
- [awesome-humanitarian-foss](https://hfoss.etica.ai/): A curated list of HFOSS projects.

#### Projects with Mentor Connections

Having a mentor to guide your work in a project can be very useful in getting started, identifying appropriate tasks and getting help when you are stuck. Regardless of the project that you pick you will want to make an effort to find a mentor in the project. This is easier in some projects and harder in others. 

There are several projects where we have potential mentor connections:

- [OpenStack: Swift](https://www.openstack.org/software/releases/dalmatian/components/swift) - Distributed object storage.
  - A contact at the [OpenInfra Foundation](https://openinfra.dev/) has offered to try to connect a few teams from Dickinson with mentors in OpenInfra swift.  She may also be able to help with connections in other [OpenStack projects](https://www.openstack.org/software/project-navigator/openstack-components#openstack-services).

- [Rust](https://github.com/rust-lang) - The Rust programming language.
  - [Ben Kimock](https://github.com/saethlin) is a Dickinson alum and has been a contributor to the Rust language project. He has offered to connect with interested students.

- [Penrose](https://penrose.cs.cmu.edu/) - Plain text diagramming tool.
  - [Wode "Nimo" Ni](https://github.com/wodeni) is a Dickinson alum who started the Penrose project as part of his Ph.D. studies at Carnegie Mellon. He has offered to connect with interested students.

#### Broader H/FOSS Project Lists

The following lists are also good places to find H/FOSS projects that are are open to contributions:

- [Past Google Summer of Code Projects](https://summerofcode.withgoogle.com/archive): The H/FOSS projects that have participated in Google's Summer of Code program.
- [Past Outreachy Internship Projects](https://www.outreachy.org/past-projects/): The H/FOSS projects that have sponsored Outreachy internships.
- [NumFOCUS Sponsored](https://numfocus.org/sponsored-projects) and [Affiliated](https://numfocus.org/sponsored-projects/affiliated-projects) projects that focus on research, data, and scientific computing.
- [Awesome FOSS apps](https://github.com/DataDaoDe/awesome-foss-apps): A curated list of some large popular FOSS projects.

#### H/FOSS Projects for New Contributors

There are also a few sites that are specifically designed to help new people get involved in FOSS projects. These often have a list of projects with "introductory" issues that make good targets for new contributors. Listing a project here and tagging issues as "introductory" suggests that the projects may be particularly welcoming to new contributors. So you may want to search these sites:

- [Up For Grabs](https://up-for-grabs.net/#/)
- [Good First Issue](https://goodfirstissue.dev/)
- [Awesome For Beginners](https://github.com/MunGell/awesome-for-beginners)
- [OVIO](https://ovio.org/) - requires a free signup.

#### H/FOSS Projects Selected by Past Senior Seminar Teams

Below is the list of all H/FOSS projects selected as capstone projects by previous Dickinson senior seminar students. Note that we do not necessarily recommend every project on this list. Every project has both advantages and disadvantages. Projects where students have had particularly good experiences are marked with an 🏆. Note though that projects change over time so past experience is not necessarily predictive of current success. If you are considering pursuing one of these projects, feel free to discuss it with the instructor to find out about the experience of previous Dickinson students.

- 2025-26:
  - [Unsloth](https://github.com/unslothai/unsloth)
  - [Godot](https://github.com/godotengine/godot) 🏆
  - [Open Library](https://github.com/internetarchive/openlibrary) 🏆
  - [Music Blocks](https://github.com/sugarlabs/musicblocks) 🏆
- 2024-25:
  - [DocsGPT](https://github.com/arc53/docsgpt)
  - [Internet Archive](https://archive.org/) 🏆
  - [Mermaid](https://mermaid.js.org/) 🏆
  - [OpenStack:Swift](https://www.openstack.org/software/releases/dalmatian/components/swift) 🏆
  - [Oppia](https://www.oppia.org/) 🏆
  - [TypeScript](https://www.typescriptlang.org/)
  - [Zed Attack Proxy](https://github.com/zaproxy)
  - [Zulip](https://zulip.com/) 🏆
- 2023-24:
  - [Apache Kafka](https://kafka.apache.org/)
  - [SugarLabs](https://www.sugarlabs.org/) 🏆
  - [OpenBSD](https://www.openbsd.org/)
  - [Huggingface](https://huggingface.co/)
  - [Mermaid](https://mermaid.js.org/) 🏆
- 2022-23: 
  - [Hugging Face Transformers](https://github.com/huggingface/transformers)
  - [Oppia](https://www.oppia.org/) 🏆
  - [Wagtail](https://wagtail.org/) 🏆
- 2021-22: 
  - [Kubernetes](https://kubernetes.io/)
  - [Teammates](https://github.com/TEAMMATES) 🏆 
  - [The Odin Project](https://github.com/TheOdinProject/) 🏆
  - [SymPy](https://www.sympy.org/en/index.html)
  - [Wagtail](https://wagtail.org/) 🏆
- 2020-21: 
  - [book project](https://github.com/Project-Books/book-project) 🏆
  - [OpenMRS](https://openmrs.org/)
  - [Numpy](https://numpy.org/) 
- 2019-20: 
  - [FreeCodeCamp](https://www.freecodecamp.org/) 🏆
  - [Jenkins](https://www.jenkins.io/)
  - [Godot Engine](https://godotengine.org/)
- 2018-19: 
  - [FreeCodeCamp](https://www.freecodecamp.org/) 🏆
  - [OpenMRS](https://openmrs.org/)
  - [Audacity](https://www.audacityteam.org/)
- 2017-18: 
  - [Sahana Eden](https://sahanafoundation.org/products/eden/)
  - [FreeCodeCamp](https://www.freecodecamp.org/) 🏆
  - [Atom](https://github.com/atom/atom) 🏆
- 2016-17: 
  - [OpenMRS](https://openmrs.org/)
  - [React Native](https://reactnative.dev/)
  - [Sugar Labs](https://www.sugarlabs.org/) 🏆

In addition there are a number of other projects students and instructors from courses similar to ours have reported having good success with:

- [Runestone Academy](https://landing.runestone.academy/)
- [OpenEMR](https://www.open-emr.org/)
- [Libre Health](https://librehealth.io/)
- [Mifos](https://mifos.org/)
- [Ushahidi](https://www.ushahidi.com/)
- [GNOME Accessibility](https://wiki.gnome.org/Accessibility)
- [Kata Containers](https://katacontainers.io/)
- [Zuul](https://zuul-ci.org/docs/zuul/latest/)

#### H/FOSS Projects You Already Know or Use

Think about the apps, software, frameworks, libraries and websites you use on your phone and computer. Which of them are open source? Are any of them suitable as capstone projects? If so, feel free to explore them.

#### Other Collections of H/FOSS Projects

If nothing in any of those places catches your attention, or you want to explore further you can leap into the void and search some of the large open source project repositories. Most of the above projects are located in one of the following repositories, but these repositories also contain millions of other projects as well. Some will be great projects to get involved with, but others will be too large, too specialized, dead, or exclusive. So if you do head off into the void searching for projects, spend a few minutes informally assessing how active a project is and how open/welcoming/accessible it is to new contributors before spending the time to explore it in detail. That said, here's a list of repositories:

- The Big Two:
  - [GitHub](https://github.com/)
  - [GitLab](https://gitlab.com/explore)

- Some other possible places to find projects:
  - [SourceForge](https://sourceforge.net/)
  - [Launch Pad](https://launchpad.net/)
  - [Savannah](http://savannah.gnu.org/)
  - [GNOME](https://welcome.gnome.org/)

<!-- Appears to be dead:
  - [BLACKDUCK - Open Hub](https://www.openhub.net/explore/projects)
  -->

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
