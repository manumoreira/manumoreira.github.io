---
layout: default
title: Inicio
---

<section class="intro">
  <p class="lead">Antropólogo de formación, trabajo hace más de 20 años en desarrollo de software. Pasé por distnitas áreas, hoy me dedico a gestionar proyectos y equipos.</p>
  <p>También soy docente universitario de metodología de la investigación y estadística en ciencias sociales, y estoy terminando la especialización en data mining en FCEN UBA.</p>
  <p> Acá comparto artículos, herramientas y algo de investigación.</p>
</section>

<section>
  <h2>Artículos</h2>
  <ul class="list">
  {% for post in site.posts %}
    <li class="with-date">
      <span class="date">{{ post.date | date: "%Y-%m-%d" }}</span>
      <div>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        {% if post.description %}<p>{{ post.description }}</p>{% endif %}
      </div>
    </li>
  {% endfor %}
  </ul>
</section>

<section>
  <h2>Charlas y entrevistas</h2>
  <ul class="list">
  {% assign appearances = site.data.appearances | sort: "date" | reverse %}
  {% for item in appearances %}
    <li class="with-date">
      <span class="date">{{ item.date | date: "%Y-%m-%d" }}</span>
      <div>
        <a href="{{ item.url }}">{{ item.title }}</a>
        <p>{{ item.outlet }}</p>
      </div>
    </li>
  {% endfor %}
  </ul>
</section>

<section>
  <h2>Herramientas y proyectos</h2>
  <ul class="list">
  {% for project in site.data.projects %}
    <li>
      <a href="{{ project.repo }}">{{ project.name }}</a>
      <p>{{ project.description }}</p>
    </li>
  {% endfor %}
  </ul>
</section>

<section>
  <h2>Investigación</h2>
  <ul class="list">
  {% for pub in site.data.publications %}
    <li{% if pub.featured %} class="featured"{% endif %}>
      <a href="{{ pub.url }}">{{ pub.title }}</a>
      <span class="meta">{{ pub.type }}, {{ pub.year }}</span>
    </li>
  {% endfor %}
  </ul>
</section>

<section>
  <h2>CV</h2>
  <p>Project manager en Manas e InSTEDD desde 2017, al frente de proyectos de software para salud pública y cooperación internacional. Magíster en Antropología Social (UBA) y docente universitario desde 2007.</p>
  <p><a href="{{ '/cv/' | relative_url }}">Ver CV completo →</a></p>
</section>