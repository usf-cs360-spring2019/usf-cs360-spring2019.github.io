---
title: Getting Started with D3.js
navbar: Guides
layout: guides
key: 1.1
---

This guide provides a little background for getting started with [D3.js](https://d3js.org/). See the [Data Visualization Resources](resources.html) and the [Introduction to D3.js](https://beta.observablehq.com/d/28ba93f58fb82f49) Observable notebook for more.

{% include section.html level="h2" name="Web Technologies" %}

Before trying to tackle learning [D3.js](https://d3js.org/), it helps to already be familiar with basic web technologies. The [Mozilla Developer Network (MDN)](https://developer.mozilla.org/en-US/) guides are great for both tutorials and no-nonsense references:

  - [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
  - [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
  - [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
  - [SVG](https://developer.mozilla.org/en-US/docs/Web/SVG)

I also recommend the following:

  - [Truthy](https://developer.mozilla.org/en-US/docs/Glossary/Truthy) (MDN Glossary)
  - [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) (Github Guides)

Here are a few other resources that may be useful for learning HTML and JavaScript:

  - [Introduction to HTML](https://lab.github.com/githubtraining/introduction-to-html) (Github Training Course)
  - [Introduction to HTML](https://beta.observablehq.com/@mbostock/introduction-to-html) (Observable Notebook)
  - [Introduction to HTML](https://www.codecademy.com/learn/learn-html) (Codecademy)
  - [Introduction to Basic HTML and HTML5](https://learn.freecodecamp.org/responsive-web-design/basic-html-and-html5/) (freeCodeCamp)
  - [Introduction to CSS](https://learn.freecodecamp.org/responsive-web-design/basic-css/) (freeCodeCamp)
  - [Introductionto JavaScript](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript/) (freeCodeCamp)
  - [Introduction to JavaScript](https://www.codecademy.com/learn/introduction-to-javascript) (Codecademy)
  - [JavaScript](https://en.wikibooks.org/wiki/JavaScript) (Wikibooks)
  - [JavaScript for Cats](http://jsforcats.com/)

There are many more options that can be found with a web search, especially if you prefer videos over text.

{% include section.html level="h2" name="Remote Hosting" %}

Small examples may be hosted via a combination of [Github gists](https://gist.github.com/), [bl.ocks.org](https://bl.ocks.org/), and [blockbuilder.org](https://blockbuilder.org/).

The files required for the visualization(s) are stored in a [gists](https://gist.github.com/), which is basically a lightweight `git` repository meant for sharing code with others. This should include an `index.html` file, and any other files and resources required by the code. See the [Github Help](https://help.github.com/categories/gists/) pages for more information about gists.

To view the visualization, load the gist in [bl.ocks.org](https://bl.ocks.org/). See the [About](https://bl.ocks.org/-/about) page for how to view a gist on [bl.ocks.org](https://bl.ocks.org/). Keep in mind there is sometimes a slight delay between the files cached by [bl.ocks.org](https://bl.ocks.org/) and those hosted on [gist.github.com](https://gist.github.com/). If you want to modify the code and see live changes, load the gist in [blockbuilder.org](https://blockbuilder.org/) instead.

All of these websites use the `gistid` in the URL, with the primary difference being the domain:

```
https://gist.github.com/username/gistid
https://bl.ocks.org/username/gistid
https://blockbuilder.org/username/gistid
```

Small examples may also be hosted using [Observable Notebooks](http://beta.observablehq.com/) as well. Many examples are being moved over to Observable, but it is still in beta. See the [Introduction to D3.js](https://beta.observablehq.com/d/28ba93f58fb82f49) Observable notebook for more.

For hosting an entire website of visualizations, use [Github Pages](https://pages.github.com/). There are many guides for setting up Github repositories for Github Pages:

  - [Github Pages](https://pages.github.com/) (Landing Page)
  - [Github Pages](https://lab.github.com/githubtraining/github-pages) (Github Training Course)
  - [Github Pages Basics](https://help.github.com/categories/github-pages-basics) (Github Help Pages)
  - [Getting Started with GitHub Pages](https://guides.github.com/features/pages/) (Github Guides)
  - [Customizing Github Pages](https://help.github.com/categories/customizing-github-pages) (Github Help Pages)

The [course website](https://github.com/usf-cs360-spring2019/usf-cs360-spring2019.github.io) is also hosted using Github Pages.

{% include section.html level="h2" name="Local Development" %}

Run a local web server to run and debug visualizations locally. This is especially important for loading data. There are many options for running a local web server.

The official [D3 wiki](https://github.com/d3/d3/wiki#local-development) recommends using `npm` to run the [`http-server`](https://www.npmjs.com/package/http-server) package from [Node](https://nodejs.org/en/):

```
npm install -g http-server
http-server &
```

It is also possible to [use Python to run a web server](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/set_up_a_local_testing_server#Running_a_simple_local_HTTP_server). Use the [SimpleHTTPServer](https://docs.python.org/2/library/simplehttpserver.html) module if Python version 2 is installed:

```
python -m SimpleHTTPServer
```

Use the [http.server](https://docs.python.org/3/library/http.server.html) module for Python version 3:

```
python3 -m http.server
```

Another option is to develop in [Atom](https://atom.io/) and use the [live-server](https://atom.io/packages/atom-live-server) package to launch a local web server.

For all of these options, run the local web server from the same directory as the `index.html` file. Access the website at `http://localhost:[port]` where `[port]` is the port number used by the web server. This is usually something like `3000`, `4000`, or `8080`.
