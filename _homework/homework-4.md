---
title: Homework 4
navbar: Guides
layout: guides
key: 2.4

assignments:
  - text: Homework 4
    link: https://usfca.instructure.com/courses/1582982/assignments/6821959

  - text: Homework 4 Feedback
    link: https://usfca.instructure.com/courses/1582982/assignments/6821977

tags:
  - text: 'Due 04/25'
    type: 'is-danger'

blurb: |
  <p>
    For this homework assignment, you must visualize the data from the <a href="https://data.sfgov.org/Public-Safety/Fire-Department-Calls-for-Service/nuek-vuh3">Fire Department Calls for Service</a> dataset using hierarchical data visualization techniques in D3 version 5. You must perform some data wrangling for this assignment to transform the data into a hierarchical format.
  </p>

  <p>
    This guide details the requirements for this homework assignment. See the <a href="homework-submission.html">Homework Submission</a> and <a href="homework-feedback.html">Homework Feedback</a> guides for other requirements.
  </p>
---

{% include section.html level="h2" name="Dataset" %}

The <a href="https://data.sfgov.org/Public-Safety/Fire-Department-Calls-for-Service/nuek-vuh3">Fire Department Calls for Service</a> dataset can be viewed and downloaded from:

<https://data.sfgov.org/Public-Safety/Fire-Department-Calls-for-Service/nuek-vuh3>

However, the dataset is not hierarchical. Students must decide how to form a hierarchy from this dataset such that:

  - The hierarchy must have height 3 or higher (i.e. at least 3 levels, including root and leaves).

  - Each leaf node must have an attribute associated with it.

This hierarchy could be formed using dates (year, month, day), regions (supervisor district, zip code, etc.), and categories (call type group, call types, etc.). Node attributes could be the count of unique incident numbers associated with the node, average or median response time, and so on. It also looks like the [SF zip code](https://data.sfgov.org/Geographic-Locations-and-Boundaries/San-Francisco-ZIP-Codes/srq6-hmpi) boundaries dataset has population and area information associated with each zip code, which can be used to calculate per-capita or per-square mile metrics.

Any tool or language may be used to wrangle the dataset, including the SF Data interface itself. Specifically, students can use the "Filter" &raquo; "Sort &amp; Roll-Up" &raquo; "Roll-Ups &amp; Drill-Downs" functionality to start building a hierarchy from the dataset.

Students should also filter the data, but the exact filter depends on the hierarchy formed. For example if the hierarchy is formed by region or category, it might make sense to filter by date. However, if the hierarchy is formed by date, then it might make sense to filter by region or category.

{% include section.html level="h2" name="Grading" %}

The grade for this homework will be broken down as follows:

| Letter | Requirement |
|:------:|:------------|
| `D` | Data wrangling into a hierarchical format. |
| `C` | D-level requirements plus implement one node/link diagram in D3v5. |
| `B` | C-level requirements plus implement one space filling or enclosure visualization in D3v5.  |
| `A` | B-level requirements except one technique must use polar coordinates. |

See the requirements below and the [Homework Grading](homework-submission.html#grading) section for more details.

{% include section.html level="h2" name="Requirements" %}

Create one image (or SVG) visualization. The visualization should be no more than 960 pixels wide (maximum) and should be at least 500 pixels tall (minimum).

See below for the detailed requirements for each letter grade level.

{% include section.html level="h3" name="Base Level Functionality" %}

The base letter grade will be determined as follows:

  - **D Level:** Successfully wrangle the data into a hierarchical format that can be interpreted by either [d3.hierarchy()](https://github.com/d3/d3-hierarchy#hierarchy) or [d3.stratify()](https://github.com/d3/d3-hierarchy#stratify). The hierarchy must have height 3 or more (i.e. at least 3 levels including the root and leaf nodes) and each leaf node must have an attribute.

  - **C Level:** Complete the D-level functionality and implement a node link visualization using [d3.cluster()](https://github.com/d3/d3-hierarchy#cluster) or [d3.tree()](https://github.com/d3/d3-hierarchy#tree) and any edge layout/style. The node attribute must be encoded somehow (i.e. using color, size, shape, etc.). Nodes must have a minimum details-on-demand interactivity showing the node label.

  - **B Level:** Complete the C-level functionality and implement a space-filling or enclosure visualization using [d3.partition()](https://github.com/d3/d3-hierarchy#partition), [d3.treemap()](https://github.com/d3/d3-hierarchy#treemap), or [d3.pack()](https://github.com/d3/d3-hierarchy#pack). The node attribute must be encoded somehow (i.e. using color, size, shape, etc.). Nodes must have a minimum details-on-demand interactivity showing the node label.

  - **A Level:** Complete the B-level functionality and implement at least one technique using polar coordinates. The allowable techniques are: a radial/circular dendogram, a radial/circular traditional tree layout, or a sunburst. (Circle packing does *not* use polar coordinates.)

See the details below for how minus, normal, and plus letter grades will be assigned.

{% include section.html level="h3" name="Plus/Minus Functionality" %}

The base level functionality will determine whether you earn an A, B, C, or D base letter grade. However, the following will determine whether you earn a minus, normal, or plus letter grade.

To earn a **minus letter grade** (D-, C-, B-, or A-), you must complete **ALL** of the following:

  - Properly submit a visualization on time meeting the minimum requirements.

  - No matter which technique is used, nodes must have a minimum details-on-demand interactivity showing the node label.

  - Include a 1 paragraph (3-5 sentence) writeup about how to interpret your visualization.

To earn a **normal letter grade** (D, C, B, or A), you must complete the minus requirements above and **ALL** of the following:

  - Include the context necessary to interpret your visualization, including color and/or size legends, titles, and annotations (if appropriate).

  - When hovering over a node in a node/link visualization, highlight or brush the nodes and the edges that form the shortest path to the root node.

  - Include a 1 paragraph (3-5 sentence) writeup about what you can learn about that data from your visualizations.

To earn a **plus letter grade** (D+, C+, B+, or A+), you must complete the normal and minus requirements above and **ONE** of the following:

  - Automatically label nodes if space is available.

  - Add advanced interactivity, such as filtering, collapsing, or zooming. See the [d3-hierarchy notebook collection](https://observablehq.com/collection/@d3/d3-hierarchy) for examples. It is allowable to use HTML form controls for this interactivity.

The goal is to have a single professional webpage that provides users all the context necessary to understand the data being visualized. Think about a professional blog post, or even a newspaper/magazine article!
