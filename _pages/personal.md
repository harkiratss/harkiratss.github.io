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
Hey, little train, we're jumping on<br>
The train that goes to the Kingdom<br>
We're happy, ma, we're having fun<br>
The train ain't even left the station<br>
Hey, little train, wait for me<br>
I once was blind, but now I see<br>
And have you left a seat for me?<br>
Is that such a stretch of the imagination?<br>
Hey, little train, wait for me<br>
Was held in chains, but now I'm free<br>
I'm hanging in there, don't you see?<br>
In this process of elimination (ooh, children)<br>
Hey, little train, we're jumping on<br>
The train that goes to the Kingdom<br>
We are happy, ma, we are having fun (ooh, children)<br>
Beyond my wildest expectation (ooh, children)<br>
Hey, little train, we're jumping on<br>
The train that goes to the Kingdom<br>
We're happy, ma, we're having fun (ooh, children)<br>
The train ain't even left the station (ooh, children)<br>
Hey, little train, wait for me<br>
I once was blind but now I see, ooh-ooh-ooh<br>

-- <strong>Nicholas Edward Cave, O Children.<strong>
</blockquote>
