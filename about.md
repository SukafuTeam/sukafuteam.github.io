---
title: About
layout: page
---
<!-- SOBRE -->
![Profile Image]({{ site.url }}/assets/images/people.png)

<p>A Sukafu Team é uma equipe de desenvolvimento de jogos eletrônicos para computadores e dispositivos móveis, composta apenas por estudantes e amantes do desenvolvimento de entretenimento digital.</p>
<p>Criada em 2014, para um evento de criação de jogos, a Global Game Jam, a Sukafu Team vem evoluindo e melhorando conforme seus integrantes também evoluem em habilidades artísticas, de programação, game design e música.</p>

<!-- PREMIACOES -->
<!-- <h2> Premiações e indicaçoes <p class="fa fa-trophy" style="color: #ffd700"></p> </h2> -->
<h2 class="samurai-font"> PREMIOS E INDICACOES <p class="fa fa-trophy" style="color: #ffd700"></p></h2>

<ul class="skill-list">
	<li>Eleito melhor jogo da Global Game Jam da PUCPR, edição 2015. ( jogo <a target="_blank" href="https://sukafu-team.itch.io/ninja-sukafu-ii">Ninja Sukafu II</a> )</li>
	<li>Finalista na SBGames de 2015. (jogo <a target="_blank" href="https://sukafu-team.itch.io/ninja-sukafu-ii"> Ninja Sukafu II</a>)</li>
	<li>Eleito melhor jogo na Seed's Jam de 2015. ( jogo <a target="_blank" href="https://sukafu-team.itch.io/prev-enchente">PrevEnchente</a> )</li>
	<li>Eleito melhor jogo na Global Game Jam da PUCPR, edição 2016. ( jogo <a target="_blank" href="https://sukafu-team.itch.io/sukafu-neon">Sukafu Neon</a> )</li>
	<li>Eleito melhor jogo da Winter Game Jam de 2016. ( jogo <a target="_blank" href="https://sukafu-team.itch.io/bounded">Bounded</a> )</li>
	<li>Eleito melhor jogo (pelo público e pelo júri) da Seed's Jam de 2016. ( jogo <a target="_blank" href="https://sukafu-team.itch.io/jornada-paralimpica">Jornada Paralímpica</a> )</li>
	<li>Finalista na mostra de artes da SBGames 2017. ( jogo <a target="_blank" href="https://sukafu-team.itch.io/sukafu-duel"> Sukafu Duel</a> )</li>
	<li>Vencedor do desafio "Pira no Cartola" que aconteceu na Brasil Game Jam 2017. ( jogo <a target="_blank" href="https://sukafu-team.itch.io/cartolaria">Cartolaria</a> )</li>
	<li>Eleito melhor jogo da SBGames Light Jam 2017 em conjunto com núcleo Seed's. ( jogo <a target="_blank" href="https://sukafu-team.itch.io/vida">Vida</a> )</li>
	<li>Eleito melhor jogo por votação da sede de Curitiba da Café Game Jam 2018. ( jogo <a target="_blank" href="https://sukafu-team.itch.io/kingdom-blast">Kingdom Blast</a> )</li>
</ul>


<!-- TEAM -->
<h2 class="samurai-font"> TIME </h2>

<hr style="margin-top:0">

<section class="entry-list">
    {% for person in site.data.team %}
        <article class="team-entry">
            {% if person.image_path %}
                <a class="team-image">
                    <img src="{{ site.url }}/assets/images/team/{{ person.image_path }}">
                </a>
            {% endif %}
            {% if person.name %}
                <h3 class="game-title" style="text-align:center;">
                    <a style="text-decoration: none">
                        {{ person.name }}
                    </a>
                </h3>
            {% endif %}

						{% if person.function %}<p class="game-description" style="text-align:center; margin:0">{{ person.function }}</p>{% endif %}

						<p style="text-align:center; margin:0">
							{% if person.facebook %}<a href="{{person.facebook}}" target="_blank">Facebook</a>{%endif%}

							{% if person.github %}| <a href="{{person.github}}" target="_blank">Github</a>{%endif%}

							{% if person.twitter %}| <a href="{{person.twitter}}" target="_blank">Twitter</a>{%endif%}

							{% if person.artstation %}<a href="{{person.artstation}}" target="_blank">Artstation</a>{%endif%}

							{% if person.behance %}| <a href="{{person.behance}}" target="_blank">Behance</a>{%endif%}

							{% if person.soundcloud %}| <a href="{{person.soundcloud}}" target="_blank">SoundCloud</a>{%endif%}
						</p>

        </article>
    {% endfor %}
</section>
