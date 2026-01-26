---
layout: sidebar_default
permalink: news/final_glide/
sidebar_title: "news"
cover: "/assets/images/news/250415-CKC_3940.jpg"
---

<title>Final Glide - OUGC</title>

# <i>Final Glide</i>

<i>Final Glide</i> is OGC's special edition annual newsletter, consisting of a collection of member-written articles submitted over the year. From epic soaring adventures to light-hearted tales around the club, this newsletter celebrates the club's achievements and highlights of the year.

To keep this tradition alive, we need your stories! If you wish to write something for the newsletter, please feel free to submit your pieces to us at [president@ougc.org](mailto:president@ougc.org).

<ul>
  {%- for row in site.data.final_glide -%}
    <li>
      <a href="/assets/documents/final_glide/final-glide-{{ row.issue }}.pdf">Issue {{ row.issue }}: {{ row.month }} {{ row.year }}{%- if forloop.first %} (LATEST){% endif %}</a>
    </li>
  {%- endfor -%}
</ul>