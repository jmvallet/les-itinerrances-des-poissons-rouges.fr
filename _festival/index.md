---
layout: default
title: "Le festival"
description: "Le festival d'art comptemporain « Les itinerrances des poissons rouges » a lieu dans le bassin Valentinois depuis 2010 au mois de juin"
social_image: social.jpg
---

<h2>Le festival</h2>
<p>
  Organisé par l'association « Les Itinerrances », le festival d'art comptemporain « Les itinerrances des poissons rouges » a lieu dans le bassin Valentinois depuis 2010 au mois de juin. Retrouvez ci-dessous les affiches des 9 éditions passées.
</p>

<ul class="festivals">
  {% for fest in site.festival reversed %}
    {% if fest.layout == 'festival' %}
      <li>
        <h3><span>{{fest.year}}</span></h3>
        <img src="{{ fest.path|remove:'_festival/'|split: '/'|first}}/affiche.jpg" />
        {% for link in fest.links %}
          <a href="{{fest.url|remove:'index.html'}}{{ link.path }}"><span>{{link.name}}</span></a>
        {% endfor %}
      </li>
    {% endif %}
  {% endfor %}
</ul>
