---
layout: page
title: How to Puppet
tagline: A community Puppet FAQ.
---
{% include JB/setup %}

howtopuppet.com is intended to be a curated, up-to-date, _linkable_ repository for common
questions and explanations, errors, and patterns for Puppet an related software.

Contributions are certainly welcome; see the [GitHub repository](https://github.com/jantman/howtopuppet)
for more information.

## Newest Additions

<ul class="posts">
  {% for post in site.posts limit:5 %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a> in {{ post.category }}</li>
  {% endfor %}
</ul>

## All Posts by Category

<ul class="tag_box inline">
  {% assign categories_list = site.categories %}
  {% include JB/categories_list %}
</ul>


{% for category in site.categories %} 
  <h3 id="{{ category[0] }}-ref">{{ category[0] | join: "/" }}</h3>
  <ul>
    {% assign pages_list = category[1] %}  
    {% include JB/pages_list %}
  </ul>
{% endfor %}
