---
title: Positron Markdown vs R-Markdown
author: Michael Niemeyer
date: '2025-09-08'
slug: positron-markdown-vs-r-markdown
categories: []
tags: [ ["Positron","blogdown", "Hugo","Markdwon","R Markdown"]]
---

# Markdown

Markdown Post werden mit folgendem Befehl erstellt:
`blogdown::new_post("Mein 1. Markdown Post")`

Bei Markdown wird die Vorschau in Positron automatisch mit dem Speichern der .md Datei aktualisiert.


# R-Markdown

R-Markdown hat mehr Möglichkeiten als Markdown. Die Aktualisierung der Vorschau ist jedoch nicht so einfach wie bei Markdown.

R-Markdown Post werden mit folgendem Befehl erstellt:
`blogdown::new_post("Mein 1. R-Markdown Post", ext= ".rmd")`

Bei R-Markdown wird die Vorschau nicht automatisch mit dem Speichern der .rmd Datei aktualisiert.
Zur Aktualierung sind folgende Schritte notwendig:

- [ ] rmd Datei speichern
- [ ] alle Dateien außer .rmd löschen
- [ ] server stoppen (`blogdown::stop_server`)
- [ ] server neu starten (`blogdown::serve_site`)

Deshalb ist R-Markdown in Positron (2025.09.0) nur sinnvoll wenn auch wirklich R-Markdown Funktionen benötigt werden.

