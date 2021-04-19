# Developer Resources

###### Table of Contents
[Version Control](#vc)

[nanoHub and Tool Development](#nanohub)

[Register as a New Developer on nanoHuB](#nd)

[Ownership, Authorship and Licenses](#owner)

<a name="vc"/>

# Version Control using Git and GitHub

New to GitHub:<br/>
[signing up for a new github account](https://help.github.com/en/articles/signing-up-for-a-new-github-account)<br/>
[student upgrades](https://education.github.com/pack)

These two of the best getting started articles to _git_ you up and running:

[https://help.github.com/articles/set-up-git/](https://help.github.com/articles/set-up-git/)

[https://help.github.com/articles/create-a-repo/](https://help.github.com/articles/create-a-repo/)

The first two chapters of the Pro Git book is certainly one of the best introductions to using Git:

[https://git-scm.com/book/en/v2](https://git-scm.com/book/en/v2)

For Windows and Mac users, you might consider using GitHub's Desktop app.  This is a good choice if you want to maintain a working copy (clone) of a repository natively on a Windows PC or Mac using a GUI.

[https://desktop.github.com](https://desktop.github.com/)

and

[The GitHub Desktop User Guide](https://help.github.com/desktop/guides/getting-started-with-github-desktop/)

<a name="nanohub"/>

or [VSCode](https://code.visualstudio.com/).

## Editing Markdown Documents
Below is a link to one of the best maredown resources, GitHub's own markdown documentation:

[mastering markdown](https://guides.github.com/features/mastering-markdown/)

Below are more tips and tricks...

### Adding images to GitHub Markup Documents
A nice trick to include images in a markup document is to use the [image attachment feature for issues](https://help.github.com/en/articles/file-attachments-on-issues-and-pull-requests).  Any issue will do, as the image does not have to be embedded there.
* Pick an issue or open on in your repo.  
* Drag the image into to the edit window to geneare an anonymized url which can then be pasted in and `*.md` file in the repository
  - An example image tag will look like: `<img width="600" alt="Screen Shot 2019-05-13 at 7 28 51 PM" src="https://user-images.githubusercontent.com/12611210/57662580-b3591180-75b5-11e9-83a5-e043848f46a9.jpg">`


## Handling Jupyter Notebooks with Git

Jupyter notebooks are great, but the nice features also lead to some annoying problems when trying to use a traditional version control based on diffs like git.  The problem is that cell output and various meta data are accumulated in the .ipynb file when executing it, so you see differences even if no substantive edits were made to the cells.  Here is a good article for configuring Git to avoid these hassles:

[Making Git and Jupyter Notebooks play nice](http://timstaley.co.uk/posts/making-git-and-jupyter-notebooks-play-nice/)

<a name="zh"/>
<!--
## ZenHub Extensions to Github
Zenhub is a set of extensions to the GitHub platform that add project management features such as:
* Epics
* Multi-repo boards
* Reports

Contact this nanoMFG GitHub Organization to request ZenHub extension access for your team. 

#### Accessing ZenHub
There are two ways to access ZenHub features:
* On GitHub itself via [browser extension](https://www.zenhub.com/extension)
* Via [app.zenhub.com](app.zenhub.com)

The Firefox/chrome browser extension will add a ZenHub tab to your repositories and allow Epics to be rendered directly when viewing issues on gitHub.

#### ZenHub Basics

* [Create an Epic](https://www.zenhub.com/guides/getting-started-with-epics-in-zenhub#creating-epics-in-zenhub)
* [Create a multi-repo board](https://www.zenhub.com/guides/creating-a-multi-repo-board)
-->
<a name="nanohub">
# NanoHub Links

<a name="nd"/>
### New Developers
[Register](https://nanohub.org/register/)<br/>
* Note: It is better to create a full login/username rather than using the institutional login.  Usernames can be added to an institutional account, but it is good to have one from the beginning as a developer.<br/>
[Submit a ticket]() to request developer access to the "workspace", e.g:
> Hi, I am working on a application in collaboration with the nanoMFG node.  I would like to request access to the developer workspace.


### Instructional Links

 [Tool Development](
https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=5&ved=0ahUKEwirlPLmldPaAhUq0oMKHbH9BOAQFghFMAQ&url=https%3A%2F%2Fhelp.hubzero.org%2Fdocumentation%2F220%2Ftooldevs%3Faction%3Dpdf%26children%3D1&usg=AOvVaw0bLi0aG4sqWCS5yMXXtAAY)
[Jupyter Examples](https://nanohub.org/resources/jupyterexamples)

### Unix Linux

### Rappture

[Rappture Bootcamp Tutorial](https://nanohub.org/resources/14671#series)

In particular these sections:

[1.1 Introducing the Rappture Tookit](https://www.youtube.com/watch?time_continue=1577&v=2g7lgOr8SJ4)

[1.3: Introduction to Scientific Programming in MATLAB](https://www.youtube.com/watch?time_continue=3&v=0NHazC8_MBg)

[1.4: Adding Rappture to MATLAB Applications](https://www.youtube.com/watch?time_continue=693&v=GykLDQfw8G8)

Covers the basics of running Matlab or Octave code on nanoHub.  Covers writing .m files and functions, input output Rappture etc.

### Jupyter notebooks

[jupyter notebook tutorial](https://www.youtube.com/watch?v=5wJ9yz8iV2c)

## Example Tools:
 
[https://nanohub.org/topics/MaterialScienceSimulationTools](https://nanohub.org/topics/MaterialScienceSimulationTools)

[https://nanohub.org/tools/rtdnegf](https://nanohub.org/tools/rtdnegf)

[https://nanohub.org/tools/crystal_viewer](https://nanohub.org/tools/crystal_viewer)

<a name="owner" />

# Ownership authorship and Licensing

[Commonly used licenses](https://opensource.org/licenses)

[UofI OTM Student Ownership Policies](http://otm.illinois.edu/disclose-protect/student-ownership-policy)

<a name="python" />

# Python

[PEP 8 style guide](https://www.python.org/dev/peps/pep-0008/#function-and-variable-names)

[Style guide for testing](https://jrsmith3.github.io/python-testing-style-guidelines.html)


## Templates

[Make *code* repo public](https://github.com/nanoMFG/GSA-Raman/issues/10)

[Register Skeleton Tool on nanoHub](https://github.com/nanoMFG/GSA-Raman/issues/14)
