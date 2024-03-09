---
title: Blog
description: Create a blog with collections & pagination
layout: default
tags: blog
date: 2024-02-02
---
## Pagination et navigation d'une page à l'autre

```
{% raw %}
{% if collections.blog %}
{% assign previousPost = collections.blog | getPreviousCollectionItem %}
{% assign nextPost = collections.blog | getNextCollectionItem %}
{% if nextPost or previousPost %}
{% if previousPost %}
<a role="button" href="{{ previousPost.url }}">Previous post: {{ previousPost.data.title }}</a>
{% endif %}
{% if nextPost %}
<a role="button" href="{{ nextPost.url }}">Next post: {{ nextPost.data.title }}</a>
{% endif %}
{% endif %}
{% endif %}
{% endraw %}
```
## Tri par date et cacher des pages pour le futur