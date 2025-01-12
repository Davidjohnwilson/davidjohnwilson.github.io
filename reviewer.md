---
layout: page
title: Reviewer
permalink: /reviewer/
---

## <i class="fa fa-newspaper-o"></i> Reviewing Experience

Over the last four years I have contributed reviews and features to a variety of ballet websites, including the Royal Opera House, The Ballet Bag, and A Younger Theatre. I have also be hired to cover the opening night of Carlos Acosta's new production of Don Quixote for the Royal Opera House on their social media channels (with The Ballet Bag).

This page is a portfolio of some of these reviews and features, along with select articles from my site chronicling my personal ballet journey: [DaveTriesBallet](http://www.davetriesballet.com).

## <i class="fa fa-newspaper-o"></i> Selected Reviews

<ul>
<hr>
<br />
{% for rev in site.data.reviews %}
  <li>
    <i>{{ rev.quote }}</i>
    <br />
    <b>{{ rev.quote_desc}}</b>
    <br />
    <a class="link" href="{{ rev.link_1 }}">{{ rev.piece_1 }}</a>
    {% if rev.link_2 %} and <a class="link" href="{{ rev.link_2 }}">{{ rev.piece_2 }}</a>{% endif %}
    <br />
    <br />
   </li>
  <hr>
  <br />
{% endfor %}
</ul>
<!-- 
## <i class="fa fa-newspaper-o"></i> Contact

If you are interested in contacting me regarding reviewing or ballet articles: [<i class="fa fa-envelope"></i> Contact](mailto:reviewer@davidjw.co.uk?Subject=Reviewing%20Contact%20Enquiry)


 -->