---
layout: default
title: "UnitedCTF"
---

**UnitedCTF** est une compétition informatique universitaire dans le format d'un **[CTF](#quest-ce-quun-ctf)**, proposant une multitude de défis de programmation et de sécurité informatique. 

Cette année, le niveau de la compétition sera très orienté vers les débutants et débutantes afin de les initier au monde des CTF!
 
**UnitedCTF** est une collaboration des clubs informatiques universitaires suivants:
<ul>  
  {% for club in site.data.clubs %}
  <li>
    <b><a href="{{ club.url }}">{{ club.name }}</a></b> de {{ club.university_name }}
  </li>
  {% endfor %}
</ul>

{% if site.ctf.display %}
# {{ site.ctf.name }}

Le {{ site.ctf.name }} aura lieu du <b>{{ site.ctf.date_start }}</b> au <b>{{ site.ctf.date_end }}</b>. 

{% if site.ctf.registration_enabled %}
 [Inscription]({{ site.ctf.url }})
{% else %}
Ajoutez-le à votre calendrier!
{% endif %}
{% endif %}

# Rejoignez la discussion

Si ce n'est pas déjà fait, inscrivez-vous sur notre groupe Slack pour rester à l'affût de toutes les annonces en lien au UnitedCTF!

- [Lien pour s'inscrire au groupe Slack]({{ site.slack_inscription_url }})
- [Lien du groupe Slack]({{ site.slack_url }}) (pour ceux et celles déjà inscrit.e.s)

# Qu'est-ce qu'un CTF?

Un **CTF**, sigle de **[Capture The Flag](https://fr.wikipedia.org/wiki/Capture_du_drapeau#En_s%C3%A9curit%C3%A9_de_l'information)** (_Capture du drapeau_), est une compétition informatique dont le but est d'obtenir le plus de points. Les points sont ramassés en soumettant des *flags* dans le système de pointage. Un drapeau est une chaîne de caractère secrète, que l'on obtient lorsque l'on résout un défi.

