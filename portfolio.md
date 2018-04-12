---
layout: default
title: qianze zhang | portfolio
permalink: /portfolio/
---
 <center>
 <div class="home">
 {% for post in site.posts %}
    {% if post.categories contains 'blog1' %}
     {% cycle 'add row' : '<div class="row" style="width:30%">', nil, nil %}
             <div class="preview-panel">
                 <a href="{{ post.url | prepend: site.baseurl }}">
                     <img src="{{ post.preview | prepend: site.baseurl }}">
                 </a>
            </div>
 {% cycle 'end row' : nil, nil, '</div>' %}
   {% endif %}
 {% endfor %} 
 </div>hellooo got to bottom pls be centered and small
 </center>
