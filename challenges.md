---
layout: page
title: Companies & Challenges
permalink: /challenges/
---

Each participating company brings one concrete challenge for the working groups.
Registered participants receive the full challenge briefs, with business context,
available data and constraints, before the event.

{% for c in site.data.companies %}
<section class="challenge" id="{{ c.id }}">
  <div class="challenge-head">
    <a class="challenge-logo" href="{{ c.url }}" title="{{ c.name }}"><img src="{{ "/assets/images/" | append: c.logo | relative_url }}" alt="{{ c.name }}"></a>
    <div>
      <div class="company-sector">{{ c.sector }}</div>
      <div class="challenge-company"><a href="{{ c.url }}">{{ c.name }}</a></div>
    </div>
  </div>
  <h3>{{ c.challenge_title }}</h3>
  <p>{{ c.pitch }}</p>
</section>
{% endfor %}
