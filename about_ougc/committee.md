---
layout: sidebar_page
title: " "
redirect_from:
  - /about_ougc/
permalink: /about_ougc/committee/
sidebar_title: "about_ougc"
cover: "/assets/images/about_ougc_pages/K13_launching.webp"

committee:
  - role: President
    name: Haixuan Liu
    image: assets/images/about_ougc_pages/HaixuanImage.webp
    bio: |
      It has always been a dream of mine to be able to fly in the skies on my own, so it's great to be a part of OUGC/OGC where I can share my joy with many other cool people in the club. It's always amazing to see everyone helping out (for free!!) to keep the sport as affordable and accessible, and I also feel great to be a part of that each time I visit the airfield!

  - role: Captain
    name: Adam Hu
    image: assets/images/about_ougc_pages/AdamImage.webp
    bio: |
      I got into gliding in 2023 at Gransden Lodge, and quickly got hooked. I subsequently joined OUGC in 2024, and earned my Bronze & Cross-Country endorsements, as well as my Silver badge in 2025. I love spending time with the awesome people at the club, whether it's just hanging out or helping out at the launch site. As the Captain, I organise our expeditions and the annual Varsity match against Cambridge.

  - role: Secretary
    name: Sergey Ichtchenko
    image: assets/images/about_ougc_pages/SergeyImage.webp
    bio: |
      I originally started flying back in Finland, where I got my PPL(A) license for powered planes back in 2023. I love that I can continue my flying hobby with gliders at Oxford, surrounded by wonderful and excited pilots from OUGC.
      Blue skies!

  - role: Treasurer
    name: Teddy Ong
    image: assets/images/about_ougc_pages/TeddyImage.webp
    bio: |
      I started gliding four years ago during my undergraduate and I'm now doing a DPhil in Physics. I come from Singapore and the sport is not possible in Southeast Asia. In fact, I think the UK is the safest place to learn gliding, so cherish your opportunity here and now!

---

<title>Our Committee - OUGC</title>

# OUR COMMITTEE 2025-2026
{: .about-committee-titles}

The Committee are the organising heart of the club.  
For any general enquiries, please email [president@ougc.org](mailto:president@ougc.org)
{: .about-committee-intros}

<div class="committee-stack">
{% for m in page.committee %}
  <section class="committee-row">
    <div class="photo">
      <img src="{{ m.image | relative_url }}" alt="{{ m.name }} – {{ m.role }}">
    </div>
    <div class="bio">
      <h3 class="role-name">{{ m.role | upcase }} – {{ m.name | upcase }}</h3>
      {{ m.bio | markdownify }}
    </div>
  </section>
{% endfor %}
</div>