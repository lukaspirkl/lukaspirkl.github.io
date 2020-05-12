---
title: Portfolio
layout: landing
description: 'This is a list of all significant projects I have been working on.'
image: assets/images/code.jpg
nav-menu: true
---

<div id="main">

<section class="spotlights">
{% for project in site.projects reversed %}
	<section>
		<a href="{{ project.url }}" class="image">
			<img src="{{ site.baseurl }}/{{ project.image }}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<div class="row">
					<div class="6u 12u$(small)">
						<header class="major">
							<h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
						</header>
					</div>
					<div class="6u 12u$(small)" style="text-align-last: right;">
						<p>
							{% for tag in project.tags %}
								<span class="msc-badge msc-badge__blue">{{tag}}</span>
							{% endfor %}
						</p>
					</div>
				</div>
				{{ project.description | markdownify }}
				<b>{{ project.accolades | markdownify }}</b>
				<ul class="actions small">
					<li><a href="{{ project.url }}" class="button small">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
{% endfor %}
</section>

<section>
	<div class="inner">
		<header class="major">
			<h2>Other projects</h2>
		</header>
		<p>
			<b><a href="https://lowcase.itch.io/procedural-audio-prototype/">Procedural audio prototype</a></b>
			<ul>
				<li>submission to <a href="https://itch.io/jam/procjam/">PROCJAM - The Procedural Generation Jam</a></li>
				<li>proof of concept that combines <a href="https://puredata.info/">Pure Data</a> and <a href="https://love2d.org/">LÖVE</a> to have procedurally generated sounds in a simple game</li>
			</ul>
		</p>
		<p>
			<b><a href="https://github.com/lukaspirkl/AdventOfCode/">Advent of Code</a></b>
			<ul>
			<li>solutions for programming puzzles</li>
			<li>for fun and to improve my C++ skills</li>
			</ul>
		</p>
	</div>
</section>

</div>
