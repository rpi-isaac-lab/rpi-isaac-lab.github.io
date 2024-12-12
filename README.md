# ISAaC Lab Website

Public website for the lab!

This website is forked from [al-folio](https://github.com/alshedivat/al-folio/), which itself is built on Jekyll pages. This allows for the majority of rotating content to be written in simple Markdown. Below, I will outline how students,projects,news updates, and publications can be added to and students may be retired from the site.

NOTE: I have not bothered to update the INSTALL.md and CUSTOMIZE.md files. These are original to the al-folio repo. Once you have jekyll working, then you can proceed to edit the project files.

## Student Pages

Pages for all students, current and former, can be found in the "_people" directory.

- To add a new student: copy the template (in the same directory) and fill in the relevant tags and the bio. The template should be able to walk you through what needs to change. Insert the students picture into the "assets/profiles" directory, and copy the filename into the relevant spot on the tags. If in doubt, look at other students pages as an example.
- To change a student's status: open up the student's file and edit the relevant tag. Common edits will be "category", which should be one of: "PhD", "Masters", and "Undergrad", and "Status", which should be one of "Current", "Former"

## Project Pages

All the lab's projects should have project pages. They are found in the "_projects" directory.

- To add a project: copy the template (in the same directory) and fill in the relevant tags and summary. The template should be able to walk you through what needs to change. Insert the projects images into the "assets/img" directory so that they may be linked from the project page.
- To modify a project: Open the file and make the relevant changes. Common changes will include retiring a project (change the "status" from "current" to "former") and changing the lead researcher as people graduate. Changing the "Lead Researcher" tag will allow the latter. Make sure to double check that all of the links work after this is done. If the name is entered differently than in the student's profile, this will not work.

## News Updates

Prof. Mishra has stated that he wants the news section removed, I just haven't handled that yet. I'll take care of it.

## Publications Updates

This one is the easiest. It's the same as adding sources to a .bib file for LaTeX. Add citations to the "bibliography/papers.bib" file. Try and include as much information as you can. The website is capable of displaying an abstract/publisher/etc. When in doubt, look at other citations already in the file.
