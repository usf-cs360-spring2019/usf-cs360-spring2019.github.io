---
title: Homework Submission
navbar: Guides
layout: guides
key: 1.1

assignments:
  - text: Homework 1
    info: (Writeup)
    link: homework-1.html

  - text: Homework 2
    info: (Writeup)
    link: homework-2.html

  - text: Homework 3
    info: (Writeup)
    link: homework-3.html

  - text: Homework 4
    info: (Writeup)
    link: homework-4.html

blurb: |
  <p>All homework assignments will follow the same process for submission. See also the <a href="homework-feedback.html">Homework Feedback</a> guide.</p>
---

{% include section.html level="h2" name="Setup" %}

Homework websites **must** be created by using the Github Classroom links provided. Websites hosted anywhere else or created in any other way will not be accepted.

To setup the repository initially:

  1. Click the Github Classroom link provided in the associated Canvas assignment. This will create a base repository already setup for use with Github Pages. The Github repository will be located at:

      ```
      https://github.com/usf-cs360-spring2019/homework#-username/
      ```

      Note repository links always start with `github.com`, followed by the class organization `usf-cs360-spring2019`, followed by the `homework` preface and homework `#` (either `1`, `2`, `3`, or `4`), and end with `username` (your Github username).

      Keep in mind repositories and their resulting websites are **public** when creating commit messages and commenting your code.

  2. Verify you are able to access the Github Pages website associated with your homework repository. The Github Pages repository will be located at:

        ```
        https://usf-cs360-spring2019.github.io/homework#-username/
        ```

        Note repository links always start with the class organization `usf-cs360-spring2019` followed by `github.io`, followed by the `homework` preface and homework `#` (either `1`, `2`, `3`, or `4`), and end with `username` (your Github username).

  3. Clone the repository locally, and verify you are able to commit and push changes. Commit your work often; not only is it good practice but it also allows you to defend against any cheating allegations.

See the [Getting Started with D3.js](/guides/general/getting-started-with-d3js.html) guide for more details on using Github Pages.

{% include section.html level="h2" name="Submission" %}

Once you have created your homework website, you should **immediately** submit a link to your homework website on [Canvas]({{ site.data.course.canvas }}).

**Double-check you submitted the correct link.** It should be the `github.io` link to your website, **not** the `github.com` link to your repository. Other students will use this link to provide peer feedback on your visualizations and website; they will not comment on your code and do not need your repository link.

{% include notice.html type = "is-info" icon = "fas fa-info-circle" text = "You can continue working on your website after submitting the link as long as it is still before the homework deadline." %}

{% include section.html level="h3" name="Late Policy" %}

Late homework website submissions are not accepted. Your homework will still be graded even if you forget to submit your website on Canvas on time. However, this will severely impact your [Homework Feedback](homework-feedback.html) grade.

Do **NOT** commit to your `gh-pages` branch after the deadline. If you want to keep working on your visualizations for personal gain (not course credit), do so in a fork or different branch. Only commits to your repository **before** the deadline will be considered when grading the homework assignment, and any commits made after the deadline may result in heavy point deductions (up to 100% of the homework grade).

{% include section.html level="h2" name="Grading" %}

Each homework assignment has a letter grade breakdown detailing the functionality required for a `D`, `C`, `B`, and `A` letter grade. In general, homework assignments are designed such that achieving a `D-` to `D+` requires minimal effort, `C-` to `C+` requires some effort, `B-` to `B+` requires moderate effort, and `A-` to `A+` requires significant effort.

Credit for higher letter grades cannot be earned until all of the functionality for the lower grades is fully implemented. For example, the `D` level functionality must be fully implemented before credit may be earned for `C` level functionality.

The teacher assistants have leeway to assign a `+` or `-` grade depending on whether the assignment was submitted properly and how well students completed the required functionality. For example, if a student completes `B` level functionality, the TAs will determine whether that student earned a `B-`, `B`, or `B+` letter grade. In some cases, specific items will be proposed for earning a `+` grade for a specific letter grade.

Keep in mind that the final grade in this class must be a `D` or above to receive credit for most non-major undergraduate students, must be `C` or above for undergraduate students in CS, and must be `B` or above for graduate students in CS.
