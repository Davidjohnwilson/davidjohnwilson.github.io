---
layout: page
title: Data Scientist
permalink: /data/
---


##<i class="fa fa-bar-chart"></i> Data Studies

<ul class="post-list">
{% for post in site.posts %}
<li>
<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

<h2>
<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
</h2>
{{ post.excerpt }}
Tags: {% for tag in post.tags %}  <b>{{tag}}</b>  {% endfor %}
</li>
{% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>


##<i class="fa fa-bar-chart"></i> Contact

If you are interested in contacting me regarding development: [<i class="fa fa-envelope"></i> Contact](mailto:developer@davidjw.co.uk?Subject=Development%20Contact%20Enquiry)

