---
title: Welcome
description: Our company is your's...
layout: default
tags: [primary, footer]
date: 2024-01-01
---
[Building the main navigation for a website](https://web.dev/articles/website-navigation)

{% for i in collections.blog %}
- [{{ i.data.title }}]({{ i.url }})
{% endfor %}