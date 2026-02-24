---
title: "Introduction to Machine Learning"
collection: teaching
type: "Workshop"
permalink: /teaching/2024-fall-ML-SMiP
venue: "SMiP, University of Tübingen"
date: 2024-12-19
location: "Tübingen, Germany"
---

<!-- {% include base_path %} -->

<!-- naive password protection -->
<script>
    const password = "smip24";

    document.addEventListener("DOMContentLoaded", function() {
        const userPassword = prompt("Enter password to access this page:");
        if (userPassword !== password) {
            document.body.innerHTML = "<h1>Access denied</h1>";
        }
    });
</script>


## Syllabus

- [Syllabus.pdf](/files/teaching/2024-fall-ML-SMiP/syllabus.pdf)


## Slides

<ul>
  {% for file in site.static_files %}
    {% if file.path contains '/files/teaching/2024-fall-ML-SMiP/Slides' %}
      <li><a href="{{ file.path | relative_url }}">{{ file.name }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

<ul>
  {% assign folder_pages = site.pages | where_exp: "item", "item.path contains 'files/'" %}
  {% for p in folder_pages %}
    {% if p.path contains '.Rmd' %}
      <li>
        <a href="{{ p.url | relative_url }}">
          {{ p.title | default: p.name }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>


## Tutorials

<ul>
  {% for file in site.static_files %}
    {% if file.path contains '/files/teaching/2024-fall-ML-SMiP/Tutorials' %}
      <li><a href="{{ file.path | relative_url }}">{{ file.name }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

<!-- ALT: GDrive integration

## Slides
- <a href="https://drive.google.com/drive/folders/1-t7K_oENLJ54192cjvTejiuZXjPfsJXv?usp=drive_link">Download all slides here</a>

<iframe src="https://drive.google.com/embeddedfolderview?id=1-t7K_oENLJ54192cjvTejiuZXjPfsJXv#list" style="width:90%; height:300px;"></iframe>


## Tutorials

- <a href="https://drive.google.com/drive/folders/10EiREBfzM1-9niTGqHaFZlasS8-dqRF0?usp=drive_link">Download all tutorial materials here</a>

<iframe src="https://drive.google.com/embeddedfolderview?id=10EiREBfzM1-9niTGqHaFZlasS8-dqRF0#list" style="width:90%; height:300px;"></iframe>

-->