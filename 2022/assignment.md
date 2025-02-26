---
title: "Assignment 2022"
layout: tud-toc
---


## Getting Started

To get started with the assignment, the following tasks need to be completed:

1. [Form a team](#team-formation) and register on Brightspace
2. [Pick a suitable project](#picking) and claim it on the Brightspace forum
3. Write your [project introduction](#gitlab) and make your first contribution to DESOSA on GitLab

<a id="team-formation"></a>

### Team Formation

As software architecture is all about collaboration and communication, the work must be done in teams:

1.	Required team size is 4
2.	Aim for diversity in your team. For example, aim at at a mixture of master tracks, backgrounds, domain knowledge, technical expertise,  cultures, countries, etc. This will broaden your horizon and offer opportunities to learn from each other.
3.  Form your group in Brightspace. Go to Collaboration -> [Groups].

If you are looking for partners, you can post a message on our Brightspace forum (there is a topic for [partners wanted][partners]), and offer your expertise.

[brightspace]: https://brightspace.tudelft.nl/d2l/home/400610
[partners]: https://brightspace.tudelft.nl/d2l/le/280700/discussions/topics/42189/View
[groups]: https://brightspace.tudelft.nl/d2l/lms/group/group_list.d2l?ou=400610

<a id="picking"></a>

### Picking a Project

In principle you are free to pick any open source project on GitHub. Take the following factors into account:

* The project should be sufficiently large and complex to make it interesting, but not too large to keep the assignment manageable. A system of around  100,000 lines of code is a good guideline: If you're interested in a larger system try  to identify a smaller component that you can focus on.
* The project should be under active development (a pull request handled  per day would  be a good number).
* The project should use GitHub as its main communication platform (and not merely as a mirror, as, e.g., Linux is doing).
* The project should not have been used in previous courses in the two  previous years (you can see them by checking previous versions of our books -- see the list of [non-projects](non-projects.html).
* The project should be open to external contributors (i.e. accept pull requests from outsiders).

To get you started, we hand-picked a [list of projects](suggested-projects.html) which are large, actively developed, maintained by a vibrant community, and are not analyzed in the previous runs of this course.

To claim a project: Post on the Brightspace forum, title _Claiming project P_, explain why you like this project in the issue, and indicate the 4 team members that will work on this project as well as your group number. Make sure to add their GitLab accounts in the issue so we can find them.

After your project choice is approved, you will be granted [access to the GitLab repository](#gitlab) where you can find your project in the `./content` directory. Add a short (around 100 words) enthusiastic description of the project to the  `_index.md` file in your project sub folder (see the [usage instructions][gitlab-desosa-project-page] of the DESOSA project for more information). Consider adding a logo or some representative image, and provide all the required meta-data. Also fill out the author details with your names and a small introduction.


[claiming]: https://brightspace.tudelft.nl/d2l/le/280700/discussions/topics/42190/View
[gitlab-desosa-project-page]: https://gitlab.ewi.tudelft.nl/in4315/2021-2022/desosa2022#project-page


<a id="gitlab"></a>

### Getting Access to GitLab for Writing

All team members will get access to a shared [GitLab][gitlab-desosa] repository hosting the sources of DESOSA 2022.

Within this repository, each team will have one dedicated project sub-folder to work in.
Teams should only add changes to their own sub-folder (`./content/projects/<projectname>`).

The repo includes all essays written for all projects. The essays themselves are writen in [Markdown], and rendered using [Hugo]. Usage instruction are provided on the [README][gitlab-desosa] page of the DESOSA project.

Follow all good software development practices in this repository, such as using issues and milestones for planning, merge requests, review, etc. Show that you are well-organized, and that the teachers can clearly see what you did and what you  are planning to do.

You are encouraged to use issues and must use merge requests, properly labeling them with an identifier for your project.

(Some teams prefer to use a collaborative tool like Overleaf or Google Doc for "pair writing". That is OK, as long as the eventual result is committed, in time, in the gitlab repository in proper markdown format.)

[gitlab-desosa]: https://gitlab.ewi.tudelft.nl/in4315/2021-2022/desosa2022
[hugo]: https://gohugo.io/
[markdown]: https://daringfireball.net/projects/markdown/


## The Assignment

The main part of the assignment consists of three parts:

1. Writing four [essays](#essays) about different aspects of your project and reviewing the essays of others teams
2. [Contributing](#contributions) to your project
3. Keeping track of your progress through personal [journals](#journals)


<a id="essays"></a>

### Essays

Strong writing skills are an invaluable asset for an architect. To quote [Dan Heller] in his "Ten Principles for Growth as an Engineer":

> Crisp technical writing eases collaboration and greatly improves your ability to persuade, inform, and teach.

Therefore, we will use this course to train and improve our writing skills.

Each team will write four essays. Each essay should be around 1500-2000 words. After 2000 words teachers (or any reader, in fact), reserve the right to stop reading, which may affect your grade. We'll be counting words by running [Markdown Word Count], developed by a former Software Architecture student, on your `.md` markdown files.

Your essays will be evaluated based on the following:

1. The text is well-structured, with a clear goal, a natural breakdown in sections, and a compelling conclusion.
2. Sentences, paragraphs, and sections are coherent. They naturally build upon each other and work towards a clear message. 
3. The arguments laid out are technically sound, and of adequate technical depth.
4. The English writing is grammatically correct
4. A standard notation, such as [UML 2](https://en.wikipedia.org/wiki/Unified_Modeling_Language), is appropriately used for all diagrams
5. The text clearly references any sources it builds upon
6. The essay is unique and recognizable in its voice and its way of approaching the topic
7. The essay is independently readable
8. The story-line is illustrated with meaningful and appealing images and infographics.

The intended audience for the essays consists of computer science students or software engineers, interested in learning about architectural aspects of your open source project.

A [publicly visible blog][desosa2022] is available through which teams can publish their essays. We are publishing the essays throughout the course (and not just all at once after the course). We will use the blog to engage with and share our work with the open source community. Published essays (blog posts) will carry a [CC BY-SA 4.0] license, allowing the open source projects to include the resulting posts in their own documentation.
You can decide yourself which posts you want to make public by means of [simple meta-data flag][gitlab-desosa-consent] in your Hugo markdown document.

[Dan Heller]: https://medium.com/@daniel.heller/ten-principles-for-growth-69015e08c35b
[Markdown Word Count]: https://github.com/gandreadis/markdown-word-count
[cc by-sa 4.0]: https://creativecommons.org/licenses/by-sa/4.0/legalcode
[desosa2021]: https://2021.desosa.nl/
[desosa2022]: https://desosa2022.netlify.app/
[gitlab-desosa-consent]: https://gitlab.ewi.tudelft.nl/in4315/2021-2022/desosa2022#consent-to-publish-publicly


<a id="vision"></a>

#### Essay 1: Product Vision and Problem Analysis


The starting point for your architectural analysis is a description of the _vision_ underlying your project and its future success. 
Aspects to take into account include:

1. A concise, inspirational characterization of what the project aims to achieve
1. A brief explanation of the key domain concepts (underlying domain model)
1. A description of the system's main capabilities (e.g. use cases), as they are visible to the typical (end) user
1. A description of the current and future (external) context in which the system operates
1. An analysis of the stakeholders involved in the project, and what they need from the system so that it is beneficial to them
1. A characterization of key quality attributes the system must meet
1. A product roadmap, laying out the main directions anticipated for the upcoming years
1. Ethical considerations of the system and its construction process

It may be the case that some of these aspects do not naturally match your open source system under investigation. In that case, say so explicitly, and explain why you think this is the case in your essay. Instead offer a deeper analysis of other relevant aspects.

Relevant literature for this essay includes 

- _Software Architecture Visual Lecture Notes_ [^pautasso]: Chapters 2 (Quality Attributes), 3 (Software Development Lifecycle) and 4 (Domain Model, System Context View)
- _arc42 documentation_ [^arc]: Chapters 1 (Requirement and goals), 2 (Constraints) and 3 (Scope & Context)
- _Lean Architecture_ [^coplien], Chapters 2 (end-user mental model), 3 (stakeholder analysis), and 4 (problem definition)
<!-- - _Software Systems Architecture_ [^rozanski], Chapter 9 (stakeholder analysis) and 16 (context analysis) -->


<a id="architecture"></a>

#### Essay 2: From Vision to Architecture

While the first essay focuses on the set of fundamental concepts or properties of the system in its environment, 
in the second you explore how these are realized through the system's architectural elements and relationships, and the principles of its design and evolution.
Aspects to take into account include:

1. The main architectural style or patterns applied (if relevant), such as layering or model-view-controller architectures.
2. Containers view: The main execution environments, if applicable, as used to deploy the system.
3. Components view: Structural decomposition into components with explicit interfaces, and their inter-dependencies
4. Connectors view: Main types of connectors used between components / containers.
5. Development view, covering the system decomposition and the main modules and their dependencies, as embodied in the source code.
6. Run time view, indicating how components interact at run time to realize key scenarios, including typical run time dependencies
7. How the architecture realizes key quality attributes, and how potential trade-offs between them have been resolved.
8. API design principles applied

It may be the case that some of these aspects do not naturally match your open source system under investigation. In that case, say so explicitly, and explain why you think this is the case in your essay. Instead offer a deeper analysis of other relevant aspects.

Relevant literature for this essay includes 

- _Software Architecture Visual Lecture Notes_ [^pautasso]: Chapter 4
- _arc42 documentation_ [^arc]: Chapters 4-9
- _C4 model_ [^c4]: Levels 2 (Containers) and 3 (Components)

<!--
- _Lean Architecture_ [^coplien], Chapters 5-7
- _Software Systems Architecture_ [^rozanski],  Chapters 20 (development viewpoint) and 21 (deployment viewpoint)
- _SIG componentization_: The Sigrid Beta Architecture visualization for your system may provide input to your development view
-->


<a id="quality"></a>

#### Essay 3: Quality and Evolution

With key aspects of the architecture described, the third essay focuses on means to safeguard the quality and architectural integrity of the underlying system, with special empahsis on the rate of change.
Aspects to take into account include:

1. The system's key quality attributes and the degree to which they are currently satisfied
1. The overall software quality processes that apply to your system
2. The key elements of the system's continuous integration processes
3. The rigor of the test processes and the role of test coverage
4. Hotspot components from the past (previously changed a lot) and the future (needed for roadmap)
5. The code quality, with a focus on hotspot components
6. The quality culture, as evidenced in actual discussions and tests taking place in architecturally significant feature and pull requests (identify and analyze at least 10 such issues and 10 such pull requests)
7. An assessment of technical debt present in the system.

Again, it may be the case that some of these aspects do not naturally match your open source system under investigation. Also, doing all of these well may not fit in a single essay. Select those aspects that are most relevant, and do a thorough analysis for them. 

If you conduct measurements, you may find that certain numbers point at poor code quality.
In such cases, offer an explanation _why_ the code ended up like it is now, 
assess whether trade-offs have been made, and demonstrate leadership by offering constructive proposals how to resolve the problems you found.

Relevant pointers for this essay include:

- Martin Fowler: _Technical Debt_. https://www.martinfowler.com/bliki/TechnicalDebt.html
- _SonarQube_: https://www.sonarqube.org/
- _JArchitect_: https://www.jarchitect.com/Metrics
- _arc42 documentation_ [^arc]: Chapters 10 and 11.


<a id="scalability"></a>
#### Essay 4: Scalability
Your team's final essay serves to deepen your analysis in an aspect
where software architecture plays a particularly important role, namely
the system's _scalability_.
This includes ensuring that under increasing workloads
or reduced resources (think of porting to a resource-constrained platform)
the system exhibits adequate

1. time performance regarding
latency, throughput, processor time requirements, real time response, or
time variability;
2. space performance associated with the main and secondary memory; and
3. energy consumption performance.

The study should include the following.

1. Identification of the system's key scalability challenges under a
   plausible scenario.
2. Empirical quantitative analysis under varying workloads
   of at least one scalability dimension that can limit scalability .
   Examples include achievable transactions per second, processing time,
   memory use, or energy consumption.
3. Identification of the system's architectural decisions that affect
   its scalability.
4. Proposals for architectural changes that can address the identified issues.
5. Diagrams in a standard notation,
   such as [UML 2](https://en.wikipedia.org/wiki/Unified_Modeling_Language),
   depicting the "as is" and the "to be" architectural designs.
6. An argument using an appropriate method (analysis, simulation, or experiment)
   showing how the proposed changes will address the identified scalability
   issues.

Relevant pointers for this essay include:

- _Software Architecture Visual Lecture Notes_ [^pautasso]: Chapter 11 (Scalability)
- Beyer, Betsy, Chris Jones, Jennifer Petoff, and Niall Richard Murphy. _[Site reliability engineering: How Google runs production systems](https://sre.google/sre-book/table-of-contents/)_. O'Reilly Media, Inc., 2016.   Chapters 19–21, 25.
- Hull, Sean. [20 obstacles to scalability.](https://queue.acm.org/detail.cfm?id=2512489) _Communications of the ACM_ 56, no. 9 (2013): 54-59.
- Killalea, Tom. [Building Scalable Web Services: Build only what you really need.](https://dl.acm.org/doi/pdf/10.1145/1466443.1466447) Queue 6, no. 6 (2008): 10-13.
- Cole, Clem, and Russell Williams. [Photoshop scalability: Keeping it simple.](https://queue.acm.org/detail.cfm?id=1858330) _Communications of the ACM_ 53, no. 10 (2010): 32-38.
- [Patterns for scalable and resilient apps](https://cloud.google.com/architecture/scalable-and-resilient-apps)


#### Submissions

Once you are ready to submit your essay, please follow the following steps:

1.  Open a merge request on GitLab, and make sure that your team members review your changes.
    If everything looks good and everyone approves, you can merge your MR.

    **Important note:** Your MR needs to be merged for it to be considered submitted.

2.  To prepare your essay for peer reviews, a PDF, _containing only your new essay_, needs to be created.
    See the [README on GitLab][gitlab-desosa-pdf] for instructions on generating such a PDF locally or on the DESOSA site.

3.  Submit your essay to [peer.tudelft.nl][peer], the peer evaluation system that we use.
    After logging in with your NetID, you can find the Software Architecture course under "Enrolled Courses".
    On the course page, select the assignment matching your essay and submit the PDF from step 2.
    
    _Note:_ This only needs to be done once per team.

[gitlab-desosa-pdf]: https://gitlab.ewi.tudelft.nl/in4315/2021-2022/desosa2022#pdf
[peer]: https://peer.tudelft.nl/

<a id="contributions"></a>

### System Contributions

To familiarize yourself with the system under analysis, your team will _contribute_ to the system.
This will take the form of a pull request to the system.
Aspects to consider include:

1. It is probably a good  idea  to start with a very simple pull request, just to understand the whole process.
2. Starting with a documentation pull request might be a good way to get started.
3. Many projects have labels for issues that are easy to start with for newcomers to the project. Explore these and see if you can help.
4. After one or two simple pull requests, try to contribute more substantially, for example in refactorings or simple features.
5. In your interactions (in GitHub comments) with the developers  who are responsible for integrating your change, be polite, to the point, and responsive.
6. Follow any guidelines, for example in the projects `CONTRIBUTING.md` file.

For pull requests you've actually submitted, [create a new contributions entry in the DESOSA project][gitlab-desosa-contributions] to share your contributions on the website and PDF/epub.

There will be two deadlines, for two simple reports:

- Pull request midway report: Halfway the course, ensure submitted pull requests have all been added to your [DESOSA contributions listing][gitlab-desosa-contributions], and write a short plan for remaining pull requests that you still intend to submit.
- Pull request final report: Again, ensure all submitted pull requests have been added to your [DESOSA contributions listing][gitlab-desosa-contributions]. Furthermore, for work on potential pull requests you  _tried_, but which eventually did not result in an actual pull request submission, write a short summary of what you did, and what was so hard about it.

The two reports can be put in a file `contributions.md`, which you can put in your `journals` folder (so that it is ignored by Hugo). As an indication, around 100 words will probably suffice per planned (or terminated) pull request.

Pull requests will be graded, based on the following criteria:

- Timely start and well-caried out series of activities that lead to pull requests.
- Professional (responsive, polite, clear, to the pont) interaction with open source developers
- Substance of the pull requests

While your aim is of course that the pull request gets merged, the merge itself is not part of the grade.

[gitlab-desosa-contributions]: https://gitlab.ewi.tudelft.nl/in4315/2021-2022/desosa2022#contributions


<a id="journals"></a>

### Individual Journals

You will have considerable freedom in this course. Nevertheless, a _steady heartbeat is required_, and you are accountable for how you spend your time.

In this course, you have 5 EC available for software architecture in 8 weeks, giving a _minimum effort of 5 * 28 / 8 = 17.5 hours per week_ that you should spend on this course.

Use this time to learn as much as you can, as an architect is always eager to learn more.
Grading will also be based on the progress you made compared to your initial knowledge and skill level, not just based on a preset end-goal.

To make this possible, it is important that you and your team provide insight in what you do each week. To that end:

1. Create a journal file for each team member in the `journals` directory of your project.
2. Team members individually reports their own weekly experiences and effort in the course. It is important to commit and push these reports weekly (or even more frequently), and that you commit your own updates.

In the journal, you can offer a story of what you learned, what activities you participated in (lectures, meetings).
All effort related to the course can be included, including routes taken that do not directly lead to text in your essays (e.g., projects considered when selecting your project).
For each week, also include _the number of hours you spent that week on the software architecture course_.


<a id="videos"></a>

### Final Presentation

#### Video

The course will be concluded with an online presentation day. To that end each team prepares a 10 minute video highlighting their work. 

The primary audience for this video is your fellow students who also followed this course.
Furthermore, try to make the video of interest to current or future contributors of the open source system you analyzed.

Aspects you can cover in your video include the purpose of the system (essay 1), the underlying architecture (essay 2), the quality assurance process (essay 3), as well as your choice of topic for essay 4.
As it is impossible to cover everything you did, please focus on what sets your system apart from many other systems -- the key thing other students in this course should learn about your system.

In terms of video style, feel free to use your full creativity.
The best videos trigger applause and awe when presented to all students.
If possible, try to make it clear that the video is _team_ work, by letting all team members feature in the video.

You should upload your video as a (unlisted or public) YouTube video, and add the URL to your project page on the DESOSA website.
See the [DESOSA README][gitlab-desosa-videos] for full instructions on how to add the video.
You can indicate whether you want your video to be public.
Both should be done _before_ the deadline of the presentation video.

[gitlab-desosa-videos]: https://gitlab.ewi.tudelft.nl/in4315/2021-2022/desosa2022#videos


#### Presentation Day

During presentation day, we will create six _sessions_ of approximately two hours.
Sessions will start at 10:00, 12:30, and 15:00, in two parallel tracks (in two separate Zoom calls).

For each team, there will be 20 minutes. During the first 10 minutes the team's video will be shown.
During the second 10 minutes there will be Q&A. All four team members must be present, and should be involved in answering questions.

Each team is expected to join the full (two hour) session during which their own video is shown and discussed,
and participate actively in the discussions of the other four teams in the same session.

Furthermore, individual students are welcome to join any other session and participate in the Q&A (but this is not compulsory).


#### Grading

Students should fill in a form for each of the four presentations and Q&A sessions they participate in.
This form will distinguish content depth, presentation style, and the handling of questions.

In each session 1-2 teachers will participate, who will also grade the teams.

The Q&A sessions including the chat will be recorded.



## References

[lsa]: http://www.leansoftwarearchitecture.com/
[views]: https://www.viewpoints-and-perspectives.info/
[arc42]: https://docs.arc42.org/home/
[cesare]: https://leanpub.com/software-architecture/

[^coplien]: Jim Coplien Gertrud Bjørnvig. [Lean Architecture][lsa] for Agile Software Development. Wiley, 2010.

[^rozanski]: Nick Rozanski and Eoin Woods. [Software Systems Architecture: Working with Stakeholders Using Viewpoints and Perspectives][views]. Addison-Wesley, 2012, 2nd edition.

[^pautasso]: Cesare Pautasso. Software Architecture: Visual Lecture Notes. Leanpub, 2020. [leanpub.com][cesare].

[^kruchten]: Philippe Kruchten. The 4+1 View Model of architecture. IEEE Software 12(6), 1995.
    ([doi](https://doi.org/10.1109/52.469759), 
    [preprint](https://www.cs.ubc.ca/~gregor/teaching/papers/4+1view-architecture.pdf), 
    [wikipedia](https://en.wikipedia.org/wiki/4%2B1_architectural_view_model))

[^arc]: Peter Hruschka and Gernot Starke. arc42: Effective, lean and pragmatic architecture documentation and communication. [https://docs.arc42.org/home/][arc42]

[^c4]: The C4 model for visualising software architecture. [https://c4model.com/](https://c4model.com/).

[^cataldo]: Cataldo, Herbsleb, and Carley.  Socio-Technical Congruence: A Framework for Assessing the Impact of Technical and Work Dependencies on Software Development Productivity. ICSE 2008. [https://herbsleb.org/web-pubs/pdfs/cataldo-socio-2008.pdf](https://herbsleb.org/web-pubs/pdfs/cataldo-socio-2008.pdf)


