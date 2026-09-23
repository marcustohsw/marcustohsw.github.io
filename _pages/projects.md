---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
description: "Explore Marcus Toh's projects in software, AI, and robotics."
---

A selection of my personal, academic, and internship projects. Open a project to read about its purpose and my contributions.

<div class="project-previews">
  {% assign projects = site.projects | sort: 'order' %}
  {% for project in projects %}
  <article class="project-preview" id="{{ project.slug | escape }}" aria-labelledby="{{ project.slug | escape }}-title">
    <p class="project-preview-context">{{ project.context | escape }}</p>
    <h2 id="{{ project.slug | escape }}-title"><a href="{{ project.url | relative_url }}">{{ project.title | escape }}</a></h2>
    <p>{{ project.excerpt | strip_html | escape }}</p>
    <a class="project-read-more" href="{{ project.url | relative_url }}" aria-label="Read More about {{ project.title | escape }}">Read More <span aria-hidden="true">&rarr;</span></a>
  </article>
  {% endfor %}
</div>

<style>
.project-previews { margin-top: 2rem; }
.project-preview { padding: 1.5rem 0; border-top: 1px solid #d5d9dc; scroll-margin-top: 5rem; }
.project-preview .project-preview-context { margin: 0 0 0.5rem; font-size: 0.75em; }
.project-preview h2 { margin: 0 0 0.6rem; padding: 0; border: 0; font-size: 1.3em; }
.project-preview h2 a { color: inherit; text-decoration: none; }
.project-preview h2 a:hover { text-decoration: underline; }
.project-preview > p { margin-bottom: 0.75rem; }
.project-read-more { font-size: 0.85em; font-weight: 600; }
.project-preview a:focus-visible { outline: 3px solid #287b91; outline-offset: 4px; }
</style>
