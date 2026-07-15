---
layout: archive
title: "Advising & Thesis Committees"
permalink: /advising/
author_profile: true
---

{% include base_path %}

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
