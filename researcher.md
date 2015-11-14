---
layout: page
title: Researcher
permalink: /researcher/
---

##<i class="fa fa-flask"></i> Research Summary

I have spent three years researching into *Cylindrical Algebraic Decomposition* (CAD) for my PhD at the [University of Bath](university-of-bath). I was supervised by Prof. James Davenport and Dr Russell Bradford, as part of the Real Geometry and Connectedness via Triangular Description resarch group. I submitted by thesis in July 2014 (available: [<i class="fa fa-book"></i> PDF](/publications/djwthesis.pdf)) and successfully defended in November 2014 (with Prof. C K Yap and Prof N Vorobjov as my examiners). I was awarded my PhD in January 2015, and graduated in July 2015. 

This page describes my academic work and publications.

The following is a short video explaining the ideas behind my research, submitted for the finals of the EPSRC UK ICT Pioneers competition:

<iframe class="embed-responsive-item" src="http://www.youtube.com/embed/M33WRwr4bAY" allowfullscreen></iframe>

##<i class="fa fa-flask"></i> Publications

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

##<i class="fa fa-flask"></i> Contact

If you are interested in contacting me regarding academic research: [<i class="fa fa-envelope"></i> Contact](mailto:researcher@davidjw.co.uk?Subject=Research%20Contact%20Enquiry)



[university-of-bath]: http://www.bath.ac.uk
[arxiv]:              http://arxiv.org/a/wilson_d_3
[opus]:               http://opus.bath.ac.uk/view/person_id/6172.html
