---
layout: default
title: scientificproductivity.github.io
tagline: Reproducible research in biomedical sciences
---
{% include JB/setup %}
### Latest Blog Post ###
{% for post in site.posts limit:5 %}
  <p>
    <strong><a href="{{ post.url }}">{{ post.title | xml_escape }}</a></strong>
    <span>
    	<em><time datetime="{{ post.date | date: "%Y-%m-%d" }}">
    		{{ post.date | date: "%B %d, %Y" }}
    	</time></em>
    </span>
  <br />{{ post.content | split:"<!--more-->" | strip_html | truncatewords: 50 }} <a href="{{ post.url }}">continue reading...</a>
  </p>
{% endfor %}

[More blog posts](/blog.html)
    
## More to Come
I am planning to post several tips on R programming in biomedical research regarding reproducibility. 
Stay tuned.
## How to use custom domain name to point my github.com pages?
I am trying to figure out how to point domain (like [Scientific Productivity](www.scientificproductivity.com)) to my github pages.





