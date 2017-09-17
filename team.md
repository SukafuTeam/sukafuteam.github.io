---
title: Team
layout: page
---

[#]:<h1> Conheça o time </h1>

<p style="text-align:center; margin-bottom: 0">
	<img class="title-image" src="{{site.url}}/assets/images/team.png">
</p>

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
