---
layout: archive
title: ""
permalink: /publications/
author_profile: true
---
<!-- <p style="text-align:left; color:Blue; font-size:30px; font-weight:bold;"> Journal Articles </p> -->
<ol>

{% assign pubs = site.data.publications.references | sort: "date" | reverse %}
{% for pub in pubs %}
   {% if pub.article == "Journal" %}
      <li>
         <b> {{ pub.title }} </b>
         <br>
         {% for name in pub.author %}
            {{ name.given }} {{ name.family }},
         {% endfor %}
         <br>
         <i> {{ pub.journal }}, </i>
         {{ pub.year }},
         {% if pub.DOI %}
            DOI: <a target="_blank" href="{{ pub.DOI }}"><span class="tag is-danger">{{ pub.DOI }}</span></a>
         {% endif %}
<!--         <br>
         <br>
         {{pub.abstract}} -->
         <br>
         <br>
      </li>
   {% endif %}
{% endfor %}

</ol>

<!-- <p style="text-align:left; color:Blue; font-size:30px; font-weight:bold;"> Book Chapters </p> -->
<ol>

{% assign pubs = site.data.publications.references | sort: "year" | reverse %}
{% for pub in pubs %}
   {% if pub.article == "Book" %}
      <li>
         <b> {{ pub.title }} </b>
         <br>
         {% for name in pub.author %}
            {{ name.given }} {{ name.family }},
         {% endfor %}
         <br>
         <i> {{ pub.book }} </i>,
         {{ pub.year }},
         DOI: <a target="_blank" href="{{ pub.DOI }}"><span class="tag is-danger">{{ pub.DOI }}</span></a>
      </li>
   {% endif %}
{% endfor %}

</ol>


<!-- <p style="text-align:left; color:Blue; font-size:30px; font-weight:bold;"> Theses </p> -->
<ol>

{% assign pubs = site.data.publications.references | sort: "year" | reverse %}
{% for pub in pubs %}
   {% if pub.article == "Thesis" %}
      <li>
         <b> {{ pub.title }} </b>
         <br>
         {% for name in pub.author %}
            {{ name.given }} {{ name.family }}
         {% endfor %}
         <br>
         <i> {{ pub.University }} </i>,
         {{ pub.year }},
         DOI: <a target="_blank" href="{{ pub.DOI }}"><span class="tag is-danger">{{ pub.DOI }}</span></a>
      </li>
   {% endif %}
{% endfor %}

</ol>
