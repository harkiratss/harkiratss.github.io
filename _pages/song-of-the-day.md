---
layout: page
title: Song of the Day
permalink: /song-of-the-day/
---

{% assign dayIndex = site.time | date: "%j" | plus: 0 %}
{% assign idx = dayIndex | modulo: site.data.youtube_songs.songs.size %}
{% assign song = site.data.youtube_songs.songs[idx] %}

## 🎵 Song of the Day

**{{ song.name }}**

<iframe width="100%" height="400"
 src="https://www.youtube.com/embed/{{ song.url | split: '=' | last }}"
 frameborder="0" allowfullscreen>
</iframe>

[Open on YouTube]({{ song.url }})
