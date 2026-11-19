---
layout: about
title: About
permalink: /
subtitle: Senior Research Engineer · Saint-Gobain Research North America · Cambridge, MA

profile:
  align: right
  image: prof_pic.jpg
  image_circular: true # crops the image to make it circular

selected_papers: false # the Publications section is rendered in the page body below
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # the News section is rendered in the page body below

latest_posts:
  enabled: false
---

## About

I build numerical and analytical models of structures and materials, calibrate them against mechanical tests, and use them to design aerospace parts. I hold a PhD in Mechanical Engineering & Applied Mechanics from the [University of Pennsylvania](https://www.me.upenn.edu/).

## Work

- **Aircraft windshields:** finite-element models that set load cases and guide load-bearing designs.
- **Knitted composites:** material models that enabled a 50% weight reduction on a redesigned part.
- **Adhesion (PhD):** shape optimization of adhesive pillars, lap joints, and attachment structures.

## Interests

Finite element analysis · Fracture & adhesion mechanics · Material modeling · Design optimization

## News

<div class="news">
  <table class="table table-sm table-borderless">
    {% assign news = site.news | reverse %}
    {% for item in news %}
      <tr>
        <th scope="row" style="width: 20%">{{ item.date | date: '%b %Y' }}</th>
        <td>{{ item.content | remove: '<p>' | remove: '</p>' }}</td>
      </tr>
    {% endfor %}
  </table>
</div>

## Publications

<div class="publications">
  {% bibliography --group_by none --query @*[selected=true]* %}
</div>
