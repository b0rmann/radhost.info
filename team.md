---
layout: page
title: Náš team 
description: When building a website it's helpful to see what the focus of your site is. This page is an example of how to show a website's focus.
sitemap:
    priority: 0.7
    lastmod: 2018-08-21
    changefreq: weekly
---
Reprezentujeme všechné věkové skupiny, všechný obecní časti. 
Delámé různou praci, patřime k různým národnostěm. Jsou mezi nama
starousedlici i přistěhovalci. Reprezentujeme všechný občanske spolky -
TJ Sokol, dobrovolní hasiče a myslivce. Navzajem se dopnujeme a jsme 
jeden team. 

Nas spojuje společný zájem o to, aby náše obec vkvětala a nestarla, 
aby se mezi občany se udržovali dobre vztahy a vzájemná výpomoc, 
aby lidě mezi sebou vice setkavali a komunkovali, aby i v naši vesnici
pravda a láska zvítězili nad lží a nenávistí.

Vime jak toho dosahnout, mame kompletní <a href="/program">program</a> a věřime ve vaší podporu.


{% for person in site.data.people %}
### {{person.position}}. {{ person.name }}, {{ person.work }}
<div class="box">
<img class="image left" style="height: 200px;" src="/images/persons/{{  person.id }}.jpg" alt="{{ person.name }}" />
{{person.biografy}}
<hr style="clear:left;">
</div>
{% endfor %}
