---
layout: page
title: Home
id: home
permalink: /
---

# Waidmannsheil! 👋

> Das ist des Jägers Ehrenschild,
> Daß er beschützt und hegt sein Wild,
> Waidmännisch jagt, wie sich’s gehört,
> Den Schöpfer im Geschöpfe ehrt!

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
    Das ist des Jägers Ehrenschild,
    Daß er beschützt und hegt sein Wild,
    Waidmännisch jagt, wie sich’s gehört,
    Den Schöpfer im Geschöpfe ehrt!
</p>

<strong>Vor kurzem aktualisiert</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
