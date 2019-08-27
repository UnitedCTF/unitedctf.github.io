---
layout: default
title: "UnitedCTF"
---

**UnitedCTF** est compétition amicale informatique dans le format d'un [CTF](https://fr.wikipedia.org/wiki/Capture_du_drapeau#En_s%C3%A9curit%C3%A9_de_l'information), proposant une multitude de défis de programmation et de sécurité. 

Le niveau de difficulté des défis varie de _très facile_ à _difficile_. Cette compétition est donc idéale pour les personnes débutantes en informatique, n'ayant jamais fait de compétition informatique, de même que pour les personnes déjà initiée.
 
**UnitedCTF** est une collaboration des clubs informatiques universitaires suivants:
<ul>  
  {% for club in site.data.clubs %}
  <li>
    <a href="{{ club.url }}">{{ club.name }}</a> de {{ club.university_name }}
  </li>
  {% endfor %}
</ul>



## Qu'est-ce qu'un CTF

Un [«Capture the Flag (CTF)»](https://fr.wikipedia.org/wiki/Capture_du_drapeau#En_s%C3%A9curit%C3%A9_de_l'information) (en français **Capture du drapeau**) est une compétition informatique où le but est d'obtenir le plus de points. Les points sont ramassés en soumettant des drapeaux dans le système de pointage. Un drapeau est une chaîne de caractère secrète, que l'on obtient lorsqu'on résout un défi.

{% if site.ctf.display %}
## {{ site.ctf.name | capitalize }}

- [Inscription]({{ site.ctf.url }})
- {{ site.ctf.date }}
{% endif %}
