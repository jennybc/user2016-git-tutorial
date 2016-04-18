Using Git and GitHub with R, RStudio, and R Markdown
================

##### Jenny Bryan, University of British Columbia & rOpenSci

Overview
--------

Data analysts can use the [Git version control system](https://git-scm.com) to manage a motley assortment of project files in a sane way (e.g., data, code, reports, etc.). This has benefits for the solo analyst and, especially, for anyone who wants to communicate and collaborate with others. Git helps you organize your project over time and across different people and computers. Hosting services like [GitHub](https://github.com), [Bitbucket](https://bitbucket.org), and [GitLab](https://about.gitlab.com) provide a home for your Git-based projects on the internet.

What's special about using R and Git(Hub)?

-   the active R package development community on GitHub
-   workflows for R scripts and [R Markdown](http://rmarkdown.rstudio.com) files that make it easy to share source and rendered results on GitHub
-   Git- and GitHub-related features of the [RStudio IDE](https://www.rstudio.com/products/rstudio-desktop/)

Outline
-------

The tutorial will be structured as ~5 task-oriented units. Indicative topics:

-   The most difficult part: installation and configuration!
-   Creating a Git repository and connecting the local repo to a GitHub remote, for new and existing projects.
-   The intersection of GitHub and the R world: R packages developed on Github and how to make use of ["issues"](https://guides.github.com/features/issues/); [METACRAN](http://www.r-pkg.org) [read-only mirror](https://github.com/cran) of all of CRAN; R-specific searching tips.
-   How to propose a change or fix to someone else's project, i.e. "make a [pull request](https://help.github.com/articles/using-pull-requests/)".
-   Daily workflows and FAQ: how often should I commit?, which files should I commit? how do I change a commit or its message? how do groups of 1, 5, or 10 people structure their work with Git(Hub)? etc.

This will be a hands-on tutorial, so bring your prepared laptop and pre-register a free GitHub account (see below).

What this tutorial is not
-------------------------

This tutorial will teach novices about Git on a strict "need to know" basis. Git was built to manage development of the Linux kernel, which is probably very different from what you do. Most people need a small subset of Git's functionality and that will be our focus. If you want a full-blown exposition of Git as a directed acyclic graph or a treatise on the Git-Flow branching strategy, you will be sad.

Our target audience is someone who uses R to analyze data. While R package development with Git(Hub) is absolutely in scope, it's not an explicit focus or requirement.

We target GitHub -- not Bitbucket or GitLab -- for the sake of specificity. However, all the big-picture principles and even some mechanics will carry over to these alternative hosting platforms.

Background knowledge
--------------------

The tutorial is aimed at intermediate to advanced R users, who are comfortable writing R scripts and managing R projects. You should have a good grasp of files and directories and be generally knowledgeable about where things live on your computer.

Although we will show alternatives for most Git operations, we will inevitably spend some time in the shell and we assume some prior experience. For example, you should know how to open up a shell, navigate to a certain directory, and list the files there. You should be comfortable using shell commands to view/move/rename files and to work with your command history.

[R Markdown](http://rmarkdown.rstudio.com) or [RStudio](https://www.rstudio.com/products/rstudio-desktop/) will feature prominently in most of the units, so this tutorial will be most rewarding for people who already use these or are eager to try them out.

Preparation
-----------

Closer to the day, we will create a stand-alone website or GitHub repository with all materials.

Preparation instructions will be taken from those developed in [STAT 545](http://stat545.com), in case you want to start NOW!

-   [All the Git and GitHub (and RStudio) things](http://stat545.com/git00_index.html)

In an ideal world everyone will have successfully completed that set up in advance. In the real world, *we expect everyone to have tried that*, but that a subset will need some assistance in the first half hour.

Instructors
-----------

Jenny Bryan ([twitter](https://twitter.com/jennybryan), [GitHub](https://github.com/jennybc)) is a professor at the University of British Columbia. She's been using and teaching R (or S!) for 20 years, most recently in [STAT 545](http://stat545.com) and [Software Carpentry](http://software-carpentry.org). Other aspects of her R life include work with [rOpenSci](https://ropensci.org/about/#leadership), development of the [`googlesheets`](https://cran.r-project.org/web/packages/googlesheets/index.html) and [`gapminder`](https://cran.r-project.org/web/packages/gapminder/index.html) packages, and being academic director for [UBC's Masters of Data Science](http://mds.science.ubc.ca).

Dean Attali and Bernhard Konrad will be teaching assistants. They both have experience in teaching this material (and much more) in [STAT 545](http://stat545.com) and [Software Carpentry](http://software-carpentry.org). Added bonus: they know how to use Windows.

-   Dean Attali ([blog](http://deanattali.com), [GitHub](https://github.com/daattali/), [twitter](https://twitter.com/daattali)) is finishing up a Masters in Bioinformatics at UBC. He's the developer of the [shinyjs](https://cran.r-project.org/web/packages/shinyjs/index.html) package and [much more](http://deanattali.com/projects/).
-   Bernhard Konrad ([GitHub](https://github.com/BernhardKonrad), [twitter](https://twitter.com/bernhardkonrad)) recently earned his PhD in Applied Math at UBC, completed an [Insight Data Science Fellowship](http://www.insightdatascience.com), and is a software engineer at Google.
