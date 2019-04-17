---
title: Final Project Proposal
navbar: Guides
layout: guides
key: 6.1

assignments:
  - text: 'Project Proposal'
    info: '(Canvas Submission)'
    link: 'https://usfca.instructure.com/courses/1582982/assignments/6821966'

blurb: |
  <p>
    Students setup their final project website repository, as well as identify and describe a dataset for their final project.
  </p>
---

{% include section.html level="h2" name="Repository Setup" %}

The final project websites will be hosted using Github Pages. To get started, use the following Github Classroom link:

  > <https://classroom.github.com/a/7XeIRAw->

Once created, the Github repository will be located at:

```
https://github.com/usf-cs360-spring2019/project-username/
```

The associated Github Pages website will be located at:

```
https://usf-cs360-spring2019.github.io/project-username/
```

In both, replace `username` with your Github username. You do not have to use the template provided; feel free to change it.

{% include section.html level="h2" name="Dataset Selection" %}

Use the [Resources]({{ '/guides/general/resources.html' | relative_url }}) page to identify a dataset. You are encouraged to find a dataset that matches your interests and/or helps support the [mission of the university](https://www.usfca.edu/about-usf/who-we-are/vision-mission).

You need a dataset that is "just right" in size and complexity. It should have a mix of column types (numerical, categorical, date/time, **latitude/longitude**, etc.) and many rows. Some larger datasets can be filtered down to a subset manageable for interactive web visualizations, but avoid any "big data" datasets that require special processing to reduce in size.

Keep in mind you will need to produce somewhere between 3 to 4 distinct, interactive, complex visualizations of your dataset. Make sure you have a rich enough dataset to support that!

{% include notice.html type="is-warning" icon="far fa-hourglass-half" text="You can change your dataset later if it ends up not working out, but you lose a significant amount of time and effort if you switch." %}

{% include section.html level="h2" name="Website Requirements" %}

For the project proposal, you must have drafts of the following sections complete:

  - Create an initial version of the **Home/Landing Page** as required for the final release (*except* for the optional demonstration video).

  - Create an initial version of the **About Page** as required for the final release. Include drafts of all the required sections.

  - Create an initial version of the **Data and Processing Page** as required for the final release. Include drafts of all the required sections.

These do not have to be the final versions of these pages; the content may change later. However, the more work you put in now, the less you will have to do later.

{% include section.html level="h2" name="Submission" %}

The proposal is due on <strong>April 2 at 12:15pm</strong>. You must [submit a link in Canvas](https://usfca.instructure.com/courses/1582982/assignments/6821966) to a [release of your website repository](https://help.github.com/articles/creating-releases/) before the deadline. Name the release using the pattern `v0.0.x` where `x` starts at `0` and is incremented each time you make another release before the deadline.
