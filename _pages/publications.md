---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
            .container {
                        max-width: 800px;
                        margin: 0 auto;
                        padding: 20px;
            }
            .publication {
                background-color: #fff;
                border: 1px solid #ddd;
                padding: 20px;
                margin-bottom: 20px;
                border-radius: 5px;
            }
            
            .publication h2 {
                margin: 0;
                cursor: pointer; /* Make the title a pointer to indicate it's clickable */
                color: #007BFF; /* Change the color to indicate it's a link */
            }
            .publication p {
                font-style: italic;
            }
</style>

{% include base_path %}

{% for post in site.publications reversed %}
  <div class="container">
        <div class="publication">
            <h2>{{ post.title }}</h2>
            <p>Author(s): {{post.Authors}}</p>
            <p>Published in: {{post.venue}}</p>
            <p>Date: {{post.year}}</p>
            <div class="abstract" id="abstract1">
                <p>Abstract: {{post.abstract}} </p>
            </div>
        </div>
  </div>
{% endfor %}
