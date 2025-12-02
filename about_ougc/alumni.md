---
layout: sidebar_page
title: " "
permalink: /about_ougc/alumni_1937_club/
sidebar_title: "about_ougc"
cover: "/assets/images/about_ougc_pages/grid.png"

events:

  - title: A Unique Sport Experience
    image: assets/images/about_ougc_pages/2017_Dina_upside_down.jpg
    alt: Inverted
    body: |
      The Oxford University Gliding Club is one of the oldest gliding clubs in the country. It has been teaching students to fly since 1937, and the number of people that have been introduced to the joy of un-powered flight is countless. 
    align: left    # image on the LEFT, text on the RIGHT

  - title: Varsity Victories
    image: /assets/images/about_ougc_pages/IMG_1460.jpg
    alt: Varsity Team Photo 2018
    body: |
      OUGC’s long-standing commitment to professional training can be best seen through the large variety of opportunities the club offers. Oxford has won the majority of varsity matches against Cambridge in recorded [history](/competitions/varsity_results/).
    align: right   # image on the RIGHT, text on the LEFT

  - title: History
    image: /assets/images/about_ougc_pages/1960s.jpg
    alt: 1960s
    body: |
      Only a tiny fraction of a good part of a century of flying can be found in the Bodleian Libraries.
---

<title>The 1937 Club - OUGC</title>

# Introducing ‘The 1937 Club’
{: .about-alumni-titles}

The 1937 Club offers membership to all alumni of OUGC and kind donors. It aims to reconnect the OUGC alumni with other alumni, friends, and the current members. This will help to support OUGC financially, supporting us in our current campaign to re-gel our gliders and purchase them new trailers. The club also aims to better integrate the community of past and present OUGC members and support a thriving gliding community.  
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

Over its long history OUGC has strived towards
{: .about-all-intros}
- providing high quality gliding training for as many students as possible, with the goal of becoming certified pilots while undertaking the challenge of an Oxford degree;
- offering our motivated young pilots a pathway into professional aviation by holding talks with commercial pilots and facilitating networking within the aviation community;
- continuously creating a social environment for both current OUGC members and its alumni to meet.
{: .about-all-intros}

Given the diverse structure of the club our alumni find themselves in a variety of different circumstances after leaving university. As such, the club welcomes donations of any amounts and any donor automatically becomes a member of The 1937 Club, receiving E news and an invite to our annual dinner.
{: .about-all-intros}

<div class="home-button-wrapper">
  <a href="https://docs.google.com/forms/d/e/1FAIpQLSfiX8qwFBxW6Q25WarfJinKM03eVTyeUc9dY6mM90PEjdrLqw/viewform?usp=dialog" class="big-button">Sign Up to The 1937 Club</a>
</div>

Our main aim is to raise funds for the re-finishing of the gel coat on our K-21 G-DESB. We are about £25,000 short of our target and we would appreciate help in any form. In addition to financing, this may include volunteering your time to help with preventative maintenance, organising logistics for transporting the glider and trailer, etc. More details on how to support us can be found below.
{: .about-all-intros}

<div class="home-button-wrapper">
  <a href="/support_us/" class="big-button">Support Us!</a>
</div>

