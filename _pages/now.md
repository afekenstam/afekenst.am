---
layout: page
title:  "Now"
permalink: /now
---
<section class="fl w-100 ph5 ph0-ns pv6">
  <div class="tl tc-ns pt3 pb4 pb6-ns">
    <h3 class="f4 fw6 silver ttu gotham-bold tracked">Now</h3>
    <p class="f4 f3-ns fw3 sentinel-light-italic">Current work status + random stuff I find <br class="dn db-ns">interesting at the moment.</p>
    <p class="f7 fw6 silver ttu gotham-bold tracked">BASED ON <a href="https://nownownow.com/p/wMyz" target="_blank" class="silver">NOWNOWNOW</a></p>
  </div>
  <div class="w-100 w-40-ns center tl ph5-ns">
    {% for item in site.data.now %}
      <a href="{{ item.cta_url }}" rel="nofollow" title="{{ item.cta }}" class="db link pv4 pv5-ns" target="_blank">
        <img src="{{ item.picture }}" alt="{{ item.cta }}" class="h2 pr2 dib v-mid">
        <h5 class="f4 fw5 ttu dib v-mid ma0 gotham-extralight">{{ item.type }}</h5>
        <p class="f4 fw3 sentinel-light">{{ item.body }}</p>
        <span class="db f7 silver ttu gotham-bold tracked">{{ item.cta }}</span>
      </a>
    {% endfor %}
  </div>
</section>