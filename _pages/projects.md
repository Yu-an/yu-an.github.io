---
layout: page
title: projects
permalink: /projects/
---
My research concerns structures that indicate, not only *what* a speaker is saying, but also *why* they are saying it, and how it is supposed to relate to the conversation. I approach these structures in two ways: as a semanticist, I look for the simplest analysis of these structures; as an acquisitionist, I ask how children acquire these meanings. Here are some of my projects:

{% for project in site.projects %}
<div>
        {% if project.img %}
        <img class="project-col" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}
</div>    
<h3 class = "project-title" >
    {{ project.title }}
</h3>
<h5 class = "project-description" >{{ project.description }}</h5>

<div>
<div class="project-text">
{{project.content}}

</div>
</div>

{% endfor %}
