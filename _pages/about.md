---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a 2nd year computer science PhD student at the Courant Institute of Mathematical Sciences, New York University, advised by [Joseph Tassarotti](https://cs.nyu.edu/~jt4767/). I am broadly interested in formal methods. Lately, I have been working at the intersection of programming languages and formal verification for security properties.

In the past I have worked with [Thomas Wies](https://cs.nyu.edu/~wies/) and [Eric Koskinen](https://www.erickoskinen.com/#/) on developing an abstract-interpretation analysis for verifying certain temporal properties of recursive, higher-order programs.

During a remote internship at TIFR, with [Shibashis Guha](https://www.tifr.res.in/shibashis.guha/), I also worked on developing statistical-model-checking techniques to estimate certain LTL objectives for discrete- and continuous-time markov decision processes.
<br><br>

<h1>Preprints</h1>
{% for post in site.publications reversed %}
  {% if post.category != "preprints" %}
    {% continue %}
  {% endif %}
  {% include archive-single-simple.html %}
{% endfor %}

<h1>Publications</h1>
{% for post in site.publications reversed %}
  {% if post.category != "conferences" %}
    {% continue %}
  {% endif %}
  {% include archive-single-simple.html %}
{% endfor %}