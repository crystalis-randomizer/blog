---
layout: default
no_sidebar: true
---

## Welcome to Crystals Randomizer Blog

This blog will have some articles about the [randomizer](https://crystalisrandomizer.com), development, and history.

### Posts
<ul class="posts">
   {% assign reversed_posts = site.posts | sort:'date' | reversed %}
  {% for post in reversed_posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
