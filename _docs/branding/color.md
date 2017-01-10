---
title: Color
info: Colors used in this product.
---

<section class="sg-branding">
  {% for group in page.colors %}
  <div>
    <h3>{{ group.name | capitalize }}</h3>
    <ul class="color-set">
    {% for item in group.items %}
      <li>
        <div style="background:#{{ item.hex }}"></div>
        <p><code>{{ item.name }}</code></p>
        {% if item.hex %}<p>#{{ item.hex }}</p>{% endif %}
        {% if item.pretty %}<p>{{ item.pretty }}</p>{% endif %}
        {% if item.rgb %}<p>{{ item.rgb }}</p>{% endif %}
      </li>
    {% endfor %}
    </ul>
  </div>
  {% endfor %}
</section>

<section>
  <p>bla keks</p>
</section>