---
layout: page
title: Náš team 
description: When building a website it's helpful to see what the focus of your site is. This page is an example of how to show a website's focus.
sitemap:
    priority: 0.7
    lastmod: 2018-08-21
    changefreq: weekly
---
Reprezentujeme všechny věkové skupiny, všechny časti obce. 
Děláme různou práci, patříme k různým národnostem. Jsou mezi nami
starousedlíci i přistěhovalci. Reprezentujeme všechny občanské spolky -
TJ Sokol, dobrovolní hasiči a myslivci. Navzájem se dopnujeme a jsme 
jeden team. 

Nás spojuje společný zájem o to, aby naše obec vzkvétala a nestarla, 
aby se mezi občany udržovalí dobré vztahy a vzájemná výpomoc, 
aby lide se mezi sebou vice setkávali a komunkovali, aby i v naši vesnici
pravda a láska zvítězili nad lží a nenávistí.

Vime jak toho dosáhnout, máme kompletní <a href="/program">program</a> a věříme ve vaší podporu.


{% for person in site.data.people %}
<div class="box">
<header>
<img class="image left" src="/images/persons/{{  person.id }}.jpg" alt="{{ person.name }}" />
<h3>{{person.position}}. {{ person.name }}</h3>
<p>{{ person.work }}</p>
</header>
<p>
{{person.biografy}}
{% if person.facebook %}
<a href="https://www.facebook.com/{{person.facebook}}" class="icon fa-facebook"><span class="label">Facebook</span></a>
{% endif %}
</p>
{% if person.mission %}
<p>{{ person.mission }}</p>
{% endif %}
<hr style="clear:left;">
</div>
{% endfor %}
