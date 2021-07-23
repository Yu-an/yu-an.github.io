---
layout: page
title: projects
permalink: /projects/
---
Broadly, I am interested in the interaction of meaning, structure and context across different languages, in connection with language acquisition: 

-- Cross-linguistically, how does meaning interact with syntactic structure and pragmatic context? 

-- Does the interaction simplify or complicate the task of acquiring meaning? 

-- Are solutions to the acquisition of semantics that draw on pragmatics and syntax general enough to deal with the cross-linguistic differences? 


{% for project in site.projects %}

<div style="float:right;max-width: 40%;padding-top:7px;">
        {% if project.img %}
        <img style="width:100%" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
</div>
<h3 class = "project" >
    {{ project.title }}
</h3>

<div>
<div style="width:100%;text-align: justify;">
{{project.content}}
</div>
</div>

{% endfor %}
