---
layout: default
title: Welcome
---

# Welcome to My Website

This site was built using **Jekyll** and the **Midnight theme**.  
Feel free to explore and modify it as you like!

---

## 📄 Pages

<ul>
  {% for page in site.pages %}
    {% if page.title and page.permalink != "/" %}
      <li><a href="{{ page.url }}">{{ page.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

---

## 📝 Blog Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
