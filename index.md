---
title: Portfolio
layout: landing
description: 'This is a list of all significant projects I have been working on.'
image: assets/images/code.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

<!-- One -->
<!--
<section id="one">
	<div class="inner">
		<header class="major">
			<h2>Sed amet aliquam</h2>
		</header>
		<p>Nullam et orci eu lorem consequat tincidunt vivamus et sagittis magna sed nunc rhoncus condimentum sem. In efficitur ligula tate urna. Maecenas massa vel lacinia pellentesque lorem ipsum dolor. Nullam et orci eu lorem consequat tincidunt. Vivamus et sagittis libero. Nullam et orci eu lorem consequat tincidunt vivamus et sagittis magna sed nunc rhoncus condimentum sem. In efficitur ligula tate urna.</p>
	</div>
</section>
-->
<!-- Two -->
<section id="two" class="spotlights">
{% assign sorted-projects = site.projects | reverse %}
{% for project in sorted-projects %}
	<section>
		<a href="{{ project.url }}" class="image">
			<img src="{{ site.baseurl }}/{{ project.image }}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
				</header>
				<p>{{ project.description }}</p>
			</div>
		</div>
	</section>
{% endfor %}
</section>

<!-- Three -->
<section id="three">
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
