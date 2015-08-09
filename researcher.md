---
layout: page
title: Researcher
permalink: /researcher/
---

##{% icon fa-flask %} Research Summary

I have spent three years researching into *Cylindrical Algebraic Decomposition* (CAD) for my PhD at the [University of Bath](university-of-bath). I was supervised by Prof. James Davenport and Dr Russell Bradford, as part of the Real Geometry and Connectedness via Triangular Description resarch group. I recently submitted by thesis (available: [PDF]()) and will be defending my thesis later this year.

This page describes my academic work and publications.

The following is a short video explaining the ideas behind my research, submitted for the finals of the EPSRC UK ICT Pioneers competition:

<iframe class="embed-responsive-item" src="http://www.youtube.com/embed/M33WRwr4bAY" allowfullscreen></iframe>

##{% icon fa-flask %} Publications

The following is a list of my peer-reviewed publications, in preprint form, hosted on the [arXiv](arxiv). They are all freely-available on the [University of Bath Opus Repository](opus), along with various non-peer reviewed technical reports and peer-reviewed pedagogical articles.

<ul>
<hr>
{% for pub in site.data.publications %}
  <li>
      <a class="post-link" href="/publications/{{ pub.filename | prepend: site.baseurl }}">{{ pub.title }}</a>
    {{ pub.author_list }} 
    {% if pub.conference %}({{ pub.conference}}){% endif %}
    <br />
    {{ pub.journal_name }} 
    {% if pub.volume or pub.pages %}({% endif %}
    {% if pub.volume %}<b>{{ pub.volume }}</b>{% endif %}
    {% if pub.volume and pub.pages %}:{% endif %}
    {% if pub.pages %}p.{{ pub.pages}}{% endif %}
    {% if pub.volume or pub.pages %}){% endif %}
    {% if pub.year %}| {{pub.year}}.{% endif %}
    <br/>

    {% if pub.arxiv_url or pub.opus_url %}Mirrors:{% endif %}
    {% if pub.arxiv_url %}<a class="link" href="{{ pub.arxiv_url }}">the arXiv</a>{% endif %}
    {% if pub.arxiv_url and pub.opus_url %}and{% endif %}
    {% if pub.opus_url %}<a class="link" href="{{ pub.opus_url }}">University of Bath Opus</a>{% endif %}
    <br />
  </li>
  <hr>
{% endfor %}
</ul>

##{% icon fa-flask %} Contact

If you are interested in contacting me regarding academic research: [{% icon fa-envelope %} Contact](mailto:researcher@davidjw.co.uk?Subject=Research%20Contact%20Enquiry)



[university-of-bath]: http://www.bath.ac.uk
[arxiv]:              http://arxiv.org/a/wilson_d_3
[opus]:               http://opus.bath.ac.uk/view/person_id/6172.html