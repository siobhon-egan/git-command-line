---
title: 'Wrap-up'
---

:::::::::::::::::::::::::::::::::::::: questions 

- Where can I learn more about using git?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Be familiar with useful resources for git

::::::::::::::::::::::::::::::::::::::::::::::::

> **RECAP**
>
>- The goal of this session is to become familiar with git and provide users with the confidence to use it in their study and work.
>- After today you should have created a GitHub account and configured your computer to use git version control software.
>- We stepped through an example that demonstrated the power of git version control in tracking history and changes.
>- This workshop provided a practical and 'hands-on' introduction to git. 
>- We did not cover all aspects of version control/git theory but hope you can now begin to navigate the world of git after today.
>- An important part of your git journey is learning how to navigate through online resources and find meaningful help. 


### Additional software carpentry lessons we did not cover today

We did not cover all lessons in the software carpentry suite today. After today's workshop you may find it helpful to navigate your own way through the remainder of the lessons to sharpen your new git skills.

A list of additional [git novice][sw-git-novice] lessons:

* [Collaborating](https://swcarpentry.github.io/git-novice/08-collab/index.html)
* [Conflicts](https://swcarpentry.github.io/git-novice/09-conflict/index.html)
* [Open Science](https://swcarpentry.github.io/git-novice/10-open/index.html)
* [Licensing](https://swcarpentry.github.io/git-novice/11-licensing/index.html)
* [Citation](https://swcarpentry.github.io/git-novice/12-citation/index.html)
* [Hosting](https://swcarpentry.github.io/git-novice/13-hosting/index.html)
* [Supplemental: Using Git from RStudio](https://swcarpentry.github.io/git-novice/14-supplemental-rstudio/index.html)

## Where to get help

* The [GitHub Docs pages](https://docs.github.com/en) are a good place to start
* GitHub has '[activities](https://guides.github.com/activities/hello-world/)' which aim to explain how git works
* GitHub also has interactive tutorials for their [online version (Learning Labs)](https://lab.github.com/) and for [using Git offline (Git-It)](https://github.com/jlord/git-it-electron#git-it-desktop-app)
* Atlassian has in depth but clear [tutorials](https://www.atlassian.com/git/tutorials) on using git
* Additional episodes for this workshop can be found at the software carpentry lesson site for [Version Control with Git](https://swcarpentry.github.io/git-novice/)
* [Complete list of all git commands](https://git-scm.com/docs/git#_git_commands)

## References for git/GitHub

Git cheat sheets:

- Printable Git cheat sheets in several languages are [available here](https://github.github.com/training-kit/) ([English version](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)). More material is available from the [GitHub training website](http://try.github.io/).
* [Tower client git cheat sheet](https://www.git-tower.com/blog/git-cheat-sheet/)

![](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf){width=200% height=500}


### Resources

- An [interactive one-page visualisation](http://ndpsoftware.com/git-cheatsheet.html) about the relationships between workspace, staging area, local repository, upstream repository, and the commands associated with each (with explanations).
- Both resources are also available in other languages (e.g. Spanish, French, and more).
- "[Happy Git and GitHub for the useR](http://happygitwithr.com)" is an accessible, free online book by Jenny Bryan on how to setup and use Git and GitHub with specific references on the integration of Git with RStudio and working with Git in R.
    - For RStudio users see the lesson on [using GitHub from RStudio](https://swcarpentry.github.io/git-novice/14-supplemental-rstudio/index.html)
- [Open Scientific Code using Git and GitHub](https://open-source-for-researchers.github.io/open-source-workshop/) - A collection of explanations and short practical exercises to help researchers learn more about version control and open source software.


### Help on error messages

These helpful coding tips have been inspired by [Y. Wendy Huynh from R for Graduate Students](https://bookdown.org/yih_huynh/Guide-to-R-Book/trouble.html)...(p.s. yes I know we are using git and not R here, but many tips still apply :smile:)

**Some common mistakes to watch out for when coding**

- Capitalization 
    - You typed an uppercase letter when you should have typed a lowercase letter (vice versa). 
    - Depending on the situation capitalization does not always matter but to be safe its best to make sure it does match.
- Mis-spelling
    - Sounds obvious but might be surprised out often this is the problem (especially when starting out). Use the `tab` auto-complete features where possible or the old copy-and-paste usually works.
- Closing Punctuation
    - Don't forget to close any parentheses, bracket, or quotation if you use them. 

#### Searching the web

As you navigate the world of code let me introduce you to your new bestfriend...[Stack overflow][stackoverflow]. An excellent resource to find help on error messages for new and experienced users alike!

Everybody – beginner and expert alike – will Google how to code something at some point. The real skill that experts have over beginners is that experts know how to strategically Google. For that, you want to master these skills:

- Make sure that your question is specific and reproducible.
- Don’t forget to include the language/tool you are using e.g. "git".
- Remove text which is specific to you (i.e. the name of your repository or file). 


:::::: discussion

### Searching an error message

You received the following error message and wanted to find help on the web. 
What parts would you put into a search engine?

```error
From https://github.com/siobhon-egan/planets
   1e7a65e..2b65923  master     -> origin/master
error: Your local changes to the following files would be overwritten by merge:
	myNewFile.sh
Please commit your changes or stash them before you merge.
Aborting
```
:::::: 

:::::: solution

- Including the first two lines of the output in the search won't help, as the repository URL and commit log ID are unique to me. 
- The third line (`error: Your local changes to the following files would be overwritten by merge:`) tell us the type of error encountered here. This is probably going to be the most helpful to enter into a search engine.
- The fourth line is just the name of my new file in the directory and won't be helpful.
- The fifth line explains how to fix the error, but you may not know exactly the steps to do this. Searching for help on this line might also retrieve some useful tips
- Searches for the final line (`Aborting`) probably won't yield many useful results.

:::::: 


---


:::::: keypoints

 - Keep a copy of GitHub cheat-sheet handy when starting out. [*PDF copy*](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)
 - [GitHub Docs pages](https://docs.github.com/en) is your go-to for extensive documentation.
 
::::::
