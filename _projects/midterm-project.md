---
title: Midterm Project
navbar: Guides
layout: guides
key: 1

blurb: |
  <p>
    Instead of a midterm exam, all students must complete a midterm group project. This guide details all of the associated requirements for this project.
  </p>

assignments:
  - text: Midterm Project Group
    info: (Canvas Assignment)
    link: https://usfca.instructure.com/courses/1582982/assignments/6822050

  - text: Midterm Alpha Release
    info: (Canvas Assignment)
    link: https://usfca.instructure.com/courses/1582982/assignments/6821963

  - text: Midterm Beta Release
    info: (Canvas Assignment)
    link: https://usfca.instructure.com/courses/1582982/assignments/6821964

  - text: Midterm Prototype Demonstration
    info: (No Submission)
    link: https://usfca.instructure.com/courses/1582982/assignments/6822053

  - text: Midterm Prototype Feedback
    info: (No Submission)
    link: https://usfca.instructure.com/courses/1582982/assignments/6821971

  - text: Midterm Final Release
    info: (Canvas Assignment)
    link: https://usfca.instructure.com/courses/1582982/assignments/6821965

  - text: Midterm Presentation
    info: (No Submission)
    link: https://usfca.instructure.com/courses/1582982/assignments/6821961

---

{% include notice.html type = "is-info" icon = "fas fa-info-circle" text = "While all of these requirements listed here are related to the midterm project, the associated assignments may belong to other categories (such as participation or presentations)." %}

{% include section.html level="h2" name="Groups" %}

The midterm project will be completed in groups of 2 to 4 people from the same section (meaning undergraduate and graduate students may not join the same group). The exact requirements for the midterm project will depend on the number of students in each group.

For details on how to form the groups and submit a group name, see the [Midterm Groups](/guides/projects/midterm-groups.html) guide.

{% include section.html level="h2" name="Dataset" %}

All groups must visualize the following dataset:

  - [SF Fire Department Calls for Service](https://data.sfgov.org/Public-Safety/Fire-Department-Calls-for-Service/nuek-vuh3)

However, each group must decide on a subset (or multiple subsets) of this dataset that will be more manageable in size. There is no exact size requirement; the subset must be big enough to warrant several unique visualizations but not too large to load in the browser or Tableau.

The subset can be selected by focusing on specific categories or aggregating the data. However, it should **support a cohesive theme** that the entire group will integrate into their individual visualizations. This theme could be an overall story that each visualization will support, or a broad question that each visualization will help answer.

Groups are also welcome to find related datasets to the one above that can help augment their visualizations as well.

{% include section.html level="h2" name="Requirements" %}

Each group must produce *at least* one unique interactive multi-component visualization page per person. The individual components on the visualization page should have their interactivity linked. For example, highlighting a category in one component should highlight  that same category in all components.

The visualization techniques can include any of the basic, time series, or multivariate visualization techniques we have discussed thus far in class. This includes: <i class="fas fa-table"></i> **tables** (normal or Bertin-style), <i class="fas fa-grip-horizontal"></i> **heatmaps** (rectangular or circular), <i class="fas fa-chart-bar"></i> **bar charts** (normal, grouped, stacked, 100% stacked, horizontal or vertical, small multiples), <i class="fas fa-chart-line"></i> **line charts** (normal, multi-series, small multiple, slope graphs, rectangular or circular, small multiples), <i class="fas fa-chart-area"></i> **area charts** (normal, stacked, 100% stacked, small multiples, **streamgraphs**, rectangular or circular, **horizon charts**, joyplots), <i class="fas fa-chart-pie"></i> **pie charts** (normal, small multiples, ~~donut charts~~), <i class="fas fa-chart-scatter"></i> **scatterplots** (normal, hexbinning, bubble charts, scatterplot matrices), **parallel coordinates** (rectangular or circular), or **distribution plots** (histograms, boxplots, violin plots, density plots, beeswarm plots, small multiples).

Group communication and coordination will be key. While each visualization page will be worked on individually, the visualizations should complement each other and **support a cohesive theme**. Beyond having a cohesive story or question, the encodings and styles should also be kept as consistent as possible across visualizations. For example, use the same color encoding for categories throughout the entire project.

Keep the required screenspace to view your visualizations within 1440 x 900 pixels. These are just maximums; your visualizations do *not* need to take up that entire space and do *not* need to have that aspect ratio. Your visualizations do *not* need to be responsive to the browser size.

This is in addition to the other pages required for the midterm project website. This includes a dataset page, which will also include simple visualizations. See the [Midterm Website](/guides/projects/midterm-website.html) guide for additional details.

{% include section.html level="h2" name="Prototypes" %}

Each group must submit several prototypes before their final release of their projects. This includes an [alpha release](https://usfca.instructure.com/courses/1582982/assignments/6821963) and [beta release](https://usfca.instructure.com/courses/1582982/assignments/6821964). Groups will give each other feedback on the prototypes in the beta release on Tuesday 3/5 and Thursday 3/7.

See the [Midterm Prototypes](/guides/projects/midterm-prototypes.html) guide for additional details.

{% include section.html level="h2" name="Website" %}

The midterm project websites must include a rich page describing the data subset selected (and any processing performed), a team page with photos and bios of each team member, a prototypes page illustrating the development of the final visualizations, and one visualization page per team member (as described in the requirements section).

Each group must [submit a final release](https://usfca.instructure.com/courses/1582982/assignments/6821965) of their professional project website showcasing their visualizations before class on Tuesday 03/19. All groups must meet this deadline regardless of when they are presenting.

See the [Midterm Website](/guides/projects/midterm-website.html) guide for additional details.

{% include section.html level="h2" name="Presentation" %}

Each group must present their midterm project in class on week 9 (Tuesday 3/19 and Thursday 3/21). The presentation length must be 5 minutes per person; a 3 person group must present for 15 minutes and a 4 person group must present for 20 minutes. The presentation dates will be semi-randomly assigned by the instructor (taking into account the size of groups and length of presentations).

See the [Midterm Presentations](/guides/projects/midterm-presentations.html) guide for additional details.

{% include section.html level="h2" name="Grading" %}

The instructor will grade the final release of the midterm project websites. The midterm group project will be graded not just on whether you meet the core requirements, but also how well you meet or exceed those requirements. Specifically:

| Letter | Description |
|:------:|:------------|
| F | Reserved for projects that do not meet the minimum requirements. |
| D | Reserved for projects that meet the minimum requirements, but fail to deliver informative visualizations and a professional website. |
| C | Reserved for those projects that meet the minimum requirements, and deliver informative visualizations and a professional website. |
| B | Reserved for those projects that exceed the minimum requirements, and deliver informative visualizations and a professional website. |
| A | Reserved only for those projects that go above and beyond the minimum requirements, and deliver a highly effective visualizations and a well-written professional website. |

Keep in mind the **entire website** will be considered, not just the visualizations. Be as wary of irregular punctuation and poor writing as a misplaced tick mark in your visualizations!
