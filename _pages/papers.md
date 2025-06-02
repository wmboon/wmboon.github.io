---
permalink: /papers/
title: "Publications and Manuscripts"
classes: wide
---

{% assign preprint_posts = site.posts | where_exp:"post", "post.categories contains 'preprints'"%}
<h2> Preprints ({{ preprint_posts.size }}) </h2>

<ul style="list-style-type:square">
  {% for post in preprint_posts %}
    <li>
      {{ post.authors }}. 
      <a href='{{ post.url }}'>{{ post.excerpt }}</a>.
      ({{ post.date | date: '%Y' }})
    </li>
  {% endfor %}
</ul>


{% assign paper_posts = site.posts | where_exp:"post", "post.categories contains 'papers'"%}

<h2> Journal articles ({{ paper_posts.size }}) </h2>

{% assign years = paper_posts
   | group_by_exp: "post", "post.date | date: '%Y'"
%}
{% for year in years %}
  <h4>{{ year.name }}</h4>

  <ul style="list-style-type:square">
    {% for post in year.items %}
      <li>
        {{ post.authors }}. 
        <a href='{{ post.url }}'>{{ post.excerpt }}</a>.
        <em>{{ post.journal }}.</em>
      </li>
    {% endfor %}
  </ul>
{% endfor %}


{% assign proceeding_posts = site.posts | where_exp:"post", "post.categories contains 'proceedings'"%}
<h2> Conference proceedings ({{ proceeding_posts.size }})</h2>
{% assign years = proceeding_posts
   | group_by_exp: "post", "post.date | date: '%Y'"
%}
{% for year in years %}
  <h4>{{ year.name }}</h4>

  <ul style="list-style-type:square">
    {% for post in year.items %}
      <li>
        {{ post.authors }}. 
        <a href='{{ post.url }}'>{{ post.excerpt }}</a>.
        <em>{{ post.journal }}.</em>
      </li>
    {% endfor %}
  </ul>
{% endfor %} 

<h2> Theses </h2>

- Doctoral thesis. \
    [Conforming Discretizations of Mixed-Dimensional Partial Differential Equations](https://bora.uib.no/bora-xmlui/handle/1956/18159)\
    University of Bergen.
- Master thesis. \
    [Incorporation of Contracture Formation in Dermal Wound Healing: A Mathematical Model](https://repository.tudelft.nl/islandora/object/uuid:fd95b7e1-5509-455b-9bca-febbafba72a0)\
    Delft University of Technology.
