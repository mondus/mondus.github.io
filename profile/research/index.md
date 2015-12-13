---
title: Dr Paul Richmond - Collaborative Research Team
layout: homepage
---

# Collaborative Research Team

In addition to providing [research software support](../rse) I lead a team of researchers (both RAs and PhDs) who work on collaborative projects utilising GPUs and complex systems simulation. The research projects that I engage in are interdisciplinary and have a strong focus on software. The difference between research support and collaborative research is that collaborative projects require fundamental software research to be carried out in supporting the larger collaborative goal. For example the development of the FLAME GPU software has required the development of novel techniques and methods which are in themselves publishable. In many cases it is possible to support research with software without collaboration, however collaborative projects offer a longer term embedding of research software developers into multi disciplinary teams. 

If you are interested in either software research support or developing a multidisciplinary proposal then please [contact me](../../contact).

# My Team 

My research team consists of the following people. Each of them work in developing software to facilitate research. If you are interested in working with me then please consider applying for any [Jobs and PhD studentships available](../../teaching/positions).



{% for person in site.data.team %}
<div class="team-member">
	<div class="team-member-img">
	<img src="{{person.img}}" alt="{{person.name}}">
	</div>
	<div> 
		<h3>{{person.name}}</h3>
		<h4><a href="{{person.website}}">{{person.website}}</a></h4>
		<p>{{person.description}}</p>
	</div>
</div>
{% endfor %}

