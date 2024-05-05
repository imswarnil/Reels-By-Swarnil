---
layout: default
title: All Series
permalink : /series
---
<main>
    <div class="container">
        <h1>All Series</h1>

        {% for series in site.series %}
            <div class="series">
                <h2>{{ series.name }}</h2>
                <ul>
                    {% for episode in series.episodes %}
                        <li><a href="{{ episode.url }}">{{ episode.title }}</a></li>
                    {% endfor %}
                </ul>
            </div>
        {% endfor %}
    </div>
</main>
