---
layout: page
permalink: /tag/
title: "Tag Index"
last_modified_at: 2016-02-08T16:17:58-05:00
excerpt: "An archive of posts sorted by tag frequency."
share: false
author_profile: true
---

{{ page.excerpt | markdownify }}

{% assign sorted_tags = site.tags | sort_tags_by_name %} {% for tag in sorted_tags %}
{{ tag[0] }} ({{ tag[1] }})
{% endfor %}
