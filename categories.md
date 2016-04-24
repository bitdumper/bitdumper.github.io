---
layout: page
title: Categories
permalink: categories
---

# Categories
<ul>
{% for c in site.categories %}
    <li>{{c|first}}<ul>
        {% for posts in c%}
            {% for post in posts %}
                <li><a href="{{post.url}}">{{post.title}}</a></li>
            {% endfor %}
        {% endfor %}
        </ul></li>
{% endfor %}
</ul>