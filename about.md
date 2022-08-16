---
title: About
layout: page
---
<hr>
<p>We are a group of developers from Curitiba, Brazil. We first met in 2014 at Global Game Jam and we're together, making nice and short games ever since.</p>
<p>We've been evolving our skills in programming, art, design and music and bringing it to the team as we build our own way of developing games. Stay around, we got a lot to show you!</p>

<!-- PREMIACOES -->
<!-- <h2> Premiações e indicaçoes <p class="fa fa-trophy" style="color: #ffd700"></p> </h2> -->
<h2 class="samurai-font"> AWARDS AND RECOGNITION <p class="fa fa-trophy" style="color: #ffb500"></p></h2>

<ul class="skill-list">
	<li>Best game at Global Game Jam 2015 in the Curitiba Jam site ( <a target="_blank" href="https://sukafu-team.itch.io/ninja-sukafu-ii">Ninja Sukafu II</a> )</li>
	<li>SBGames 2015 finalist ( <a target="_blank" href="https://sukafu-team.itch.io/ninja-sukafu-ii"> Ninja Sukafu II</a>)</li>
	<li>Best game at Seeds Game Jam 2015 ( <a target="_blank" href="https://sukafu-team.itch.io/prev-enchente">PrevEnchente</a> )</li>
	<li>Best game at Global Game Jam 2016 in the Curitiba Jam site ( <a target="_blank" href="https://sukafu-team.itch.io/sukafu-neon">Sukafu Neon</a> )</li>
	<li>Best game at Winter Game Jam 2016 ( <a target="_blank" href="https://sukafu-team.itch.io/bounded">Bounded</a> )</li>
	<li>Best game at Seeds Game Jam 2016 ( <a target="_blank" href="https://sukafu-team.itch.io/jornada-paralimpica">Jornada Paralímpica</a> )</li>
	<li>SBGames 2017 Art Showcase ( <a target="_blank" href="https://sukafu-team.itch.io/sukafu-duel"> Sukafu Duel</a> )</li>
	<li>Best game at Brasil Game Jam 2017 ( <a target="_blank" href="https://sukafu-team.itch.io/cartolaria">Cartolaria</a> )</li>
	<li>Best game at SBGames Light Jam 2017 ( <a target="_blank" href="https://sukafu-team.itch.io/vida">Vida</a> )</li>
	<li>Best game at Café Game Jam 2018 in the Curitiba Jam site ( <a target="_blank" href="https://sukafu-team.itch.io/kingdom-blast">Kingdom Blast</a> )</li>
	<li>Golden Cube Award 2018 finalist ( <a target="_blank" href="https://sukafu-team.itch.io/vida">Vida</a> )</li>
	<li>SBGames 2018 Art Showcase (
		<a target="_blank" href="https://sukafu-team.itch.io/vida"> Vida</a> |
		<a target="_blank" href="https://sukafuteam.com/doggonaut"> Doggonaut</a> |
		<a target="_blank" href="https://sukafu-team.itch.io/plasma-invaders"> Plasma Invaders</a> |
		<a target="_blank" href="https://sukafuteam.com/kraken_escape"> Kraken Escape</a>
	)</li>
	<li>ICGJ 2019 finalist ( <a target="_blank" href="https://sukafu-team.itch.io/akina">Akina</a> )</li>
	<li>Facebook Gaming Jam 2019 winner in the category "Business" ( <a target="_blank" href="https://sukafu-team.itch.io/beezness">Beezness</a> )</li>
</ul>

<!-- TEAM -->
<h2 class="samurai-font"> TEAM </h2>
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
							{% if person.facebook %} <a href="{{person.facebook}}" target="_blank">Facebook</a>{%endif%}

							{% if person.linkedin %} <a href="{{person.linkedin}}" target="_blank">Linkedin</a>{%endif%}

							{% if person.instagram %} <a href="{{person.instagram}}" target="_blank">Instagram</a>{%endif%}

							{% if person.website %} <a href="{{person.website}}" target="_blank">Portfolio</a>{%endif%}

							{% if person.github %}| <a href="{{person.github}}" target="_blank">Github</a>{%endif%}

							{% if person.twitter %}| <a href="{{person.twitter}}" target="_blank">Twitter</a>{%endif%}

							{% if person.artstation %} <a href="{{person.artstation}}" target="_blank">Artstation</a>{%endif%}

							{% if person.behance %}| <a href="{{person.behance}}" target="_blank">Behance</a>{%endif%}

							{% if person.soundcloud %}| <a href="{{person.soundcloud}}" target="_blank">SoundCloud</a>{%endif%}
						</p>

        </article>
    {% endfor %}
</section>
