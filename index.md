---
layout: default
title: Martin Hinz
---

<div class="odd_row about_me" markdown="1" >

# About me

I am an archaeologist whose research focuses on prehistoric archaeology, working on the prehistory of northern Central Europe / South Scandinavia and the Swiss lakeshore settlements, interested in human-environmental interactions and  population development in the Neolithic and Bronze Age. Currently I am a senior researcher (Oberassistent) at the [Institute for Archaeological Sciences (IAW)](http://www.iaw.unibe.ch/) at the University of Bern.

I am editor of the [Journal of Neolithic Archaeology](http://www.j-n-a.org) and of the [Journal of Glacial Archaeology](https://journal.equinoxpub.com/JGA), and also member of the editorial board of the [Journal of Computer Applications in Archaeology](https://journal.caa-international.org). I am also convener of the [CAA SIG Scientific Scripting Languages in Archaeology](https://sslarch.github.io/) and secretary of the [CAA National Chapter Switzerland](https://caa-switzerland.ch).

I regard quantitative methods as essential for archaeological research. That is why they represent a substantial aspect of my toolkit. This includes statistical analysis, spatial technologies (including GIS and spatial statistics), and dynamic modeling. You may find some [screencasts](/screencasts/) and other [posts](/blog/) regarding statistical method on this website.

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
* Spatial Statistics/Simulations
* Software development for archaeological applications
* Reproducible Research & Open science
</div>

<div class="pure-u-1 pure-u-lg-1-2 l-box" markdown="1">
## Education:

* MA in Archaeology, 2008
  * Kiel University
* PhD in Archaeology, 2011
  * Kiel University
</div>
</div>

</div>

<div class="even_row" markdown="1" >
<div class="pure-u-1 pure-u-md-1-2 l-box" markdown="1" style="margin-left: 25%;">

# Publications (since 2015)
{: #publications}

{% bibliography --file 0000-0002-9904-6548 --group_by year --group_order descending -q @*[year>=2015] %}

For full publication list visit [publications](/publications)
</div>
</div>

# Latest Blog Post

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

{% contentfor leftsidebar %}
<div class="personal-details">
{% include personal_details.html %}
</div>
{% endcontentfor %}
