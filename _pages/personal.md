---
layout: archive
title:
permalink: /personal/

# ===== EDIT THESE MANUALLY =====
movie_of_the_week: "One Battle After Another -- Paul Thomas Anderson"
movie_link: "https://www.imdb.com/title/tt30144839/"

book_of_the_month: "Ubik -- Philip K Dick"
book_link: "https://www.goodreads.com/book/show/22590.Ubik"
# ===============================
---
<blockquote style="font-style: italic; opacity: 0.85; text-align: center;">
... the wise man looks into space<br>
and does not regard the small as too little,<br>
nor the great as too big,<br>
for he knows that there is no limit to dimensions.<br>
— <strong>Zhuang Zhou</strong>
</blockquote>


{% assign songs = site.data.songs.songs %}
{% assign n = songs | size %}

{% if n == 0 %}
⚠️ **No songs loaded!**  
Check that `_data/songs.yml` exists and is valid YAML.

{% else %}

{% assign day_of_year = site.time | date: "%j" | plus: 0 %}
{% assign idx = day_of_year | modulo: n %}
{% assign song = songs[idx] %}

## 🎧 Song of the Day

**{{ song.name }}**

<iframe width="560" height="315"
src="{{ song.url | replace: 'watch?v=', 'embed/' }}"
frameborder="0" allowfullscreen>
</iframe>

{% endif %}

---

## 🎬 Movie of the Week  
👉 **<a href="{{ page.movie_link }}" target="_blank">{{ page.movie_of_the_week }}</a>**

---

## 📚 Book of the Month  
👉 **<a href="{{ page.book_link }}" target="_blank">{{ page.book_of_the_month }}</a>**

---

## 🗂️ Archive (click to expand)

<details>
<summary><strong>Past picks</strong></summary>

<div style="font-size: 0.85em; opacity: 0.9; margin-top: 10px;">

<h3>🎬 Movies</h3>
<ul>
  <li>
    <em>Dune (2021)</em> — 
    <a href="https://www.imdb.com/title/tt1160419/" target="_blank">IMDb</a>
  </li>
  <li>
    <em>2001: A Space Odyssey</em> — 
    <a href="https://www.imdb.com/title/tt0062622/" target="_blank">IMDb</a>
  </li>
</ul>

<h3>📚 Books</h3>
<ul>
  <li>
    <em>1984</em> — George Orwell — 
    <a href="https://www.goodreads.com/book/show/40961427-1984" target="_blank">Goodreads</a>
  </li>
  <li>
    <em>Animal Farm</em> — George Orwell — 
    <a href="https://www.goodreads.com/book/show/7613.Animal_Farm" target="_blank">Goodreads</a>
  </li>
  <li>
    <em>Before the Coffee Gets Cold</em> — Toshikazu Kawaguchi — 
    <a href="https://www.goodreads.com/book/show/44421460-before-the-coffee-gets-cold" target="_blank">Goodreads</a>
  </li>
</ul>

</div>
</details>

<blockquote style="font-style: italic; opacity: 0.85; text-align: center;">
Between my finger and my thumb<br>
The squat pen rests; snug as a gun.<br>

Under my window, a clean rasping sound<br>
When the spade sinks into gravelly ground:<br>
My father, digging. I look down<br>

Till his straining rump among the flowerbeds<br>   
Bends low, comes up twenty years away<br>
Stooping in rhythm through potato drills<br>
Where he was digging.<br>

The coarse boot nestled on the lug, the shaft<br>
Against the inside knee was levered firmly.<br>
He rooted out tall tops, buried the bright edge deep<br>
To scatter new potatoes that we picked,<br>
Loving their cool hardness in our hands.<br>

By God, the old man could handle a spade.<br>   
Just like his old man.<br>

My grandfather cut more turf in a day<br>
Than any other man on Toner’s bog.<br>
Once I carried him milk in a bottle<br>
Corked sloppily with paper. He straightened up<br>
To drink it, then fell to right away<br>
Nicking and slicing neatly, heaving sods<br>
Over his shoulder, going down and down<br>
For the good turf. Digging.<br>

The cold smell of potato mould, the squelch and slap<br>
Of soggy peat, the curt cuts of an edge<br>
Through living roots awaken in my head.<br>
But I’ve no spade to follow men like them.<br>

Between my finger and my thumb<br>
The squat pen rests.<br>
I’ll dig with it.<br>

-- <strong>Seamus Heaney, "Digging" from Death of a Naturalist.<strong>
</blockquote>
