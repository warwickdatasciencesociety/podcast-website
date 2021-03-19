---
layout: default
title: Episodes
---
<div class = "episodes">

<h2> Episodes </h2>
<ul>
{% for post in site.posts %}    
    {% if post.type == "main" %}
        <li>
            <a href="{{ post.url }}"> {{ post.title }} </a>
        </li>
    {% endif %}

{% endfor %}
</ul>

<h2> Bonus Episodes </h2>
<ul>
{% for post in site.posts %}    
    {% if post.type == "bonus" %}
        <li>
            <a href="{{ post.url }}"> {{ post.title }} </a>
        </li>
    {% endif %}

{% endfor %}
</ul>
</div> 
