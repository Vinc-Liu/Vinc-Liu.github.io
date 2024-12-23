# 📝 Publications

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

# 读取publications这个colloction里面的所有内容并按 archive-single的格式渲染出来
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
