---
permalink: /
title: "Brief introduction of this website"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

This is the home page, pertaining to the brilliant mind of [Caiden Palmer](https://github.com/CodeMaster420ImInsane), that details of his most wonderous adventures through life. [This website](https://codemaster420iminsane.github.io/) is his way of creating a journal of events and also as an exercise of his independent learning. The use of github was chosen to create this website as it sits with all of the creator's most used projects, including his A level computer science project [which you can find here](https://github.com/CodeMaster420ImInsane/Computer-Science-Project). There are a number of tabs that encapsulate the details of my life: projects, talks, jobs, a portfolio, posts, and a dynamically-generated CV. This website does not work with any ads or sponsors and is free to view by anyone.

History of this website
======
The idea for this website first arrived in my frivolous journey when my friend [Benediktas Meidus](https://github.com/NGPY) sent me a link connecting to a website he had made in his own time. A few hours later, on [March 25th 2023](https://www.calendar-365.co.uk/calendar/2023/March.html), I had put together a very basic initial version of the site using Visual Studio Code and Github. The site was made with the combined languages of markdown, Javascript, HTML, and CSS; none of which I understood anything about.

As of the 25th March 2023, I plan to use this site to deploy my CV, create a profile of myself that any employer can view, and to collate anything I need into its own section, but all on this site. I have created hyperlinks to all of my social platforms, included a location, email, profile picture & name, and bio for myself. Perhaps I will create a multi-user version of the site to share to any and all of my acquaintances, including a messaging system to communicate between profiles. Looking at [Discord](https://linuxhint.com/wp-content/uploads/2022/08/How-to-DM-Someone-on-Discord-3.png) for example, you can create groups, initiate calls, and message anyone you have added.

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
