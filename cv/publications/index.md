---
title: Dr Paul Richmond - Publication Record
layout: homepage
---

# Journal Publications

<ul class="list-of-papers">
	{% for paper in site.data.journals %}
	<li> 
		<h3>"{{paper.title}}"</h3>
		<h4>{{paper.author-list}} ({{paper.year}})</h4>
		<p class="publication">{{paper.publication}}</p>
		{% if paper.url %}
			<a class="paper-button" href="{{paper.url}}">link</a>
		{% endif %}
		{% if paper.pdf %}
			<a class="paper-button" href="{{paper.pdf}}">pdf</a>
		{% endif %}
		{% if paper.abstract %}
			<input class="abstract-toggle" type="checkbox" id="abstract-toggle-{{forloop.index}}" />
			<label class="paper-button" for="abstract-toggle-{{forloop.index}}">Abstract</label>
		{% endif %}
		<p class="abstract">{{paper.abstract}}</p>
	</li>
	{% endfor %}
</ul>

# Conference Proceedings

<ul class="list-of-papers">
	{% for paper in site.data.conference %}
	<li> 
		<h3>"{{paper.title}}"</h3>
		<h4>{{paper.author-list}} ({{paper.year}})</h4>
		<p class="publication">{{paper.publication}}</p>
		{% if paper.url %}
			<a class="paper-button" href="{{paper.url}}">link</a>
		{% endif %}
		{% if paper.pdf %}
			<a class="paper-button" href="{{paper.pdf}}">pdf</a>
		{% endif %}
		{% if paper.abstract %}
			<input class="abstract-toggle" type="checkbox" id="abstract-toggle-{{forloop.index}}" />
			<label class="paper-button" for="abstract-toggle-{{forloop.index}}">Abstract</label>
		{% endif %}
		<p class="abstract">{{paper.abstract}}</p>
	</li>
	{% endfor %}
</ul>



