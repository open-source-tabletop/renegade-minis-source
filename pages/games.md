---
title: Games
permalink: /games/
layout: games
subtitle: 3D Printable Games available to download now
---

{% assign games = site.games | sort: 'date' | reverse %}
{% for game in games %}
{% unless game.draft %}
<article>
    <header>
        <span class="date">{{ game.date | date: "%B %Y" }}</span>
        <h2><a href="{{ game.url }}">{{ game.title }}</a></h2>
    </header>
    {% if game.header %}
    <a href="{{ game.url }}" class="image fit"><img src="\{{ game.header }}" alt=""></a>
    {% endif %}
    {{ game.intro | markdownify }}
    <ul class="actions special">
        <li><a href="{{ game.url }}" class="button">See More</a></li>
    </ul>
</article>
{% endunless %}
{% endfor %}
