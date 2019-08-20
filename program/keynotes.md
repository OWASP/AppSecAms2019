---
title: Keynotes
---

<div class="keynote-full">
	
	<ul>
	{% for speaker in site.data.keynotes %}
		{% if speaker.name %}
		<li>
			<a name="{{speaker.name}}">
			<img style="background-image: url(/assets/images/keynotes/{{speaker.image | default: 'no-person.png'}});{{speaker.style}};"></a>
			<h4><a name="{{speaker.name}}">{{speaker.name}}</a></h4>
			<p>
				{{speaker.bio}}
			</p>
		</li>
		{% endif %}
	{% endfor %}
	</ul>
</div>