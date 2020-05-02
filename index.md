---
layout: default
title: "Übersicht"
permalink: /
---

# OCC Blog

_Hier schreiben [Felix Lohmeier](https://www.felixlohmeier.de) und [Sebastian Meyer](https://informathekar.de) über die Themen Openness und Digitalisierung in Kultur und Wissenschaft. Es handelt sich um Werkstattberichte ihrer gemeinsamen Arbeit für [Open Culture Consulting]({{ site.homepage }})._

Die Artikel bieten einen Einblick hinter die Kulissen der Beratungstätigkeit für Bibliotheken, Archive, Museen und Universitäten. Manchmal sind es jedoch auch einfach kleine Tipps oder Arbeitsnotizen, die nebenbei entstanden und vielleicht auch für Außenstehende interessant sind.

{% for post in site.posts %}

* * *

<small>
  {{ post.date | date: "%-d" }}.
  {% assign m = post.date | date: "%-m" | minus: 1 %}{{ site.data.dateformat.months[m] }}
  {{ post.date | date: "%Y" }}
  &mdash; {{ post.author }}
</small>

## [{{ post.title }}]({{ post.url }})

<blockquote>
  {{ post.excerpt }}
</blockquote>

[Artikel lesen...]({{ post.url }})

{% endfor %}
