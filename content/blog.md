---
title: Blog
description: Our blog with stories.
layout: default
tags: [primary, footer]
aside: blog
secondary: true
date: 2024-01-03
---
Without any media queries, that will set up a grid container that has a flexible number of columns. The columns will stretch a little, until there is enough room for another one, and then a new column is added, and in reverse.

The only weakness here is that first value in minmax() (the 10rem value above). If the container is narrower than whatever that minimum is, elements in that single column will overflow. Evan Minto shows us the solution with min().