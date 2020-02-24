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

<h3 class = "project" >
    {{ project.title }}
</h3>

<p> 
   {{ project.description }}  
 </p>  

<p>
  <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
    </a>
</p>

        


{% endfor %}
