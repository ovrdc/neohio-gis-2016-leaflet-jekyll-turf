---
layout: default
---

<div class="home">
  <br /><br />
  <h1>his site contains examples from the presentation at the Northeast Ohio GIS Symposium on Leaflet, Jekyll and TurfJS. View the full presentation <a href="https://getbounds.com/slides/neohio-gis-2016-leaflet-jekyll-turfjs/" target="ext">here</a>.</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl | remove:'index.html' }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>
