---
layout: sidebar_page
title: " "
permalink: /about_ougc/events/
sidebar_include: "about_ougc_sidebar.html"
cover: "/assets/images/about_ougc_pages/Menu.webp"

events:
  - title: Annual Dinner
    image: assets/images/about_ougc_pages/Annual+Dinner+2016.webp
    alt: OUGC members at the Annual Dinner
    body: |
      This is the OUGC event of the year, usually held in May. Enjoy re-connecting
      with OUGC members past and present, as well as a traditional Oxford formal
      dinner in a historic setting.
    align: right   # image on the RIGHT, text on the LEFT

  - title: Socials
    image: assets/images/about_ougc_pages/51333316806_bab6821e32_o.webp
    alt: OUGC members at a club social
    body: |
      Whether in Oxford or at the airfield, we always have a good time!
    align: left    # image on the LEFT, text on the RIGHT

  - title: Alumni Flying Day
    image: assets/images/trips_training_weeks_expeditions/europe5.jpg.webp
    alt: Alumni Flying Day
    body: |
      The Alumni flying day is a new event where ‘High Flyer’ members of the ‘1937’ club are invited back to RAF Weston-on-the-Green airfield for a day of flying fun. We hope to run such a day in 2026.
    align: right    # image on the LEFT, text on the RIGHT
---

# Events
{: .about-events-titles}

OUGC hosts a range of events during the year, from casual socials to our annual dinner.
{: .about-all-intros}

<div class="events-list">
{% for e in page.events %}
  {%- assign flip = e.align | default: '' -%}
  <section class="event-row {% if flip == 'right' %}right{% endif %}">
    {% if e.image %}
      <div class="event-media">
        <img src="{{ e.image | relative_url }}" alt="{{ e.alt | default: e.title }}">
      </div>
    {% endif %}
    <div class="event-copy">
      {% if e.title %}<h3 class="event-title">{{ e.title | upcase }}</h3>{% endif %}
      {{ e.body | markdownify }}
    </div>
  </section>
{% endfor %}
</div>