---
layout: creations
title: Créations
permalink: /creations/
update: "09/06/2020 21h00"
---

<p class="lead" style="margin-top:20px" >Ces quelques créations sont exclusivement extra-professionnelles.</p>

<div class="row">
  {% for creation in site.data.creations %}
  <div class="col-sm-6">
    <div class="card">
      <img 
      src="/img/creations/{{ creation.src-img }}" 
      class="card-img-top"
      alt="{{ creation.alt-img }}" />
      <div class="card-body" >
        <h5 class="card-title">{{ creation.title }}</h5>
        <h6 class="card-subtitle text-muted" >{{ creation.device }} / {{ creation.created-at }}</h6>
        <p class="card-text">{{ creation.description }}</p>
        {% if creation.type == 'Workshop' %}<a href="{{ creation.ws-link }}" class="card-link" >Workshop</a>{% elsif creation.type == 'Game' %}<a href="{{ creation.game-link }}" class="card-link" >Jeu</a><a href="{{ creation.repository }}" class="card-link" >Dépôt</a>{% else %}<a href="{{ creation.repository }}" class="card-link" >Dépôt</a>{% endif %}
      </div>
    </div>
  </div>
  {% endfor %}
</div>

<p class="lead" >
	Retrouvez toutes mes créations sur :<br />
	<a href="https://github.com/chris-scientist" class="btn btn-secondary" >GitHub</a> 
	<a href="https://gamebuino.com/fr/@chris-scientist/creations" class="btn btn-secondary" >Gamebuino</a>
</p>
