---
layout: default
title: Homepage
---


# About me

I am an archaeologist whose research focuses on prehistoric archaeology, currently on the Neolithic of northern Central Europe / South Scandinavia, and of the Swiss lakeshore settlements. I received my PhD from [Kiel University](http://www.uni-kiel.de) within the [Graduate School 'Human Development in Landscape'](http://www.gshdl.uni-kiel.de) in 2011. Until 2016 I was Assistent Coordinator at the [DFG Priority Programme 1400 'Early Monumentality and Social Differentiation'](http://www.monument.ufg.uni-kiel.de/). 2016-2018 I worked as postdoc in the [Project F1](https://www.sfb1266.uni-kiel.de/en/projects/cluster-f/f1-supra-regional-crises) of the [CRC1266 "Scales of Transformation"](https://www.sfb1266.uni-kiel.de). Currently I am a senior researcher (Oberassistent) at the [Institute for Archaeological Sciences (IAS)](http://www.iaw.unibe.ch/) at the University of Bern.

I regard quantitative methods as essential for archaeological research. That is why they represent a substantial aspect of my toolkit. This includes statistical analysis, spatial technologies (including GIS and spatial statistics), and dynamic modeling. You may find some [screencasts](/screencasts/) and other [posts](/blog/) regarding statistical method on this website.

One other main aspect is Open Data. I am leading developer of [RADON](http://radon.ufg.uni-kiel.de) and [RADON-B](http://radon-b.ufg.uni-kiel.de), which are among the largest repositories for <sup>14</sup>C data for archaeology.

I am very interested in human-environmental interactions and the questions of population development in the Neolithic and Bronze Age.

<div class="pure-g">
<div class="pure-u-1 pure-u-lg-1-2 l-box" markdown="1">

## Interests:
* Archaeology of the Neolithic and early Bronze Age
* Quantitative methods and statistics
* Theoretical archaeology
* Lakeshore settlements ('Pile Dwellings')
* Megalithic
* Radiocarbon dates
* Demographic analysis
* Agent based simulations
* Predictive modelling/mapping
* Spatial Statistics/Simulations
* Software development for archaeological applications
* Reproducible research & Open science
</div>
<div class="pure-u-1 pure-u-lg-1-2 l-box" markdown="1">
## Education:

* MA in Archaeology, 2008
  * Kiel University 
* PhD in Archaeology, 2011
  * Kiel University
</div>
</div>

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

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

{% contentfor rightsidebar %}
<div class="personal-details">
{% include personal_details.html %}
</div>
{% endcontentfor %}
