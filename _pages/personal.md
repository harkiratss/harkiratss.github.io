---
layout: archive
title:
permalink: /personal/

# ===== EDIT THESE MANUALLY =====
movie_of_the_week: "Project Hail Mary"
movie_link: "https://www.imdb.com/title/tt12042730/"

book_of_the_month: "The Plague"
book_link: "https://www.goodreads.com/book/show/11989.The_Plague"
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
    <em>One Battle After Another -- Paul Thomas Anderson (2026)</em>
    <a href="https://www.imdb.com/title/tt30144839/" target="_blank">IMDb</a>
  </li>
  <li>
    <em>Dune -- Denis Villeneuve (2021)</em> — 
    <a href="https://www.imdb.com/title/tt1160419/" target="_blank">IMDb</a>
  </li>
  <li>
    <em>2001: A Space Odyssey -- Stanley Kubrick</em> — 
    <a href="https://www.imdb.com/title/tt0062622/" target="_blank">IMDb</a>
  </li>

  <li><em>Incendies -- Denis Villeneuve</em> — <a href="https://www.imdb.com/title/tt1255953/" target="_blank">IMDb</a></li>
  <li><em>Sicario -- Denis Villeneuve</em> — <a href="https://www.imdb.com/title/tt3397884/" target="_blank">IMDb</a></li>
  <li><em>Prisoners -- Denis Villeneuve</em> — <a href="https://www.imdb.com/title/tt1392214/" target="_blank">IMDb</a></li>
  <li><em>Arrival -- Denis Villeneuve</em> — <a href="https://www.imdb.com/title/tt2543164/" target="_blank">IMDb</a></li>
  <li><em>Wind River -- Taylor Sheridan</em> — <a href="https://www.imdb.com/title/tt5362988/" target="_blank">IMDb</a></li>

  <li><em>The Shawshank Redemption -- Frank Darabont</em> — <a href="https://www.imdb.com/title/tt0111161/" target="_blank">IMDb</a></li>
  <li><em>Pulp Fiction -- Quentin Tarantino</em> — <a href="https://www.imdb.com/title/tt0110912/" target="_blank">IMDb</a></li>
  <li><em>Fight Club -- David Fincher</em> — <a href="https://www.imdb.com/title/tt0137523/" target="_blank">IMDb</a></li>
  <li><em>Se7en -- David Fincher</em> — <a href="https://www.imdb.com/title/tt0114369/" target="_blank">IMDb</a></li>
  <li><em>The Silence of the Lambs -- Jonathan Demme</em> — <a href="https://www.imdb.com/title/tt0102926/" target="_blank">IMDb</a></li>

  <li><em>Spirited Away -- Hayao Miyazaki</em> — <a href="https://www.imdb.com/title/tt0245429/" target="_blank">IMDb</a></li>
  <li><em>Parasite -- Bong Joon-ho</em> — <a href="https://www.imdb.com/title/tt6751668/" target="_blank">IMDb</a></li>
  <li><em>Everything Everywhere All at Once -- Daniel Kwan & Daniel Scheinert</em> — <a href="https://www.imdb.com/title/tt6710474/" target="_blank">IMDb</a></li>
  <li><em>Grave of the Fireflies -- Isao Takahata</em> — <a href="https://www.imdb.com/title/tt0095327/" target="_blank">IMDb</a></li>

  <li><em>The Departed -- Martin Scorsese</em> — <a href="https://www.imdb.com/title/tt0407887/" target="_blank">IMDb</a></li>
  <li><em>American History X -- Tony Kaye</em> — <a href="https://www.imdb.com/title/tt0120586/" target="_blank">IMDb</a></li>
  <li><em>Zodiac -- David Fincher</em> — <a href="https://www.imdb.com/title/tt0443706/" target="_blank">IMDb</a></li>
  <li><em>Nightcrawler -- Dan Gilroy</em> — <a href="https://www.imdb.com/title/tt2872718/" target="_blank">IMDb</a></li>
  <li><em>Mystic River -- Clint Eastwood</em> — <a href="https://www.imdb.com/title/tt0327056/" target="_blank">IMDb</a></li>

  <li><em>Spider-Man: Across the Spider-Verse -- Joaquim Dos Santos, Kemp Powers, Justin K. Thompson</em> — <a href="https://www.imdb.com/title/tt9362722/" target="_blank">IMDb</a></li>
  <li><em>The Usual Suspects -- Bryan Singer</em> — <a href="https://www.imdb.com/title/tt0114814/" target="_blank">IMDb</a></li>
  <li><em>WALL·E -- Andrew Stanton</em> — <a href="https://www.imdb.com/title/tt0910970/" target="_blank">IMDb</a></li>

  <li><em>Raiders of the Lost Ark -- Steven Spielberg</em> — <a href="https://www.imdb.com/title/tt0082971/" target="_blank">IMDb</a></li>
  <li><em>The Shining -- Stanley Kubrick</em> — <a href="https://www.imdb.com/title/tt0081505/" target="_blank">IMDb</a></li>
  <li><em>The Dark Knight -- Christopher Nolan</em> — <a href="https://www.imdb.com/title/tt0468569/" target="_blank">IMDb</a></li>
  <li><em>Oldboy -- Park Chan-wook</em> — <a href="https://www.imdb.com/title/tt0364569/" target="_blank">IMDb</a></li>
  <li><em>Princess Mononoke -- Hayao Miyazaki</em> — <a href="https://www.imdb.com/title/tt0119698/" target="_blank">IMDb</a></li>

  <li><em>Dr. Strangelove -- Stanley Kubrick</em> — <a href="https://www.imdb.com/title/tt0057012/" target="_blank">IMDb</a></li>
  <li><em>Star Wars: Episode IV - A New Hope -- George Lucas</em> — <a href="https://www.imdb.com/title/tt0076759/" target="_blank">IMDb</a></li>
  <li><em>Star Wars: Episode V - The Empire Strikes Back -- Irvin Kershner</em> — <a href="https://www.imdb.com/title/tt0080684/" target="_blank">IMDb</a></li>
  <li><em>Star Wars: Episode VI - Return of the Jedi -- Richard Marquand</em> — <a href="https://www.imdb.com/title/tt0086190/" target="_blank">IMDb</a></li>

  <li><em>Eternal Sunshine of the Spotless Mind -- Michel Gondry</em> — <a href="https://www.imdb.com/title/tt0338013/" target="_blank">IMDb</a></li>
  <li><em>The Truman Show -- Peter Weir</em> — <a href="https://www.imdb.com/title/tt0120382/" target="_blank">IMDb</a></li>
  <li><em>Oppenheimer -- Christopher Nolan</em> — <a href="https://www.imdb.com/title/tt15398776/" target="_blank">IMDb</a></li>
  <li><em>Taxi Driver -- Martin Scorsese</em> — <a href="https://www.imdb.com/title/tt0075314/" target="_blank">IMDb</a></li>
  <li><em>There Will Be Blood -- Paul Thomas Anderson</em> — <a href="https://www.imdb.com/title/tt0469494/" target="_blank">IMDb</a></li>

  <li><em>The Thing -- John Carpenter</em> — <a href="https://www.imdb.com/title/tt0084787/" target="_blank">IMDb</a></li>
  <li><em>Kill Bill: Vol. 1 -- Quentin Tarantino</em> — <a href="https://www.imdb.com/title/tt0266697/" target="_blank">IMDb</a></li>
  <li><em>Monty Python and the Holy Grail -- Terry Gilliam & Terry Jones</em> — <a href="https://www.imdb.com/title/tt0071853/" target="_blank">IMDb</a></li>
  <li><em>Harry Potter and the Prisoner of Azkaban -- Alfonso Cuarón</em> — <a href="https://www.imdb.com/title/tt0304141/" target="_blank">IMDb</a></li>

  <li><em>Memories of Murder -- Bong Joon-ho</em> — <a href="https://www.imdb.com/title/tt0353969/" target="_blank">IMDb</a></li>
  <li><em>Blade Runner -- Ridley Scott</em> — <a href="https://www.imdb.com/title/tt0083658/" target="_blank">IMDb</a></li>
  <li><em>The Wages of Fear -- Henri-Georges Clouzot</em> — <a href="https://www.imdb.com/title/tt0046268/" target="_blank">IMDb</a></li>
  <li><em>Spotlight -- Tom McCarthy</em> — <a href="https://www.imdb.com/title/tt1895587/" target="_blank">IMDb</a></li>
  <li><em>The Terminator -- James Cameron</em> — <a href="https://www.imdb.com/title/tt0088247/" target="_blank">IMDb</a></li>

  <li><em>The Big Lebowski -- Joel Coen</em> — <a href="https://www.imdb.com/title/tt0118715/" target="_blank">IMDb</a></li>
  <li><em>Before Sunset -- Richard Linklater</em> — <a href="https://www.imdb.com/title/tt0381681/" target="_blank">IMDb</a></li>
  <li><em>The Wailing -- Na Hong-jin</em> — <a href="https://www.imdb.com/title/tt5215952/" target="_blank">IMDb</a></li>
  <li><em>Hereditary -- Ari Aster</em> — <a href="https://www.imdb.com/title/tt7784604/" target="_blank">IMDb</a></li>

  <li><em>Laapataa Ladies -- Kiran Rao</em> — <a href="https://www.imdb.com/title/tt21626284/" target="_blank">IMDb</a></li>
  <li><em>3 Idiots -- Rajkumar Hirani</em> — <a href="https://www.imdb.com/title/tt1187043/" target="_blank">IMDb</a></li>
  <li><em>Taare Zameen Par -- Aamir Khan</em> — <a href="https://www.imdb.com/title/tt0986264/" target="_blank">IMDb</a></li>
  <li><em>Drishyam -- Nishikant Kamat</em> — <a href="https://www.imdb.com/title/tt4430212/" target="_blank">IMDb</a></li>

  <li><em>Gangs of Wasseypur -- Anurag Kashyap</em> — <a href="https://www.imdb.com/title/tt1954470/" target="_blank">IMDb</a></li>
  <li><em>Gol Maal -- Hrishikesh Mukherjee</em> — <a href="https://www.imdb.com/title/tt0079221/" target="_blank">IMDb</a></li>
  <li><em>Tumbbad -- Rahi Anil Barve</em> — <a href="https://www.imdb.com/title/tt8239946/" target="_blank">IMDb</a></li>
  <li><em>Jaane Bhi Do Yaaro -- Kundan Shah</em> — <a href="https://www.imdb.com/title/tt0085743/" target="_blank">IMDb</a></li>
  <li><em>Khosla Ka Ghosla -- Dibakar Banerjee</em> — <a href="https://www.imdb.com/title/tt0466460/" target="_blank">IMDb</a></li>

  <li><em>Hera Pheri -- Priyadarshan</em> — <a href="https://www.imdb.com/title/tt0242519/" target="_blank">IMDb</a></li>
  <li><em>Swades -- Ashutosh Gowariker</em> — <a href="https://www.imdb.com/title/tt0367110/" target="_blank">IMDb</a></li>
  <li><em>Chak De! India -- Shimit Amin</em> — <a href="https://www.imdb.com/title/tt0871510/" target="_blank">IMDb</a></li>

</ul>

<h3>📚 Books</h3>
<ul>
  <li>
    <em>Ubik</em> — Philip K Dick — 
    <a href="https://www.goodreads.com/book/show/22590.Ubik" target="_blank">Goodreads</a>
  </li>
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
