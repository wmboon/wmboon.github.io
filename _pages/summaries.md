---
permalink: /summaries/
title: "Summaries of papers"
layout: category
taxonomy: papers
entries_layout: grid
sort_by: date
sort_order: reverse
show_date: false
---

{% assign paper_posts = site.posts | where_exp:"post", "post.categories contains 'papers'"%}
{% assign summaries = paper_posts | where_exp:"post", "post.has_summary"%}
{% assign years = summaries
   | group_by_exp: "post", "post.date | date: '%Y'"
%}
{% for year in years %}
  <h3>{{ year.name }}</h3>

  <ul style="list-style-type:square">
    {% for post in year.items %}
      <li>
        {{ post.authors }}. 
        <a href='{{ post.url }}'>{{ post.excerpt }}.</a>
        <em>{{ post.journal }}.</em>
      </li>
    {% endfor %}
  </ul>
{% endfor %} 