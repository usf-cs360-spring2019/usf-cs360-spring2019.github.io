---
title: Data Vis Talk Topics
navbar: Guides
layout: guides
key: 3.1

assignments:
  - text: Data Vis Talk Topic
    info: (Canvas Assignment)
    link: https://usfca.instructure.com/courses/1582982/assignments/6829299

blurb: |
  <p>
    All students must give a 15 minute talk on a topic in data visualization. This guide explains the talk topic requirements. See the general <a href="data-vis-talks.html">Data Vis Talks</a> guide for more details on other requirements.
  </p>

weeks:
  - week: 5
    tues: 2019-02-19
    thur: 2019-02-21
    slots:
    - time: '12:50p'
      tues: 'Animated Representations Help Ambiguous Data' # Jordan A.
      thur: 'Visualizing the Vocabulary of Hip-Hop' # Emmit P.

    - time: '1:10p'
      tues: 'A New Way to Make Charts: Charticulator' # Jiadong W.
      thur: 'Tracking Soccer Movement' # Cristina M.C.

    - time: '1:30p'
      tues: 'A Declarative Rendering Model for Multiclass Density Maps' # Tong W.
      thur: 'Data Visualization for Traveling in Avalanche Terrain' # Enrique B.

    - time: '1:50p'
      tues: 'T-SNE: Visualize High-Dimensional Data' # Xue F.
      thur: "Where's My Data? Evaluating Visualizations with Missing Data" # Gudbrand S.

    - time: '2:10p'
      tues: 'Data Visualization in Medical Research' # Rock G.
      thur: 'The Psychology of Data Visualization' # Sameer I.

  - week: 11
    tues: false
    thur: 2019-04-04
    slots:
    - time: '12:50p'
      thur: 'Visualizing My Favorite TV Shows' # Corianna P.
    - time: '1:10p'
      thur: "Nike Vaporfly's: Do they work?" # Tony J.
    - time: '1:30p'
      thur: 'Building a Connection with Data through Original Visualization' # Darianne L.
    - time: '1:50p'
      thur: 'VR &amp; AR: The Future of Data Visualization' # Samuel E. O.
    - time: '2:10p'
      thur: 'Visualizing the Data Revolution in Sports' # Nicolas O.

  - week: 14
    tues: 2019-04-23
    thur: 2019-04-25
    slots:
    - time: '12:50p'
      tues: 'The Forgotten Horrors: Non Combat Casualties of American Servicemen' # David M.
      thur: 'ATOM: A Grammar for Unit Visualizations' # Diana P.
    - time: '1:10p'
      tues: 'Pioneers of Data Visualization: Fernanda Viégas' # Martha S.
      thur: 'Feature Visualization' # Seyyed M. H.
    - time: '1:30p'
    - time: '1:50p'
    - time: '2:10p'

  - week: 16
    tues: 2019-05-07
    thur: false
    slots:
    - time: '12:50p'
      tues: "Major League Baseball Statistics" # John M.
    - time: '1:10p'
    - time: '1:30p'
    - time: '1:50p'

---

{% include section.html level="h2" name="Approved Topics" %}

<table class="table is-narrow">
  <thead>
    <tr>
      <th>Date</th>
      <th>Time</th>
      <th width="50%">Tuesday</th>

      <th>Date</th>
      <th>Time</th>
      <th width="50%">Thursday</th>
    </tr>
  </thead>

  <tbody>
    {%- for week in page.weeks %}
    {%- for slot in week.slots %}
    <tr>
      {%- if week.tues %}
      {%- if forloop.first %}
      <th nowrap rowspan="{{ week.slots | size }}">
        {{ week.tues | date: "%m/%d" }}
      </th>
      {% endif -%}

      <td nowrap class="has-text-right">
        {{ slot.time }}
      </td>

      <td>
        {%- if slot.tues %}
        {{ slot.tues }}
        {%- else -%}
        <em class="has-text-grey">Pending</em>
        {% endif -%}
      </td>

      {%- else -%}
      {%- if forloop.first %}
      <td colspan="3" rowspan="{{ week.slots | size }}"></td>
      {% endif -%}
      {% endif -%}

      {%- if week.thur %}
      {%- if forloop.first %}
      <th nowrap rowspan="{{ week.slots | size }}">
        {{ week.thur | date: "%m/%d" }}
      </th>
      {% endif -%}

      <td nowrap class="has-text-right">
        {{ slot.time }}
      </td>

      <td>
        {%- if slot.thur %}
        {{ slot.thur }}
        {%- else -%}
        <em class="has-text-grey">Pending</em>
        {% endif -%}
      </td>

      {%- else -%}
      {%- if forloop.first %}
      <td colspan="3" rowspan="{{ week.slots | size }}"></td>
      {% endif -%}
      {% endif -%}
    </tr>
    {% endfor -%}
    {% endfor -%}
    <tr>
      <td colspan="6"></td>
    </tr>
  </tbody>


</table>

{% include section.html level="h2" name="Selecting Topics" %}

Students must [propose a talk topic](https://usfca.instructure.com/courses/1582982/assignments/6829299) *at least* 1 week before the talk, but are strongly encouraged to select a topic much sooner. When approved, topics will be posted on the schedule above. Topics will be approved in the order they are submitted, regardless of when your talk is scheduled.

All students are encouraged to use the [Data Visualization Resources](/guides/general/resources.html) guide to find topics. Each student must select a unique topic and present content not already shown in class. Before submitting a topic, check the [class schedule](/schedule.html) and the [already approved topics](#approved-topics) above to avoid any overlap.

#### CS 360

For undergraduate students registered for CS 360, valid topics include any tools, techniques, examples, books, blogs, podcasts, or important persons (historical or current) in data visualization that have not already been discussed during class. The topics can be from the broader field of data visualization, including scientific visualization, visual analytics, information dashboards, data storytelling, informative art, infographics, and so on. The [General Topics](/guides/general/resources.html#general-resources) may be especially helpful for selecting a topic.

#### CS 560

For graduate students registered for CS 560, valid topics include any data visualization research paper published in an academic venue such as an academic conference or journal. Students are encouraged to choose a research paper that (a) the authors have posted a free PDF, (b) there is an available online demo, and/or media (such as high-resolution screenshots), and (c) there are presentation or demonstration videos publicly available. The [Open Access VIS](http://oavis.steveharoz.com/) resource may be especially helpful for selecting a paper.
