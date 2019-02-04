---
title: Homework 1
navbar: Guides
layout: guides
key: 2.1
bump: true

tags:
  - text: 'Due 2/14'
    type: 'is-danger'

assignments:
  - text: Homework 1 Basic Charts
    link: https://usfca.instructure.com/courses/1582982/assignments/6821944

  - text: Homework 1 Feedback
    link: https://usfca.instructure.com/courses/1582982/assignments/6821976

blurb: |
  <p>
    For this homework assignment, you must visualize the <a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783">SFPD Incidents</a> dataset using various basic visualization techniques using <a href="https://www.tableau.com/academic/students">Tableau Desktop</a> and <a href="https://d3js.org/">D3.js</a>.
  </p>

  <p>
    This guide details the requirements for this homework assignment. See the <a href="homework-submission.html">Homework Submission</a> and <a href="homework-feedback.html">Homework Feedback</a> guides for other requirements.
  </p>
---

{% include section.html level="h2" name="Dataset" %}

Students must visualize the [SFPD Incidents](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783) dataset for the month of December 2018. The exact dataset (with the date filter already applied) can be accessed and downloaded at:

<https://data.sfgov.org/Public-Safety/December-2018/fuj3-tves>

There are 12,214 records in this dataset. Students are encouraged to apply different filters and aggregations to focus on a subset of this data. See the ["Columns in this Dataset"](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783) section of the dataset page for descriptions of the columns.

{% include section.html level="h2" name="Grading" %}

The grade for this homework will be broken down as follows:

| Letter | Requirement |
|:------:|:------------|
| `D` | Prototype **3** unique visualizations in Tableau. |
| `C` | Implement **1** of the Tableau prototypes in D3. |
| `B` | Implement **2** of the Tableau prototypes in D3. |
| `A` | Implement **3** of the Tableau prototypes in D3. |

See the requirements below and the [Homework Grading](homework-submission.html#grading) section for more details.

{% include section.html level="h2" name="Requirements" %}

Create one image (or SVG) per visualization. Each image should be no more than 960 by 500 pixels. Visualizations may be placed on the same webpage or separate webpages. Regardless, the homework website must have clear navigation to each of the visualizations.

See below for the detailed requirements for each letter grade level.

{% include section.html level="h3" name="D Level Functionality" %}

Prototype three different basic visualizations of the dataset using Tableau. Specifically:

  - Create at least **three different visualizations**. This means you need three different sheets in Tableau, and need to export three different images to include on your website.

  - Use at least **two different encodings** from the following list.

      - Encode data using points (e.g. scatter or bubble plot).
      - Encode data using bars (e.g. horizontal bar charts, vertical bars, stacked bars, grouped bars, small multiple bars, and histograms).
      - Encode data using lines (e.g. line charts, multi-series lines, small multiple lines, and slope graphs).
      - Encode data using area (e.g. area chart, stacked area, small multiple area).
      - Encode data using heatmaps or pie charts.

    Encodings belonging to the same item above do not count as different. For example, you may try both a stacked bar and a grouped bar chart, but these do not count as two different encodings in the list above. Therefore the third visualization may *not* use bars to encode data.

    Other encodings must be pre-approved in a **public** [Piazza]({{ site.data.course.piazza }}) post.

  - Use at least **two different perspectives** of the data. This can be achieved by grouping, filtering, or aggregating the data differently. For example, one visualization can use data grouped by weekday and another uses data grouped by category instead.

  - Use **color to encode data** in at least one visualization. This visualization *must* include a color legend in the static image export.

  - Use **titles and axis labels** where appropriate to make sure the encoding is clear. For example, include enough labels so that viewers can tell that category is listed on one axis and count is listed on the other.

  - For each visualization, **include a caption** that includes your name and a brief summary of what you can learn about the data using the visualization.


Export your Tableau visualizations as **static images** and include them on your homework submission website under the "Prototypes" heading. None of the visualizations for this homework assignment need to be interactive.

Use the "Dashboards" feature in Tableau to make sure your images will fit within 960 by 500 pixels and the legend and caption are clearly visible.

{% include section.html level="h3" name="C Level Functionality" %}

Implement one of your Tableau prototypes in D3. Specifically:

  - Use the same visualization technique and data encoding as one of your Tableau Visualizations. <span class="tag is-primary is-rounded">Required</span>

  - Match as much of the design from your Tableau prototype as possible. This includes colors for non-data elements, style of grid lines, tick labels, sort order, and so on. <span class="tag is-rounded is-light">Optional</span>

  - Include the captions, titles, and legends found in your Tableau prototype in your D3 implementation. <span class="tag is-rounded is-light">Optional</span>

You only have to complete the required functionality to satisfy this grade level requirements, but **you must meet the optional requirements before moving on** to the next grade level.

{% include section.html level="h3" name="B Level Functionality" %}

This level has the same requirements as the C level functionality, except for a second Tableau prototype.

As before, you only have to complete the required functionality to satisfy this grade level requirements but **you must meet the optional requirements before moving on** to the next grade level.

{% include section.html level="h3" name="A Level Functionality" %}

This level has the same requirements as the C level functionality, except for a third Tableau prototype.
