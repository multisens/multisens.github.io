---
layout: page
title: Nossos Produtos
description: "Conheça as soluções desenvolvidas pelo laboratório."
nav-menu: true
---

<section id="one" class="tiles">
  {% for product in site.products %}
    <article>
      <span class="image">
        <img src="{{ product.image | relative_url }}" alt="" />
      </span>
      <header class="major">
        <h3><a href="{{ product.url | relative_url }}" class="link">{{ product.title }}</a></h3>
        <p>{{ product.description }}</p>
      </header>
    </article>
  {% endfor %}
</section>