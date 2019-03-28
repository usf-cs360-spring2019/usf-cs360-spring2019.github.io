---
title: Homework 3
navbar: Guides
layout: guides
key: 2.3

assignments:
  - text: Homework 3
    link: https://usfca.instructure.com/courses/1582982/assignments/6821958

  - text: Homework 3 Feedback
    link: https://usfca.instructure.com/courses/1582982/assignments/6821978

blurb: |
  <p>
    For this homework assignment, you must visualize data from the <a href="">SF Tree Maintenance March 2018 to March 2019</a> dataset using a geospatial data visualization technique in D3 <strong>version 5</strong>. The techniques allowed for this homework include: non-proportional symbol map, proportional symbol map, or choropleth map.
  </p>

  <p>
    This guide details the requirements for this homework assignment. See the <a href="homework-submission.html">Homework Submission</a> and <a href="homework-feedback.html">Homework Feedback</a> guides for other requirements.
  </p>
---

{% include section.html level="h2" name="Dataset" %}

Students must visualize a filtered view of the [SF 311 Cases](https://data.sfgov.org/City-Infrastructure/311-Cases/vw6y-z8j6) dataset. The dataset has been filtered to focus only on "Tree Maintenance" cases from March 1, 2018 to March 1, 2019. Entries with missing location data have been filtered out.

The dataset can be viewed and downloaded from:

<https://data.sfgov.org/d/nm7r-4cxx?category=City-Infrastructure&view_name=Tree-Maintenance-March-2018-to-2019>

Note there are some transferred, canceled, duplicated, or invalid cases included. If interested, filtering those out requires parsing the unstructured "Status Notes" text field. It is not required, however.

{% include section.html level="h2" name="Boundaries" %}

You should show district or neighborhood boundaries (or a mix) no matter which visualization technique you choose.

The supervisor district boundaries can be downloaded at:

<https://data.sfgov.org/Geographic-Locations-and-Boundaries/Current-Supervisor-Districts/8nkz-x4ny>

The police district boundaries can be downloaded at:

<https://data.sfgov.org/Public-Safety/Current-Police-Districts/wkhw-cjsf>

The dataset uses SF Find neighborhood names. Those boundaries are located at:

<https://data.sfgov.org/Geographic-Locations-and-Boundaries/SF-Find-Neighborhoods/pty2-tcw4>

All the boundary files may be exported in GeoJSON format.

{% include section.html level="h2" name="Grading" %}

<article class="message is-danger">
  <div class="message-body">
    You <strong>must</strong> use D3 version 5 for this assignment to earn a passing grade.
  </div>
</article>

The grade for this homework will be broken down as follows:

| Letter | Requirement |
|:------:|:------------|
| `D` | A visualization in any other tool or language than D3v5. |
| `C` | A static visualization in D3v5 with a projected district or neighborhood base map. |
| `B` | C-level requirements plus details-on-demand interactivity. |
| `A` | B-level requirements plus either zoom, filter, or brush interactivity. |

The geospatial visualization techniques allowed for this homework include: non-proportional symbol map, proportional symbol map, or choropleth map. Only one technique must be implemented. You are welcome to prototype your technique using any tool, but it is not required.

See the requirements below and the [Homework Grading](homework-submission.html#grading) section for more details.

{% include section.html level="h2" name="Requirements" %}

Create one image (or SVG) visualization. The visualization should be no more than 960 pixels wide and should be at least 500 pixels tall.

See below for the detailed requirements for each letter grade level.

{% include section.html level="h3" name="Base Level Functionality" %}

The base letter grade will be determined as follows:

  - **D Level:** Visualize the dataset **including** a basemap with either the SF Supervisor Districts or SF Find Neighborhood boundaries using one of the following techniques:

    - **Non-Proportional Symbol Map:** This option should show the location of every individual request made. You should encode an additional piece of *categorical* information using color. For example, you can color by the "Source", "Request Type", "Status", or "Responsible Agency" columns. Also, consider how to use shape, stroke, and opacity of the symbols effectively.

    - **Proportional Symbol Map:** Nest and rollup the data by either district or neighborhood, and visualize a numerical value using the size of each symbol. Choose the appropriate underlying boundary map based on your choice. You will also need to calculate the "center" of that region to place each the symbol. You should be able to use [d3.geoCentroid()](https://github.com/d3/d3-geo/blob/master/README.md#geoCentroid), but it might be easier to just find the [bounding box](https://bl.ocks.org/mbostock/1160929) for a region and calculate the center pixel location.

    - **Choropleth Map:** Nest and rollup the data by either district or neighborhood, and visualize a numerical value using fill color for that region. Choose the appropriate underlying boundary map based on your choice. Consider what color scales make the most sense for your data, and whether to use a threshold scale or linear scale.

    Choose whichever technique you are more interested in---all are worth the same amount of points.

  - **C Level:** Implement the D-level functionality in D3 **version 5**.

  - **B Level:** Complete the C-level functionality and implement details-on-demand interactivity. For example, show details when the mouse hovers over a region and/or symbol. You should implement this in base D3---please do not use a tooltip library. Your details should be readable and informative. Think about which details will be useful, and adjust the formatting of the text as appropriate.

  - **A Level:** Complete the B-level functionality and implement either (1) zooming and panning, (2) filtering, or (3) brushing. You only need to choose one of these, but it should be on top of the details-on-demand interactivity implemented for B-level functionality.

    **Zooming and panning** will work with any visualization type, but can be tricky to properly scale the size of symbols. For **brushing or filtering**, you will need to be creative. You should choose a column in the dataset with semi-categorical information (or a date/time column), and then how you want to control which information is brushed/filtered. You could add a linked visualization to control what information is brushed or filtered, or add HTML form controls to your page to control this. Alternatively, if you use a **non-proportional symbol** map, you could brush/filter other points based on a characteristic of a clicked symbol. For example, if you clicked on a symbol that was opened in April, you could brush all other symbols that occurred in April.

    Keep in mind many examples of interactivity are in D3 version 3 or 4, so you may need to figure out how to adapt those examples for version 5.

See the details below for how minus, normal, and plus letter grades will be assigned.

{% include section.html level="h3" name="Plus/Minus Functionality" %}

The base level functionality will determine whether you earn an A, B, C, or D base letter grade. However, the following will determine whether you earn a minus, normal, or plus letter grade.

To earn a **minus letter grade** (D-, C-, B-, or A-):

  - Properly submit a visualization on time meeting the minimum requirements.

  - Include a 1 paragraph (3-5 sentence) writeup about how to interpret your visualization.

To earn a **normal letter grade** (D, C, B, or A), you must complete the minus requirements above and:

  - Include the context necessary to interpret your visualization, including color and/or size legends, titles, and annotations (if appropriate).

  - Include a 1 paragraph (3-5 sentence) writeup about what you can learn about that data from your visualizations.

To earn a **plus letter grade** (D+, C+, B+, or A+), you must complete the normal and minus requirements above and:

  - Calculate and visualize ratios instead of raw counts. For example, you can calculate the area of a GeoJSON boundary:

      <https://github.com/d3/d3-geo/blob/master/README.md#geoArea>

  - Include 1 paragraph (3-5 sentences) writeup of the ratio and how you calculated it.

The goal is to have a single professional webpage that provides users all the context necessary to understand the data being visualized. Think about a professional blog post, or even a newspaper/magazine article!
