---
layout: page
title: Náš team 
description: Náš team
sitemap:
    priority: 0.7
    lastmod: 2018-08-21
    changefreq: weekly
---
Reprezentujeme všechny věkové skupiny, všechny části obce. 
Děláme různou práci, patříme k různým národnostem. Jsou mezi námi
starousedlíci i přistěhovalci. Reprezentujeme všechny občanské spolky -
TJ Sokol, dobrovolní hasiči a myslivci. Navzájem se dopňujeme a jsme 
jeden team. 

Nás spojuje společný zájem o to, aby naše obec vzkvétala a nestárla,
aby se mezi občany udržovali dobré vztahy a vzájemná výpomoc, 
aby se lide mezi sebou více setkávali a komunkovali. 
<!--aby i v naší vesnici pravda a láska zvítězili nad lží a nenávistí.-->

Víme jak toho dosáhnout, máme kompletní <a href="/program">program</a> 
a věříme ve vaši podporu.


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
<p><em>{{ person.mission }}</em></p>
{% endif %}
<hr style="clear:left;">
</div>
{% endfor %}
