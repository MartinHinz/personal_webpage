---
layout: default
title: Homepage
---


# What is this all about?

I am an archaeologist whose research focuses on prehistoric archaeology, currently on the Neolithic of northern Central Europe / South Scandinavia. I received my PhD from [Kiel University](http://www.uni-kiel.de) within the [Graduate School 'Human Development in Landscape'](http://www.gshdl.uni-kiel.de) in 2011. Until 2016 I was Assistent Coordinator at the [DFG Priority Programme 1400 'Early Monumentality and Social Differentiation'](http://www.monument.ufg.uni-kiel.de/). Since then I am working as postdoc in the [Project F1](https://www.sfb1266.uni-kiel.de/en/projects/cluster-f/f1-supra-regional-crises) of the [CRC1266 "Scales of Transformation"](https://www.sfb1266.uni-kiel.de).

I regard quantitative methods as essential for archaeological research. That is why they represent a substantial aspect of my toolkit. This includes statistical analysis, spatial technologies (including GIS and spatial statistics), and dynamic modeling. You may find some [screencasts](/screencasts/) and other [posts](/blog/) regarding statistical method on this website.

One other main aspect is Open Data. I am leading developer of [RADON](http://radon.ufg.uni-kiel.de) and [RADON-B](http://radon-b.ufg.uni-kiel.de), which are among the largest repositories for <sup>14</sup>C data for archaeology.

I hope you may find some material of my website informative and that it probably may help with your own work.

<div class="pure-g">
<div class="pure-u-1 pure-u-lg-1-2 l-box" markdown="1">

## Latest Blog Post

{% assign blog_posts = site.categories['blog'] %}
<ul class="post-list">
{% for post in blog_posts limit:3 %}
  <li>
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      {{ post.excerpt }}
  </li>
{% endfor %}
</ul>
Find more at the [blog section](/blog/)...

</div>

<div class="pure-u-1 pure-u-lg-1-2 l-box" markdown="1">

## Latest Screencasts

{% assign screencasts = site.categories['screencast'] %}
<ul class="post-list">
{% for screencast in screencasts limit:3 %}
  <li>
    <span class="post-meta">Series: {{screencast.series}} | Episode: {{screencast.episode_nr}} - {{ screencast.date | date: "%b %-d, %Y" }}</span>
      <a href="{{ screencast.url | prepend: site.baseurl }}">{{ screencast.title }}</a>
      {{ screencast.excerpt }}
  </li>
{% endfor %}
</ul>
Find more at the [screencast section](/screencasts/)...
</div>
</div>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

{% contentfor rightsidebar %}
<div class="personal-details">
{% include personal_details.html %}
</div>
{% endcontentfor %}


