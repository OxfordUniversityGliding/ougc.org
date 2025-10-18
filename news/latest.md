---
layout: sidebar_page
permalink: news/latest/
sidebar_title: "news"
redirect_from:
  - /news/
---

<title>Latest Club News - OUGC</title>

# Latest News

{%- for row in site.data.news -%}
<br>
## {{ row.day }} {{ row.month }} {{ row.year }} &mdash; {{ row.title }}

{{ row.article }}
{%- endfor -%}