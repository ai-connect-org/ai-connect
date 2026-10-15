---
layout: default
---

<div class="home" markdown="1">

<div class="hero" markdown="1">

# **{{ site.event.name }}**

<div class="key-facts" markdown="1">
**Dates:** {{ site.event.dates }} <br>
**Location:** {{ site.event.venue }}, {{ site.event.city }} <br>
**Applications:** via the [application form]({{ site.event.apply_url }}) <br>
**Application deadline:** {{ site.event.application_deadline }}
{%- if site.event.contact_email != "" %} <br>
**Contact:** [{{ site.event.contact_email }}](mailto:{{ site.event.contact_email }})
{%- endif %}
</div>

{% include logo-strip.html %}

<div class="news-box">
  <div class="news-title">Applications are open!</div>
  <div>
    Two days of exchange between research and industry at {{ site.event.venue }}, Aachen.<br>
    Keynotes, company pitches, collaborative working sessions and networking.
  </div>
  <a class="btn-apply" href="{{ site.event.apply_url }}">Apply now</a>
</div>

</div>

## About

We invite applications for **{{ site.event.name }}**, taking place on
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

## Who should apply

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

The detailed schedule will be published on the [program page]({{ "/program/" | relative_url }}).

## Participating companies

Each company brings one concrete challenge for the working groups. You can state a preference
in the application form; final team assignment depends on balance across the groups.

{% include logo-grid.html logos=site.data.companies empty="To be announced." %}

## Keynote speakers

{% include people-grid.html people=site.data.speakers dir="speakers" empty="To be announced." %}

{% if site.data.committee.size > 0 %}
## Organizing committee

{% include people-grid.html people=site.data.committee dir="people" %}
{% endif %}

## Apply

In your application, please tell us about your academic or professional background,
your area of expertise, and what you hope to contribute to and gain from the event.

Before completing the form, please check that:

<ul class="checklist">
  <li>you are available in Aachen on 26 and 27 November 2026;</li>
  <li>you are willing to participate actively in the collaborative working sessions;</li>
  <li>you understand that submitting the form expresses interest in participating and is not a confirmation of acceptance.</li>
</ul>

Applications are reviewed by the organizing team. Selected participants will receive
further information about participation, travel support, accommodation and the detailed
program separately.

<p><a class="btn-apply" href="{{ site.event.apply_url }}">Open the application form</a></p>

## Venue

The event takes place at **{{ site.event.venue }}**, {{ site.event.address }}.
Selected participants will receive information about travel support and accommodation
separately.

<iframe class="map-embed" loading="lazy" referrerpolicy="no-referrer-when-downgrade"
  src="https://www.google.com/maps/embed?origin=mfe&pb=!1m3!2m1!1sBurg+Frankenberg,+Bismarckstra%C3%9Fe+68,+52066+Aachen!6i15"
  title="Map of Burg Frankenberg, Aachen"></iframe>

</div>
