---
title: "Kontakt"
layout: splash
excerpt: "Kontaktieren Sie mich für ein unverbindliches Gespräch. Ich freue mich."
permalink: /kontakt/
author_profile: false
header:
  overlay_image: /assets/images/kontakt/img_20160907_152429-1600.jpg
  # caption: "Bild: [**Siegfried, Heinrich**, 1884](https://commons.wikimedia.org/wiki/File:Zentralbibliothek_Z%C3%BCrich_-_Vue_g%C3%A9n%C3%A9rale_de_Zurich_prise_de_la_Weid_-_000009549.jpg#)"
---
{% include base_path %}

{% if page.author and site.data.authors[page.author] %}
  {% assign author = site.data.authors[page.author] %}{% else %}{% assign author = site.author %}
{% endif %}

Roger Schärer <br>
<a target="_blank" href="{{ author.location-uri }}">Weingartenstrasse 35<br>
8708 Männedorf</a>



<ul style="list-style-type:none; padding-left:0;">
  {% if author.phone %}
    <li><i class="fa fa-fw fa-phone" aria-hidden="true"></i> {{ author.phone }}</li>
  {% endif %}
  {% if author.email %}
    <li><a href="mailto:{{ author.email }}"><i class="fa fa-fw fa-envelope-square" aria-hidden="true"></i> {{ author.email }}</a></li>
  {% endif %}
  {% if author.uri %}
    <li>
      <a href="{{ author.uri }}" itemprop="url">
        <i class="fas fa-fw fa-link" aria-hidden="true"></i> {{ author.uri | remove:"http://" | remove: "https://" }}
      </a>
    </li>
  {% endif %}
</ul>
