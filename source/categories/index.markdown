---
layout: page
title: "categories"
date: 2013-06-29 14:16
comments: false
sharing: true
footer: true
---
<script type="text/javascript" src="/javascripts/sort.js"></script>
<script type="text/javascript">
	window.onload = function() {
		//sortUnorderedList('categories');
	}
</script>
<ul id="categories">
{% for item in site.categories %}
    <li><a href="/categories/{{ item[0] }}/">{{ item[0] | capitalize }}</a> [ {{ item[1].size }} ]</li>
{% endfor %}
</ul>
