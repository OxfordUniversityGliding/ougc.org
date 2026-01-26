---
layout: sidebar_default
permalink: news/latest/
sidebar_title: "news"
cover: "/assets/images/news/250417-CKC_4356.jpg"
redirect_from:
  - /news/
---

<title>Latest Club News - OUGC</title>

# Latest News

{%- for row in site.data.news %}
## {{ row.day }} {{ row.month }} {{ row.year }} &mdash; {{ row.title }}

{{ row.article }}

{% endfor -%}