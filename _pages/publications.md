---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
nav: true
nav_order: 2
_styles: >
  h2 { margin-top: 2.5rem; }
---

{% include bib_search.liquid %}

## Journal Articles

<div class="publications">
{% bibliography --query @article[keywords!=abstract] %}
</div>

## Book Chapters

<div class="publications">
{% bibliography --query @incollection %}
</div>

## Conference Abstracts

<div class="publications">
{% bibliography --query @inproceedings[keywords=abstract] %}
</div>

## Thesis

<div class="publications">
{% bibliography --query @phdthesis %}
</div>
