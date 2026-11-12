---
layout: default
---

<div class="home" markdown="1">

<div class="hero" markdown="1">

# **{{ site.event.name }}**

<div class="key-facts" markdown="1">
**Dates:** {{ site.event.dates }} <br>
**Location:** {{ site.event.venue }}, {{ site.event.city }}
{%- if site.event.contact_email != "" %} <br>
**Contact:** [{{ site.event.contact_email }}](mailto:{{ site.event.contact_email }})
{%- endif %}
</div>

{% include logo-strip.html %}

<div class="news-box">
  <div class="news-title"><a href="{{ "/apply/" | relative_url }}">Applications are closed for now</a></div>
  <div>
    Two days of exchange between research and industry at {{ site.event.venue }}, Aachen.<br>
    Keynotes, company pitches, collaborative working sessions and networking.
  </div>
</div>

</div>

## About

**{{ site.event.name }}** takes place on
**{{ site.event.dates }} at {{ site.event.venue }} in {{ site.event.city }}**.

Organized jointly by **AI Grid, JUPITER AI Factory, CAIRNE and RWTH Aachen University**,
the event brings together master's students, doctoral researchers, companies and AI
organizations from Germany and neighboring European countries.

The two-day program focuses on practical exchange between research and industry.
Participating companies will introduce concrete challenges, including their context,
constraints and desired outcomes. Researchers and company representatives will then work
in small interdisciplinary groups to analyze these challenges, connect them with relevant
AI methods, and develop possible solution concepts and next steps.

The goal is not only to discuss AI applications, but also to create opportunities for
research collaborations, thesis projects, internships, pilot projects and longer-term
partnerships.

{% include photo-strip.html photos=site.data.gallery %}

## Who takes part

- Master's students working on or interested in AI
- Doctoral researchers in AI and related fields

Participants come from Germany and neighboring European countries.

## Format

<ul class="format-list">
  <li><strong>Keynote talks</strong>Talks from research and industry to frame the two days.</li>
  <li><strong>Company pitches</strong>Companies present concrete challenges, with context, constraints and desired outcomes.</li>
  <li><strong>Working sessions</strong>Small interdisciplinary groups analyze a challenge and map it to AI methods.</li>
  <li><strong>Project presentations</strong>Groups present solution concepts and proposed next steps.</li>
  <li><strong>Networking</strong>Time to set up collaborations, thesis projects, internships and pilots.</li>
</ul>

See the [program page]({{ "/program/" | relative_url }}) for the two-day schedule.

## Participating companies

Each company brings one concrete challenge for the working groups.

{% include logo-grid.html logos=site.data.companies empty="To be announced." %}

## Speakers

{% include people-grid.html people=site.data.speakers dir="speakers" empty="To be announced." %}

## Organizers

{% include organizer-teams.html teams=site.data.organizer_teams %}

</div>
