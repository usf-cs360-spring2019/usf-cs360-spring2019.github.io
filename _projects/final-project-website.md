---
title: Final Project Website
navbar: Guides
layout: guides
key: 6.6

tags:
  - text: 'Due 05/16'
    type: 'is-danger'

blurb: |
  <p>
    The primary deliverable for the final project will be the final project website.
  </p>

assignments:
  - text: Final Release
    info: (Canvas Assignment)
    link: https://usfca.instructure.com/courses/1582982/assignments/6829968

  - text: Extra Credit
    info: (Canvas Assignment)
    link: https://usfca.instructure.com/courses/1582982/assignments/6823756

---

{% include section.html level="h2" name="Website Content" %}

The **final release** of this website must contain the following pages and information:

  - **Home Page:** Include a home/landing page that clearly describes the overall narrative, optionally includes the demonstration video, and links to the other required content. Specifically:

    - Describe the **overall narrative, goal, story, or theme** of the project. Usually this includes what you hoped to learn by visualizing this dataset. Each visualization might have its own individual goal, but it must be relevant to the overall narrative stated here.

    - *Optionally* embed your **demonstration video** on the main page. See this guide on <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content">embedding video content</a> for details.

    - Provide clear **navigation** to all of the other required content.

  - **About Page:** Include an about page/section that describes your profile and motivation behind this project. Specifically:

      - Include your name, including at least **first name** or nickname, *optionally* last name.

      - Include your **profile photo** (should be professional, but can still be fun).

      - Include your **biography**, including major/minor, expected graduation year, and *optionally* a personal tidbit.

      - *Optionally* include links to your **professional social media accounts** (Github, Linkedin, etc.).

      - Include a paragraph explaining **why you chose this dataset**. For example, is the topic a passion of yours? Does it have personal significance? Were you inspired by something? This is different from the overall narrative, which often describes what you are trying to learn from this dataset instead of why you chose this dataset in the first place.

  - **Data and Processing:** Include a SEPARATE page that describes the dataset and initial processing done to that data. Specifically:

    - Include **proper attribution** for the original dataset. You will need to look at the original dataset page for how to give proper attribution. This should include a **link to the dataset**!

    - Include the **license** for the original dataset. You need to choose a dataset with a **permissive license** that allows you to process and use that data. See [opensource.org](https://opensource.org/licenses) or [choosealicense.com](https://choosealicense.com/licenses/) for example licenses.

    - Include the **size** of the original dataset, giving the number of columns, rows, and file size where appropriate. If the dataset does not have a fixed number of rows, try to still give estimates. For example, "This dataset had <code>[n]</code> rows as of <code>[date]</code>."

    - Describe the **content** of the original dataset, giving descriptions (or better yet, distribution visualizations) of all the relevant columns. That should include the data types of these columns, the possible values for categorical data, or the range of values (and possibly other simple statistics) for numerical columns.

    - Describe the **initial processing** done to the original dataset. For example, if you filtered the data by date before downloading, give those details here. Do not include any per-visualization data processing here (that should be included on the visualization's page instead).

      Include enough detail that this process is **repeatable** by someone starting with the original dataset. If no initial processing is done, state as much! Otherwise, you may lose points for missing content.

  - **Visualizations:** See the [visualization guidelines](#visualization-guidelines) below for details on the visualizations. For each dedicated visualization page, the following must also be included:

    - Detail the **data encoding** and how to interpret your visualization.

    - Detail **how to interact** with the visualization.

    - Detail one or two **findings** that can be learned with your visualization.

  - **Feedback:** Include a SEPARATE page to discuss the feedback you received. Specifically:

    - Include the **original prototype(s)** from your beta release that you received feedback on.

    - Include the **feedback you received**. Be specific, refer to specific evaluation criteria (lie factor, data ink ratio, data density, etc.) and include anonymized quotes and specific ratings if possible.

    - Include how this feedback **affected the final versions** of the visualizations included in your project. For example, did you make slight modifications or end up trying a different encoding entirely?


Overall, you should have an informative professional website that you are proud of and want to show off to your friends, family, and future employers.

Double-check all of the required content is included in your final release. See the [alpha release](final-project-alpha.html) and [beta release](final-project-beta.html) sections for what must be included in the other releases.

{% include section.html level="h2" name="Visualization Guidelines" %}

These are basic guidelines for the visualizations you should include with your project. You will have to choose what works best for your specific dataset. These guidelines can be summarized as follows:

  > Make something *awesome*.

This guideline can be broken down as follows:

  - "Make" means you, individually, should come up with customized visualizations for your dataset. You can start with inspirations and posted examples, but the end result must represent customized individual contributions for your data!

      To be explicit, plugging in your data into someone else's code without making any modifications DOES not qualify. This includes code provided as part of lecture.

  - "Something" refers to at least one advanced visualization (e.g. multidimensional visualizations like parallel coordinates, heatmaps, or scatterplot matrices, geographic visualizations like choropleths and symbol maps, or graph visualizations) created in D3 version 5.

      You may provide additional visualizations using any tool you prefer for additional awesomeness. Aim for *at least* 3 distinct perspectives of your data.

  - "Awesome" refers to visualizations that are highly interactive (e.g. a mix of details on demand, linked views, brushing, filtering, sorting), have strong data encodings, lots of context, high data-ink ratio, high data density, low lie factor, and are well-designed and aesthetically pleasing.

Your final project represents a multi-week iterative effort to produce something awesome. This should involve significantly more work than any individual homework assignment or presented in any individual lecture.

{% include section.html level="h2" name="Grading" %}

The instructor will grade the final release of the project website. The final project will be graded not just on whether you meet the core requirements, but also how well you meet or exceed those requirements. Specifically:

| Letter | Description |
|:------:|:------------|
| F | The website and/or visualizations do not meet the minimum requirements. |
| D | The website and/or visualizations meet the minimum requirements but fail to be informative, interactive, or professional. |
| C | The website and/or visualizations meet the minimum requirements and are informative, interactive, and professional. |
| B | The website and/or visualizations exceed the minimum requirements and are *highly* informative, interactive, and professional. |
| A | The website and/or visualizations exceed the minimum requirements and are *highly* informative, *highly* interactive, and professional. |

Keep in mind the **entire website** will be considered, not just the visualizations.

{% include section.html level="h2" name="Submission" %}

The website final release is due on <strong>May 16 at 12:15pm</strong>. You must [submit a link in Canvas](https://usfca.instructure.com/courses/1582982/assignments/6829968) to a [release of your website repository](https://help.github.com/articles/creating-releases/) before the deadline. Name the release using the pattern `v1.0.x` where `x` starts at `0` and is incremented each time you make another release before the deadline.

You are welcome to continue making changes to your website repository after the deadline, but those changes will *not* be considered for your final grade.

{% include section.html level="h2" name="Extra Credit" %}

You may earn up to 10 points extra credit by signing up for an appointment at the Writing Center to improve the discussions on your final project website. See [the Canvas assignment](https://usfca.instructure.com/courses/1582982/assignments/6823756) for more details.
