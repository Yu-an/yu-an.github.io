---
layout: page
title: projects
permalink: /projects/
---
Broadly, I am interested in the interaction of semantics, syntax and pragmatics across different languages, in connection with language acquisition: 

-- Cross-linguistically, how does meaning interact with the syntactic structure and pragmatic contexts? 

-- Does the interaction simplify or complicate the task of acquiring meaning? 

-- Are solutions to the acquisition of semantics that draw on pragmatics and syntax general enough to deal with the cross-linguistic differences? 


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

<div>
<div class="project-text">
{{project.content}}
</div>
</div>

{% endfor %}
