---
layout: default
title: qianze zhang | portfolio
permalink: /portfolio/
---
 <center>
 <div class="home">
 {% for post in site.posts %}
    {% if post.categories contains 'blog1' %}
     {% cycle 'add row' : '<div class="row">', nil, nil %}
         <div class="col-sm-4">
             <div class="preview-panel">
                 <a href="{{ post.url | prepend: site.baseurl }}">
                     <img src="{{ post.preview | prepend: site.baseurl }}">
                 </a>
            </div>
         </div>
 {% cycle 'end row' : nil, nil, '</div>' %}
   {% endif %}
 {% endfor %} 
 </div>hellooo got to bottom
 </center>
