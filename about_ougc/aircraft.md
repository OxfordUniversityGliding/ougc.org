---
layout: about_page
title: Aircraft
permalink: /about_ougc/aircraft/
aircraft:
  - name: ASK 21 (ESB)
    image: assets/images/about_ougc_pages/ESB.webp
    alt: Our ASK-21 ESB at Weston-on-the-Green
    body: |
        Our ASK21, ESB. A popular training aircraft, K21’s are renowned for their friendly in-flight characteristics and easy handeling. Despite this they have good performance, with a 1:34 best glide ratio, making them great cross-country training aircraft.  
        ESB is also an aerobatic machine, with a G tolerance of +6.5 and -4. Many OUGC pilots have won aerobatic badges in her!  
        It is possible to hire ESB for a full day, week or competition. See our costs page.

  - name: ASTIR CS (FEF)
    image: assets/images/about_ougc_pages/ASTIR.webp
    alt: Our Astir FEF at Weston-on-the-Green
    body: |
        Our Astir CS, FEF. A great first cross-country machine, with decent performance and the ability to carry water in tanks to increase speed. Many pilots have completed flights hundreds of kilometers.  
        It is possible to hire FEF for a full day, week or competition. See our costs page.

  - name:  
    body: |
        Oxford Gliding Club has a large complement of aircraft for OUGC members to use. Their fleet includes:  

        1x ASK-21 (the same type as our ESB)  

        1x DG505 advanced cross-country two seater trainer  

        1x DG500 advanced cross-country two seater trainer 

        1x T21 vintage open-cockpit (!!!) two seater  

        1x ASK8 (basic single seater, often pilot’s first single seater aircraft)  

        3x Astir 
---

# Our Aircraft
{: .about-ougc-all-titles}

OUGC owns two aircraft, a ASK21 two seater trainer, and a Astir CS. By being a member of OUGC you automatically are also made a member of our host club, Oxford Gliding Club, with access to their large fleet of aircraft. 
{: .about-ougc-all-intros}

<div class="aircraft-list">
{% for a in page.aircraft %}
  <article class="aircraft-item">
    <hr class="aircraft-rule">
    {% if a.image %}
      <figure class="aircraft-figure">
        <img src="{{ a.image | relative_url }}" alt="{{ a.alt | default: a.name }}">
      </figure>
    {% endif %}
    <div class="aircraft-body">
      {% if a.name %}<h3 class="aircraft-name">{{ a.name }}</h3>{% endif %}
      {{ a.body | markdownify }}
    </div>
  </article>
{% endfor %}
</div>