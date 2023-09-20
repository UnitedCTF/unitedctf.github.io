---
layout: default
title: "UnitedCTF"
---

**UnitedCTF** est une compétition informatique universitaire dans le format d'un **[CTF](#quest-ce-quun-ctf)**, proposant une multitude de défis de programmation et de sécurité informatique.

Cette année, le niveau de la compétition est orienté vers les débutants et débutantes afin de les initier au monde des CTF!

**UnitedCTF** est une collaboration des clubs informatiques universitaires suivants:
<ul>  
  {% for club in site.data.clubs %}
  <li>
    {% if club.url %}
      <b><a href="{{ club.url }}">{{ club.name }}</a></b> de {{ club.university_name }}
    {% else %}
      <b>{{ club.name }}</b> de {{ club.university_name }}
    {% endif %}
  </li>
  {% endfor %}
</ul>

{% if site.ctf.display %}

## {{ site.ctf.name }}

Le {{ site.ctf.name }} aura lieu du <b>{{ site.ctf.date_start }}</b> au <b>{{ site.ctf.date_end }}</b>.

{% if site.ctf.registration_enabled %}
 [Inscription]({{ site.ctf.url }})
{% else %}
Ajoutez-le à votre calendrier!
{% endif %}
{% endif %}

## Rejoignez la discussion

Si ce n'est pas déjà fait, inscrivez-vous sur notre serveur Discord pour rester à l'affût de toutes les annonces en lien au UnitedCTF!

- [Lien pour joindre notre serveur Discord]({{ site.discord_invite_link }})

## Qu'est-ce qu'un CTF?

Un **CTF**, sigle de **[Capture The Flag](https://fr.wikipedia.org/wiki/Capture_du_drapeau#En_s%C3%A9curit%C3%A9_de_l'information)** (_Capture du drapeau_), est une compétition informatique dont le but est d'obtenir le plus de points. Les points sont ramassés en soumettant des _flags_ dans le système de pointage. Un drapeau est une chaîne de caractère secrète, que l'on obtient lorsque l'on résout un défi.

## Ressources utiles

  <ul>
    <li><a href="https://www.google.com" target="_blank">Google</a>! Sérieusement, utiliser Google (ou n'importe quel autre moteur de recherches) pour faire des recherches sur tout ce que vous ne savez pas dans un CTF est la meilleure habitude à prendre.</li>
    <li><a href="https://gchq.github.io/CyberChef/" target="_blank">CyberChef</a>: un outil en ligne pour faire des
        opérations de cryptographie ou de conversion d'un encodage à un autre (e.g: décoder de l'hexadécimal / base64). Il
        est même possible d'enchaîner plusieurs transformations!</li>
    <li><a href="https://github.com/gchq/CyberChef#how-it-works" target="_blank">CyberChef: How it works</a>: explications
        et exemples d'utilisation de CyberChef.</li>
    <li><a href="https://docs.google.com/presentation/d/11IYBrpSES1l3gUTqPEQs7TsR9ngiUphuOWH0sBaxtKs/edit?usp=sharing"
            target="_blank">Présentation "Compétition Informatique 101"</a> par le club CFIUL.</li>
    <li><a href="https://ctf101.org/" target="_blank">CTF 101</a>: des explications sur les catégories et concepts qu'on
        retrouve souvent dans les CTFs.</li>
    <li><a href="https://ryanstutorials.net/linuxtutorial/" target="_blank">Linux Tutorial for Beginners</a></li>
    <li><a href="https://www.mathsisfun.com/hexadecimals.html" target="_blank">Hexadecimals</a></li>
    <li><a href="https://www.lifewire.com/base64-encoding-overview-1166412" target="_blank">How Base64 Encoding Works</a>
    </li>
    <li><a href="https://beginnersbook.com/2015/04/json-tutorial/" target="_blank">Learn JSON in 10 Minutes</a></li>
    <li><a href="https://docs.oracle.com/javase/tutorial/networking/sockets/definition.html" target="_blank">What Is a
            Socket?</a></li>
    <li><a href="https://www.varonis.com/blog/how-to-use-wireshark/" target="_blank">How to Use Wireshark</a></li>
    <li><a href="https://www.varonis.com/blog/how-to-use-ghidra" target="_blank">How to Use Ghidra</a></li>
    <li><a href="https://www.geeksforgeeks.org/gdb-step-by-step-introduction/" target="_blank">How to Use GDB</a></li>
  </ul>

## Partenaires

Merci à nos partenaires!

  <div class="sponsors">
  {% for sponsor in site.data.sponsors %}
    <div class="sponsor">
      <a href="{{ sponsor.url }}" target="_blank">
        <img width="{{ sponsor.image_width }}" src="{{ sponsor.image_url }}" alt="{{ sponsor.name }}"/>
      </a>
    </div>
  {% endfor %}
  </div>

  <!-- Notre infrastructure est commanditée par :
  <div class="sponsors">
  {% for sponsor in site.data.sponsors_infra %}
    <div class="sponsor">
      <a href="{{ sponsor.url }}" target="_blank">
        <img width="{{ sponsor.image_width }}" src="{{ sponsor.image_url }}" alt="{{ sponsor.name }}"/>
      </a>
    </div>
  {% endfor %}
  </div> -->

Vous souhaitez nous appuyer? Jetez un coup d'oeil à notre <a href="/UnitedCTF-Plan-Partenariat.pdf" target="_blank">plan de partenariat</a>
