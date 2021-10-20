# How to edit the content of this website 
(Alternate title: a note for myself in six months when I have to add to this)

## CV
The sections of the CV are implemented as collections.
### Jobs
To add a job, create a file in \_jobs with the front matter:

    ---
    layout: job
    company: 
    title: 
    employment-date: 
    priority: 
    show:
    ---

`priority` determines what order the jobs will appear in on the CV. Lower numbers appear closer to the top of the page.

Write a description of the job in the main part of the file in markdown.

### Education
To add an education entry, create a file in \_education with the front matter:

    ---
    institution: 
    education-date: 
    degree: 
    show: 
    ---

The CV supports writing a description in the main part of the file and will interpret markdown.

### Projects
This pulls from the projects collection and displays any projects with the attribute `show-in-cv` set to `true`. See a description of the projects collection below.

### Skills
This section is pulled from the skills collection, which has files for different categories of skills. To add a skill to an existing category, add it to the bottom of the file in `_skills/category-name.md`. To add a new category, create a new file in \_skills with the front matter:

    ---
    title: 
    priority: 
    show: 
    ---

## Projects
The projects collection is used to generate a projects page and the projects section of the CV. Create a new project by creating a file in \_projects with the front matter:

    ---
    layout: project
    title:  
    date: 
    categories: 
    description: 
    show: 
    priority: 
    ---

These will be displayed in order of priority on the CV, with lower numbers closer to the top of the page. They will be displayed in reverse chronological order on the projects page, with newer projects closer to the top.
