# How to edit the content of this website 
## (A note for myself in six months when I have to add to this)

## CV
The sections of the CV are implemented as collections.
### Jobs
To add a job, create a file in \_jobs with the front matter:

`---
layout: job
company: 
title: 
employment-date: 
priority: 
---`

`priority` determines what order the jobs will appear in on the CV. Lower numbers appear closer to the top of the page.

Write a description of the job in the main part of the file in markdown.

### Education
To add an education entry, create a file in \_education with the front matter:

`---
institution: 
education-date: 
degree: 
---`

The CV supports writing a description in the main part of the file and will interpret markdown.

### Projects
This pulls from the projects collection and displays any projects with the attribute `show-in-cv` set to `true`. See a description of the projects collection below.

## Projects
The projects collection is used to generate a projects page and the projects section of the CV. Create a new project by creating a file in \_projects with the front matter:

`---
layout: project
title:  
date: 
categories: 
description: 
show-in-cv: 
priority: 
---`

These will be displayed in order of priority, with lower numbers closer to the top of the page.
