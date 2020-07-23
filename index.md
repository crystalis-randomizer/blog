---
layout: default
no_sidebar: true
---

## Welcome to Crystals Randomizer Blog

This blog will have some articles about the [randomizer], its
development, and history, as well as upcoming changes and
community events.  If you'd like to contribute a column, please
reach out to steve_hacks on our [discord].

[randomizer]: https://crystalisrandomizer.com
[discord]: https://discord.gg/ktyz5E6

### Posts
<ul class="posts">
   {% assign reversed_posts = site.posts | sort:'date' | reversed %}
  {% for post in reversed_posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
