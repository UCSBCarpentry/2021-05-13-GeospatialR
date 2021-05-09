[![Build Status](https://travis-ci.com/carpentries/workshop-template.svg?branch=gh-pages)](https://travis-ci.com/carpentries/workshop-template)

# The Carpentries Workshop Template

This repository was created from The Carpentries' ([Software Carpentry][swc-site], [Data Carpentry][dc-site], and
[Library Carpentry][lc-site]'s) template for creating websites for workshops.

2. Please *do your work in the repository's `gh-pages` branch*, since that is what is
   [automatically published as a website by GitHub][github-project-pages].

3. Episodes are in the `_epidodes` folder. Edit these directly

The pages on [customizing your website][customization],
the [FAQ][faq],
and the [design notes][design] have more detail on what we do and why.

## Customizing Your Website (Required Steps)

There are two ways of customizing your website. You can either:

- edit the files directly in GitHub using your web browser
- clone the repository on your computer and update the files locally

### Updating the files on GitHub in your web browser

1.  Go into your newly-created repository,
    which will be at `https://github.com/your_username/YYYY-MM-DD-site`.
    For example,
    if your username is `gvwilson`,
    the repository's URL will be `https://github.com/gvwilson/2016-12-01-oomza`.

3.  Ensure you are on the gh-pages branch by clicking on the branch under the drop
    down in the menu bar (see the note below):

    ![screenshot of this repository's GitHub page showing the "Branch" dropdown menu expanded with the "gh-pages" branch selected](fig/select-gh-pages-branch.png?raw=true)

3.  Edit the header of `index.md` to customize the list of instructors,
    workshop venue, etc.
    You can do this in the browser by clicking on it in the file view on GitHub
    and then selecting the pencil icon in the menu bar:


4.  Remove the notice about using the workshop template in the `index.md` file. You can safely
    delete everything between the `{% comment %}` and `{% endcomment %}` (included) as indicated
    below (about from line 35 to line 51):

4.  Edit `_config.yml` to customize certain site-wide variables, such as: `carpentry` (to tell your
    participants the lesson program for your workshop), `curriculum` and `flavor` for the
    curriculum  taught in your workshop, and `title` (overall title for all pages).

    Editing hints are embedded in `_config.yml`,
    and full instructions are in [the customization instructions][customization].

5. Edit the `schedule.html` file to edit the schedule for your upcoming workshop. This file is
   located in the `_includes` directory, make sure to choose the one from the appropriate `dc` (Data
   Carpentry workshop), `lc` (Library Carpentry), or `swc` (Software Carpentry) subdirectory.

