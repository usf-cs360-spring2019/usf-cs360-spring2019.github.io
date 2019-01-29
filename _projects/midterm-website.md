---
title: Midterm Website
navbar: Guides
layout: default
key: 4
---

Instead of a midterm exam, all students must complete a midterm group project. This guide explains the requirements for the midterm project website. See the [Midterm Project](/guides/projects/midterm-project.html) page for more details on other requirements.

{% include section.html level="h2" name="Website Content" %}

The primary deliverable for the midterm project will be the midterm project website. The final release of this website must contain the following pages and information:

  - **Home Page:** Include a home/landing page that clearly describes the theme chosen by the midterm project group, and provides navigation to all of the other required pages.

  - **Data and Processing:** Include a page that describes the dataset and processing/wrangling done to that data. Specifically:

      - Discuss and provide proper attribution for the original dataset. You will need to look at the original dataset page for how to give proper attribution.

      - Discuss the processing done to the original dataset. Include enough detail that this process is **repeatable** by someone starting with the original dataset. This could involve publishing a code snippet!

      - Discuss the processed data that is used by the visualizations. If you have multiple versions or subsets used by different visualizations, make sure to describe each one.

    When describing data, make sure to include how many rows and columns are in the dataset, the data types of each column, and the range of values for each column. Simple distribution visualizations (e.g. histograms, violin/box plots) will be really helpful here!

  - **Visualizations:** Include one multi-component visualization page per group member. See the [Midterm Project](/guides/projects/midterm-project.html#requirements) page for more details.

  - **Prototypes:** Include a page about the visualization prototypes. This can include links to your alpha and beta releases, static images demonstrating early drafts of your visualizations, as well as the feedback you received during the prototype exercise and how that affected the visualizations for the final release.

    Need an example? Check out a [Data Sketches](http://www.datasketch.es/february/) writeup; they discuss and demonstrate the process (including inspirations and discarded ideas) of creating their visualizations.

  - **Team/About:** Include a page that describes your group. This should include:

      - Team names, including at least first name or nickname, *optionally* last name

      - Team profile photos (should be professional, but can still be fun)

      - Team biographies, including major/minor, expected graduation year, and *optionally* a personal tidbit

      - Team contact information, *optionally* including links to social media (Github, Linkedin, etc.)


Each section can be included on the same page, or separate pages linked to from the home page. In either case, include clear navigation to each of the required sections. The writing must be professional.

These requirements are for the **final release** of the project website. Groups must create multiple releases of their project website. See the [Midterm Prototypes](/guides/projects/midterm-prototypes.html) guide for details on what each release requires.

{% include section.html level="h2" name="Website Creation" %}

The midterm group project websites will be hosted using [Github Pages](https://pages.github.com/). This is a little tricky to setup with Github Classroom, so please follow these instructions very carefully!

  1. ONE pre-designated member from each group must first click on the Github Classroom link posted on Piazza.

  2. When prompted **create a new team** using the group name already entered on Canvas. When done, let the other group members know they can move forward.

  3. AFTER the first member has created the team, the rest of the group members must then click the Github Classroom link and then **select the team already created**. Be careful---it is very difficult to undo mistakes at this stage!

This sets up the repository, gives everyone in the team access to that repository, and creates a team on the class Github organization allowing the entire group to communicate.

Once created, the Github repository will be located at:

```
https://github.com/usf-cs360-spring2019/midterm-groupname/
```

The associated Github Pages website will be located at:

```
https://usf-cs360-spring2019.github.io//midterm-groupname/
```

In both, replace `groupname` with your midterm group name.

Since this will be a **shared repository**, groups are strongly recommended to communicate regularly, use [branches](https://help.github.com/articles/about-branches/) while developing, and consider [running your site locally](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/) to test your changes before committing and pushing them live.

{% include section.html level="h2" name="Creating Releases" %}

Each group will have to create multiple [releases](https://help.github.com/articles/about-releases/) of their website, including an [alpha release](https://usfca.instructure.com/courses/1582982/assignments/6821963), [beta release](https://usfca.instructure.com/courses/1582982/assignments/6821964), and [final release](https://usfca.instructure.com/courses/1582982/assignments/6821965). These releases act as checkpoints in the development of your projects, and is a recommended process for any software project. These releases also allow us to grade a specific version of the project website without preventing groups from continuing development during the grading period.  

Follow the [creating releases](https://help.github.com/articles/creating-releases/) guide on Github for exact steps on how to create a new release. The release version should follow this pattern:

| Release | Version | Examples |
|:--------|:-------:|:---------|
| Alpha Release(s) | `v0.1.#` | `v0.1.0`, `v0.1.1`, and so on... |
| Beta Release(s)  | `v0.2.#` | `v0.2.0`, `v0.2.1`, and so on... |
| Final Release(s) | `v1.0.#` | `v1.0.0`, `v1.0.1`, and so on... |

It is only necessary to create multiple releases for each checkpoint if changes were made (before the deadline) that groups want included in the grade. For example, suppose a group creates alpha release `v0.1.0` but discovers a typo before the deadline. That group can create a new alpha release `v0.1.1` and resubmit the link in Canvas.

Made a mistake? DO NOT DELETE RELEASES. Just [edit the release](https://help.github.com/articles/editing-and-deleting-releases/) or create a new release instead.

{% include section.html level="h2" name="Submitting Releases" %}

When submitting releases for grading on Canvas, submit the URL directly to your release on the Github repository at github**.com** (*not* to the Github page at github**.io**). The URL should look like:

```
https://github.com/usf-cs360-spring2019/midterm-groupname/releases/tag/v#.#.#
```

The URL starts with `github.com` and ends with the `v#.#.#` release number (e.g. `v1.0.0` for a final release). Both `groupname` and `v#.#.#` need to be replaced to match the project group and release number.

{% include notice.html type = "is-warning" icon = "fas fa-exclamation-circle" text = "If your URL starts with <code>usf-cs360-spring2019.github.io</code> then you are submitting the wrong link!" %}
