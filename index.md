---
layout: default
---

<div class="home">
  <h1 class="page-heading">Latest Posts: </h1>
  <ul class="post-list">
    {% for post in site.posts %}
    {% assign author = site.data.authors[post.author] %}
    
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        {% if post.author %}<a href='{{site.url}}/participants/{{page.author}}/'>{{ author.display_name }}</a>{% endif %}
        
        <h2><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        {% if post.tags != empty %}
          <div class='post-meta'>
            Tags: 
              {% for tag in post.tags %}
                <span>{{ tag }}</span>
              {% endfor %}
            </div>
        {% endif %}
        
      </li>
    {% endfor %}
  </ul>

</div>
