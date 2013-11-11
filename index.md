---
layout: page
title: AguDev
tagline: dev pages
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>

<article class="unit-article layout-post">
    <div class="unit-inner unit-article-inner">
        <div class="content">
            <div class="bd">
                <div class="entry-content">
                    {{ post.content }}
                </div><!-- entry-content -->
            </div><!-- bd -->
        </div><!-- content -->
    </div><!-- unit-inner -->
</article>

  {% endfor %}
</ul>


