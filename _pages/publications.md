---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
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


{% include base_path %}

{% for post in site.publications reversed %}
  <div class="container">
        <div class="publication">
            <div class="abstract" id="abstract1">
                <p>Abstract: This is the abstract for Publication 1.</p>
            </div>
            <p>Author(s): Author 1, Author 2</p>
            <p>Published in: Journal/Conference Name</p>
            <p>Date: January 1, 2023</p>
        </div>
        <div class="publication">
            <div class="abstract" id="abstract2">
                <p>Abstract: This is the abstract for Publication 2.</p>
            </div>
            <p>Author(s): Author 1, Author 3</p>
            <p>Published in: Another Journal/Conference Name</p>
            <p>Date: February 15, 2023</p>
        </div>
</div>
{% endfor %}
