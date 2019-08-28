---
layout: default
title: "UnitedCTF"
---

**UnitedCTF** est une compétition amicale informatique dans le format d'un [CTF](https://fr.wikipedia.org/wiki/Capture_du_drapeau#En_s%C3%A9curit%C3%A9_de_l'information), proposant une multitude de défis de programmation et de sécurité. 

Le niveau de difficulté des défis varie de _très facile_ à _difficile_. Cette compétition est donc idéale pour les personnes débutantes en informatique, n'ayant jamais fait de compétition, de même que pour les personnes déjà initiées.
 
**UnitedCTF** est une collaboration des clubs informatiques universitaires suivants:
<ul>  
  {% for club in site.data.clubs %}
  <li>
    <a href="{{ club.url }}">{{ club.name }}</a> de {{ club.university_name }}
  </li>
  {% endfor %}
</ul>



## Qu'est-ce qu'un CTF?

Un **CTF**, abbreviation de **[Capture The Flag](https://fr.wikipedia.org/wiki/Capture_du_drapeau#En_s%C3%A9curit%C3%A9_de_l'information)** (_Capture du drapeau_), est une compétition informatique dont le but est d'obtenir le plus de points. Les points sont ramassés en soumettant des drapeaux dans le système de pointage. Un drapeau est une chaîne de caractère secrète, que l'on obtient lorsque l'on résout un défi.

{% if site.ctf.display %}
## {{ site.ctf.name | capitalize }}

- {{ site.ctf.date }}
- [Inscrivez vous]({{ site.ctf.url }})
- [Rejoignez notre Slack]({{ site.slack_inscription_url }})
{% endif %}
