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
    name: Teddy Ong
    image: assets/images/about_ougc_pages/TeddyImage.webp
    bio: |
      I started gliding four years ago during my undergraduate and I'm now doing a DPhil in Physics. I come from Singapore and the sport is not possible in Southeast Asia. In fact, I think the UK is the safest place to learn gliding, so cherish your opportunity here and now!

  - role: Captain
    name: Adam Hu
    image: assets/images/about_ougc_pages/AdamImage.webp
    bio: |
      I got into gliding in 2023 at Gransden Lodge, and quickly got hooked. I subsequently joined OUGC in 2024, and earned my Bronze & Cross-Country endorsements, as well as my Silver badge in 2025. I love spending time with the awesome people at the club, whether it's just hanging out or helping out at the launch site. As the Captain, I organise our expeditions and the annual Varsity match against Cambridge.

  - role: Treasurer
    name: Darshit Trevadia
    image: assets/images/about_ougc_pages/darshit.jpg
    bio: |
      Hello! I’m a DPhil student in the Department of Materials. I’ve always dreamed of becoming a pilot, but that never quite <i>materialised</i>. I love learning about the sport from members of the Uni club and OGC who have decades of experience. For me, the best thing about gliding is the perspective it gives you. When you’re up there with the birds, everything feels peaceful.

  - role: Membership and Social Secretary
    name: Janet Wang
    image: assets/images/about_ougc_pages/janet.jpeg
    bio: |
      I started gliding three years ago with Edinburgh University, training at the Scottish Gliding Centre, and quickly fall in love with this sport. I like visiting different airfields : Aboyne, Dumfries, and Portmoak always feel a bit like home. I also spent two years as the Social Secretary at the Edinburgh Gliding Club, bringing people together and shaping the little community we had there, which was genuinely one of my favourite parts of the experience.

      Now that I’m in Oxford, I’m really excited to keep flying. The atmosphere at the airfield here is brilliant, and the views from the airfield never get old. I’m looking forward to getting involved, contributing where I can, and helping organise more events that bring the club together and make the whole experience even better for everyone.

  - role: General Member
    name: Sergey Ichtchenko
    image: assets/images/about_ougc_pages/SergeyImage.webp
    bio: |
      I originally started flying back in Finland, where I got my PPL(A) license for powered planes back in 2023. I love that I can continue my flying hobby with gliders at Oxford, surrounded by wonderful and excited pilots from OUGC.
      Blue skies!

  - role: President 2024-2025
    name: Haixuan Liu
    image: assets/images/about_ougc_pages/HaixuanImage.webp
    bio: |
      It has always been a dream of mine to be able to fly in the skies on my own, so it's great to be a part of OUGC/OGC where I can share my joy with many other cool people in the club. It's always amazing to see everyone helping out (for free!!) to keep the sport as affordable and accessible, and I also feel great to be a part of that each time I visit the airfield!


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