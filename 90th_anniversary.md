---
layout: home
title: 90th Anniversary
permalink: /90th_anniversary/
cover: "/assets/images/about_ougc_pages/Menu.webp"

events:

  - title: Annual Dinner
    image: assets/images/about_ougc_pages/Annual+Dinner+2016.webp
    alt: OUGC members at the Annual Dinner
    body: |
      90th Anniversary dinner. Enjoy re-connecting
      with OUGC members past and present, as well as a cozy formal dinner in a historic setting.
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
      The Alumni flying day is a new event where ‘High Flyer’ members of the ‘1937’ club are invited back to RAF Weston-on-the-Green airfield for a day of flying fun. We hope to run such a day in 2027.
    align: right    # image on the LEFT, text on the RIGHT
---

<title>90th Anniversary Celebrations</title>

# 90th Anniversary Celebrations
{: .about-events-titles}

Please update your contact details and don't miss out on any updates or invites!

<div class="home-button-wrapper">
  <a href="https://docs.google.com/forms/d/e/1FAIpQLSfiX8qwFBxW6Q25WarfJinKM03eVTyeUc9dY6mM90PEjdrLqw/viewform?usp=dialog" class="big-button">Update Alumni Contact Details</a>
</div>

## 90th Anniversary Dinner - 30 Jan 2027

It is our greatest pleasure to announce the 90th Anniversary dinner in Oxford, celebrating the founding of OUGC in 1937! We are pleased to invite students, alumni, the gliding community and guests to share their fond memories in connection with OUGC and raise a glass towards our future ambitions.  

There will be a drinks reception, followed by a three-course dinner hosted at the historic Vincent's Club. As seating is limited, we encourage you to RSVP as soon as possible! Afterwards, we will contact you with more details of the event, payment, menu options, etc. You'll be free to modify your submission on this form (and withdraw if necessary).

Here are the details:

**Date**: Saturday 30 Jan 2027, 6.30pm (Exact timings TBC)

**Location**: Vincent's Club, 1A King Edward St, Oxford OX1 4HS

**Dress Code**: Formal; Gowns welcome
(There is full disabled access via lift with a disabled toilet at the venue.)

Ticket Prices:
- Early Bird Non-student: £98
- Student: £68

Invites are being sent out to our alumni contact lists. As they are somewhat outdated, you may not have received yours yet because the old email address we have on record have expired. Please update your contact details above, and please send any enquiries (no matter how small) to Teddy Ong at **president@ougc.org**.

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

<div class="home-button-wrapper">
  <a href="/support_us/" class="big-button">Support Us!</a>
</div>

