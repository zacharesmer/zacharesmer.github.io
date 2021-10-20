# How to edit the content of this website 
(Alternate title: a note for myself in six months when I have to add to this)

## CV
The sections of the CV are implemented as collections. They all support a `priority` attribute, which is a number that determines how it will be displayed in the CV. Lower numbers are closer to the top. They also all support a `show` attribute, which if set to false means the item will not be shown on the CV page. In the case of projects, a project with `show` set to `false`  will still appear on the project page.
### Jobs
To add a job, copy the `_templates/job.md` file into `_jobs`.

The CV supports writing a description in the main part of the file and will interpret markdown.

### Education
To add an education entry, copy the `_templates/education.md` file into `_education`.

The CV supports writing a description in the main part of the file and will interpret markdown.

### Projects
This pulls from the projects collection and displays any projects with the attribute `show` set to `true`. See a description of the projects collection below.

### Skills
This section is pulled from the skills collection, which has files for different categories of skills. To add a skill to an existing category, add it to the bottom of the file in `_skills/category-name.md`. To add a new category, copy the file `_templates/skill.md` into `_skills`.

## Projects
The projects collection is used to generate a projects page and the projects section of the CV. To create a new project, copy the `_templates/project.md` file into `_projects`.

Projects will be displayed sorted by priority on the CV, with lower numbers closer to the top of the page. They will be displayed in reverse chronological order on the projects page, with newer projects closer to the top, sorted by the `date` attribute. The `show` attribute only affects whether the project is shown in the CV. A project with `show` set to `false`  will still appear on the project page.
