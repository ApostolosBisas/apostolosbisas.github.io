---
layout: single
permalink: /debug/
---

# Debugging Publications Collection

This page is for testing the `site.publications` collection.

The number of publications found is: **{{ site.publications | size }}**.

---

{% for pub in site.publications %}
## Title: {{ pub.title }}

- **Path:** `{{ pub.path }}`
- **URL:** `{{ pub.url }}`
- **Category:** `{{ pub.category }}`
- **Date:** `{{ pub.date }}`
<hr>
{% else %}
<p><strong>Conclusion: The `site.publications` collection is empty.</strong></p>
{% endfor %}
