---
title: Instruções online hospedadas
permalink: index.html
layout: home
---

# Exercícios do Analista de Dados

Esses exercícios oferecem suporte ao curso Microsoft [DP-500: Como criar e implementar soluções de análise de escala corporativa usando o Microsoft Azure e o Microsoft Power BI](https://docs.microsoft.com/training/courses/dp-500t00)

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/labs'" %}
| Módulo ILT | Laboratório |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} — {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

<!--

## Demos

{% assign demos = site.pages | where_exp:"page", "page.url contains '/Instructions/Demos'" %}
| Module | Demo |
| --- | --- | 
{% for activity in demos  %}| {{ activity.demo.module }} | [{{ activity.demo.title }}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
 
-->
