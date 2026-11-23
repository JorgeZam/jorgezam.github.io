---
layout: archive
title: "Advising & Thesis Committees"
permalink: /advising/
author_profile: true
---

{% include base_path %}
{% include hero_layout %}

{% if hero_layout %}
{% comment %}Each category as a heading with its count over a two-column grid, as on Teaching; same order as below{% endcomment %}
{% for category in site.advising_category %}
{% assign items = site.advising | where: "category", category[0] | reverse %}
{% if items.size > 0 %}
<h2 class="pub-section">{{ category[1].title }} <span class="pub-section__count">({{ items.size }})</span></h2>
<div class="item-grid">{% for post in items %}{% include archive-single.html %}{% endfor %}</div>
{% endif %}
{% endfor %}

{% for category in site.committee_category %}
{% assign items = site.committees | where: "category", category[0] | reverse %}
{% if items.size > 0 %}
<h2 class="pub-section">{{ category[1].title }} <span class="pub-section__count">({{ items.size }})</span></h2>
<div class="item-grid">{% for post in items %}{% include archive-single.html %}{% endfor %}</div>
{% endif %}
{% endfor %}
{% else %}

<h2>Advising</h2>

{% for category in site.advising_category %}
{% assign title_shown = false %}
{% for post in site.advising reversed %}
{% if post.category != category[0] %}
{% continue %}
{% endif %}
{% unless title_shown %}
<h3>{{ category[1].title }}</h3>
{% assign title_shown = true %}
{% endunless %}
{% include archive-single.html %}
{% endfor %}
{% endfor %}

<h2>Thesis Committees</h2>

{% for category in site.committee_category %}
{% assign title_shown = false %}
{% for post in site.committees reversed %}
{% if post.category != category[0] %}
{% continue %}
{% endif %}
{% unless title_shown %}
<h3>{{ category[1].title }}</h3>
{% assign title_shown = true %}
{% endunless %}
{% include archive-single.html %}
{% endfor %}
{% endfor %}
{% endif %}
