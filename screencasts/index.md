---
layout: page
title: Screencasts
permalink: /screencasts/
---

* TOC
{:toc}

{% assign screencasts = site.categories['screencast'] %}

# Predictive Modelling
In dieser Reihe geht es um weiterführende Funktionen, die unter anderem für "predictive modelling" Verwendung finden. Ein Kurs zu diesem Thema bildet den Hintergrund.

<ul class="post-list">
  {% assign predmap = (screencasts | where: "series" , "predictive_modelling" | sort: 'episode_nr', 'last') %}
  {% for post in predmap %}
    <li>
      <span class="post-meta">Episode: {{post.episode_nr}} - {{ post.date | date: "%b %-d, %Y" }}</span>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

# Statistik mit R

<ul class="post-list">
  {% assign predmap = (screencasts | where: "series" , "statistik_mit_r" | sort: 'episode_nr', 'last') %}
  {% for post in predmap %}
    <li>
      <span class="post-meta">Episode: {{post.episode_nr}} - {{ post.date | date: "%b %-d, %Y" }}</span>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

# Korrespondenzanalyse

Die folgenden Videos beschreiben die Funktionsweise der Korrespondenzanalyse und ihre Durchführung mittels verschiedener Programme.

<ul class="post-list">
  {% assign predmap = (screencasts | where: "series" , "korrespondenzanalyse" | sort: 'episode_nr', 'last') %}
  {% for post in predmap %}
    <li>
      <span class="post-meta">Episode: {{post.episode_nr}} - {{ post.date | date: "%b %-d, %Y" }}</span>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
