---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: defaultcoronainfo
 
---

<div>
 {% for page in site.pages %}
        {% if page.exclude != true %} 
        <p>
        <a href="{{site.canonical_domain}}{{site.baseurl}}{{ page.url }}"> 
         {{site.canonical_domain}}{{site.baseurl}}{{ page.url }}
        </a>
        </p> 
        {% endif %}
     {% endfor %}
    {% for item in site.posts %}
   {% if page.exclude != true %}
            {{site.canonical_domain}} {{site.baseurl}} {{ item.url }} 
  {% endif %}
  {% endfor %}
 </div>

 <br>
 <br>
 <br>
 <br>
 <br>
 <br>
