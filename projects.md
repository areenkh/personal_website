---
layout: page
permalink: /projects/
title: Projects
class: projects
---

# Projects

<!-- {:.lead} -->

You can find the code and other cool projects on my [GitHub](https://github.com/areenkh).

{% assign projtypes = site.data.projects | group_by:"type"  %}
{% assign sorted_projtypes = projtypes %}
{% for type in sorted_projtypes %}

<!-- <h2 id="{{ type.name | replace: ' ', '-' | replace: '(', '' | replace: ')', '' }}">{{ type.name }}</h2> -->
<div class="grid">
  <!-- do not uncomment ((start)){% for project in site.data.projects %}
    {% include project.html project=project %}
  {% endfor %} Do not uncomment this one out later ((end))-->
  {% for project in type.items %}
  {% include project.html project=project %}
  {% endfor %}
</div> 
{% endfor %}
