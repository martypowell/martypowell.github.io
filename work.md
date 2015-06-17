---
layout: large
title: My Work
permalink: /work/
---
<h1>{{ page.title }}</h1>

  <ul class="latest-work">
    {% for post in site.posts %}
      {% if post.category == "work" %}
      <li class="latest-work-item">
        <figure class="list__item__inner">
          <a class="post-link link-image" href="{{ post.url | prepend: site.baseurl }}"><img src="{{ post.thumbnail}}" alt="View more infomration about {{ post.title }}" /></a>
          <figcaption><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </figcaption></figure>
      </li>
        {% endif %}
    {% endfor %}
  </ul>

<p>*View more of my work and skills on <a href="https://www.linkedin.com/in/jeffreymartinpowelljr" title="View more of my work on LinkedIn">LinkedIn</a></p>



