---
layout: about_page
title: Pilot Stories
permalink: /about_ougc/pilot_stories/
stories:
  - title: Daisy Makin - first year Physics (mphys)

 
    # first part of the story text
    text_before: |
        Hi, I’m Daisy and I’m a first year Physics student at Somerville College from East Sussex. Before coming to Oxford, I’d never flown any kind of aircraft, but I had been involved in a school project to design and build a flight simulator, and since then was keen to get behind the controls for real! However, I didn’t really think this would be possible due to how expensive flying can be, until I came across the OUGC stand at the Freshers’ Fair. With the surprisingly low costs of the OUGC, combined with the generous bursary I receive from my college, I’ve been able to make progress towards my first solo flight, and I’m really enjoying being given more responsibility for launches and landings each time I fly.  
          
        Gliding is such an amazing escape from the pressures of Oxford and is a great way to meet new and different people – the club has a mix of undergrads and postgrads, plus all the instructors from Bicester help create a really welcoming and fun environment. The fact the club is volunteer led really helps this – from day one you will be expected to help out at the airfield, and I have really enjoyed learning about how the gliders are maintained and about the internal workings of them.

  - title: Chia-Man Hung (DPhil in Robotics & Machine Learning)

    text_before: |
        Growing up in Taiwan, I had never heard about gliding nor had I thought that I would be flying one day. My first exposure to gliding was in Paris (where I did my bachelor’s and master’s degrees) in 2015. A friend of mine brought me to his club for an air experience. It wasn’t possible for me to start learning at that time, but since then, I have always wanted to fly.  
          
        At the Freshers’ Fair 2017, just as every other fresher, I signed up to a whole lot of different clubs, including Oxford University Gliding Club. Although I was very interested in gliding, to be honest, I was a bit put off by the cost. I started the first two weeks by trying out other clubs and missed the annual intro evening (which I regret), as well as the sign up to intro days (which happened at the intro evening). After checking the OUGC website, it turned out that gliding was much more affordable than I thought. Just a few days after the intro evening I finally decided to join as a trial member. To my surprise there had been so many people signing up that the first available intro day slot was right at the end of Michaelmas Term! The more I read about the gliding club, the more I wanted to join and start training as soon as possible. So I put my name down for all the waiting lists for intro days and finally joined by the end of October 2017. Moral of the story - stop wishing and start flying!
    image: assets/images/about_ougc_pages/stories/k8.webp
    alt: Alice converting to the K8
    caption: CONVERTING TO THE K8
    # text that continues *after* the image/caption
    text_after: |
        On my first day at the Bicester airfield, I was very excited, but also a bit nervous as I didn’t know what to expect. The committee members and the instructors were extremely welcoming and approachable, and I quickly got to know other members. After visiting the hangar, doing some paperwork, learning about the ground handling of gliders, etc., we arrived at the launch point and I was quickly paired up with an instructor. He gave me a briefing and off we went! My first winch launch was sudden and I felt the acceleration in my back and my heart beating fast! We climbed at about 45°, but it appeared steeper to me. After the launch, it was so smooth inside the cockpit. To me, gliding is the purest form of flying - engineless, silent and graceful - as close to the birds as I will ever be. I believe this is a universal feeling that many glider pilots share.  
          
        I have been with the gliding club for more than a year now. I can say joining the club is one of the best things that happened to me. This is the place where I feel I belong. The nature of the sport makes it such a friendly community. We all need each other’s help to get airborne and we all help each other. We are a friendly bunch, sometimes even a bit mad. We get addicted at checking weather forecast. We get annoyed if we are not available to fly on a good day. Even then, we watch gliders flying on tracking systems. (Or is it just me?) Gliding is continually challenging and every day is different. On good days, we will be aiming for new badges or setting new personal records (height gain, duration, distance, speed, etc.). There is always another badge to aim for and there is always more to learn.
        
---

# Everyone can become exceptional at OUGC
{: .committee-title}

We’re all normal students, most of whom never had experienced airsport or ever dreamed that they would learn to fly at University.
{: .committee-intro}

<div class="stories">
{% for s in page.stories %}
  <article class="story">
    {% if s.title %}<h3 class="story-title">{{ s.title }}</h3>{% endif %}
    {% if s.author %}<p class="story-byline">{{ s.author }}</p>{% endif %}

    {{ s.text_before | markdownify }}

    {% if s.image %}
      <figure class="story-figure">
        <img src="{{ s.image | relative_url }}" alt="{{ s.alt | default: s.caption | default: s.title }}">
        {% if s.caption %}<figcaption class="story-caption">{{ s.caption }}</figcaption>{% endif %}
      </figure>
    {% endif %}

    {% if s.text_after %}{{ s.text_after | markdownify }}{% endif %}
  </article>
{% endfor %}
</div>