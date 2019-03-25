---
title: Homework 2
navbar: Guides
layout: guides
key: 2.2

assignments:
  - text: Homework 2 Multivariate
    link: https://usfca.instructure.com/courses/1582982/assignments/6821957

  - text: Homework 2 Feedback
    link: https://usfca.instructure.com/courses/1582982/assignments/6821979

blurb: |
  <p>
    For this homework assignment, you must visualize data from the "<a href="https://opportunityinsights.org/paper/mobilityreportcards/">Mobility Report Cards: The Role of Colleges in Intergenerational Mobility</a>" project using a multivariate visualization technique in D3.js.
  </p>

  <p>
    This guide details the requirements for this homework assignment. See the <a href="homework-submission.html">Homework Submission</a> and <a href="homework-feedback.html">Homework Feedback</a> guides for other requirements.
  </p>
---

{% include section.html level="h2" name="Dataset" %}

Students must visualize the "Baseline Cross-Sectional Estimates of Child and Parent Income Distributions by College" dataset from the "[Mobility Report Cards: The Role of Colleges in Intergenerational Mobility](https://opportunityinsights.org/paper/mobilityreportcards/)" project from [Opportunity Insights](https://opportunityinsights.org/).

Students are encouraged to look at the material, especially the conclusions of the study, available on the website. Visualizations that conflict with the study conclusions may need close examination.

The exact dataset is the "Baseline Cross-Sectional Estimates of Child and Parent Income Distributions by College" dataset (also referred to as "Online Data Table 2"). The direct links are:

[mrc_table2.csv](https://opportunityinsights.org/wp-content/uploads/2018/04/mrc_table2.csv)  
[Codebook-MRC-Table-2.pdf](https://opportunityinsights.org/wp-content/uploads/2018/04/Codebook-MRC-Table-2.pdf)

Students may choose the rows and columns to focus on in this dataset, but should be visualizing at least 4 columns and approximately 50 or more rows.

{% include section.html level="h2" name="Grading" %}

The grade for this homework will be broken down as follows:

| Letter | Requirement |
|:------:|:------------|
| `D` | Bubble Plot |
| `C` | Normalized Heatmap |
| `B` | Small Multiples -or- Both a Bubble Plot and Heatmap |
| `A` | Parallel Coordinates -or- Scatterplot Matrix |

See the requirements below and the [Homework Grading](homework-submission.html#grading) section for more details.

{% include section.html level="h2" name="Requirements" %}

Create one image (or SVG) per visualization. Each image should be no more than 960 by 500 pixels. Visualizations may be placed on the same webpage or separate webpages. Regardless, the homework website must have clear navigation to each of the visualizations.

See below for the detailed requirements for each letter grade level.

{% include section.html level="h3" name="Base Level Functionality" %}

The base letter grade will be determined as follows:

  - **D Level:** Prototype and implement a bubble chart.

  - **C Level:** Prototype and implement a normalized heatmap. Since the values across columns may have different scales (e.g. percent female ranges from 0 to 1 but parent median income ranges from 21,200 to 226,700), you need to normalize the values in each column. There are different forms of normalization; use [feature scaling](https://en.wikipedia.org/wiki/Feature_scaling) on each column before visualizing on the heatmap.

  - **B Level:** Choose exactly ONE of the following options:

      - Implement a small multiples visualization using any basic visualization technique (like small multiple line charts, small multiple bar charts, etc.) with at least 5 different multiples. The layout in the D3 implementation does not need to 100% match the Tableau prototype (which struggles with laying out multiples in a grid).

      - Implement BOTH a bubble chart or normalized heatmap. In cases of implementing more than one visualization, the minus/normal/plus requirements must be completed for both visualizations. For example, you must add a color legend to both the bubble chart and heatmap to earn a normal letter grade.

  - **A Level:** Choose exactly ONE of the following options:

      - Implement a scatterplot matrix.

      - Implement a parallel coordinates plot. This should be prototyped using [RAWGraphs](http://app.rawgraphs.io/) instead of Tableau.

See the details below for how minus, normal, and plus letter grades will be assigned.

{% include section.html level="h3" name="Minus, Normal, Plus Functionality" %}

The technique you choose will determine whether you earn an A, B, C, or D base letter grade. However, the following will determine whether you earn a minus, normal, or plus letter grade.

To earn a minus letter grade (D-, C-, B-, or A-):

  - Prototype the visualization technique in Tableau, or using [RAWGraphs](http://app.rawgraphs.io/) if implementing parallel coordinates.

  - Implement the prototype in D3, using the same encodings as in the prototype. However, the other non-data elements (such as legends, axis and tick marks, and labels) may differ.

  - Include a 1 paragraph (3-5 sentence) writeup about how to interpret your visualization.

To earn a normal letter grade (D, C, B, or A), you must complete the minus requirements above and:

  - Include axis titles in the D3 implementation.

  - Include legends for the size and color encoding in the D3 implementation (if appropriate).

  - Include a 1 paragraph (3-5 sentence) writeup about what you can learn about that data from your visualizations.

To earn a plus letter grade (D+, C+, B+, or A+), you must complete the normal and minus requirements above and:

  - Carefully annotate and customize your D3 visualization by labeling/highlighting interesting data points.

  - Include a 1 paragraph (3-5 sentence) writeup about the highlighted data points.

The visualizations do *not* need to be interactive.
