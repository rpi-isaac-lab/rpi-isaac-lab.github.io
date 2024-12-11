---
layout: page
title: Acknowledgements
permalink: /acknowledgements/
nav: true
nav_order: 6
groups:
- image: nsf.jpg
  link: https://www.nsf.gov/
  name: National Science Foundation

- image: lesa.jpg
  link: https://lesa.rpi.edu/
  name: Light Enabled Systems and Applications

- image: sikorsky.jpg
  link: https://www.lockheedmartin.com/en-us/capabilities/sikorsky.html
  name: Sikorsky

- image: nystar.jpg
  link: https://esd.ny.gov/innovation-development-support
  name: NY STAR

- image: cats.jpg
  link: https://research.rpi.edu/research-centers/center-automation-technologies-and-systems-cats
  name: Center for Automation Technologies and Systems

- image: doe.jpg
  link: https://www.energy.gov/
  name: US Dept of Energy

- image: onr.jpg
  link: https://www.onr.navy.mil/
  name: US Office of Naval Research

- image: nyserda.jpg
  link: https://www.nyserda.ny.gov/
  name: NYSERDA

- image: cnpq.jpg
  link: https://www.gov.br/cnpq/pt-br
  name: Conselho Nacional de Sesenvolvimento Cientifico e Technologico

- image : linksim.png
  link: https://linksim.org/
  name: LINKSIM
---

Funding agencies and research partners:

{% assign cols = 3 %}

{% assign max_rows = page.groups | size | divided_by: cols %}

<div class="grid-container-container">
{% for i in (0..max_rows) %}
	{% assign offnum = i | times: cols %}
	<div class="grid-container">
	{% for group in page.groups offset:offnum limit:cols %}
		{% assign image_path = group.image | prepend: 'assets/acknowledgements/' %}
		<div class="grid-item">
		{% include figure.liquid loading="eager" path=image_path class=image_class sizes=sizes alt=group.name link=group.link %}
		</div>
	{% endfor %}
	</div>
{% endfor %}
</div>
