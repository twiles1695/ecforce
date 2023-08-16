# URLによる条件分岐

```liquid
{% assign url_path = page_url | remove: site_url %}
{% if url_path contains '/shop/pages/about' %}
  aboutページのみに表示する記述
{% endif %}
```