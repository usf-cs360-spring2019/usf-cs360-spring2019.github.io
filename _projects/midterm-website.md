---
title: Midterm Website
navbar: Guides
layout: default
key: 4
---

Instead of a midterm exam, all students must complete a midterm group project. This guide explains the requirements for the midterm project website. See the [Midterm Project](/guides/projects/midterm-project.html) page for more details on other requirements.

{% include section.html level="h2" name="Website Content" %}

The primary deliverable for the midterm project will be the midterm project website. The final release of this website must contain the following information:

  - Pending

These requirements are for the **final release** of the project website. Groups must create multiple releases of their project website. See the [????](#) guide for details on what each release requires.

{% include section.html level="h2" name="Website Creation" %}

Pending

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


{% comment %}
The midterm project websites must include a rich page describing the data subset selected (and any processing performed), a team page with photos and bios of each team member, a prototypes page illustrating the development of the final visualizations, and one visualization page per team member (as described in the requirements section).

Each group must [submit a final release](https://usfca.instructure.com/courses/1582982/assignments/6821965) of their professional project website showcasing their visualizations before class on Tuesday 03/19. All groups must meet this deadline regardless of when they are presenting.
{% endcomment %}
