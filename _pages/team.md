---
layout: page
permalink: /team/
title: team
nav: true
nav_order: 2
---

<div class="container">
	{%- assign people = site.people | sort: "order" -%}
	{%- assign pi = people | where: "status", "PI" -%}
	{%- assign current = people | where: "status", "Current" -%}
	{%- assign alumni = people | where: "status", "Alumni" -%}
	{%- assign unspecified = people | where_exp: "p", "p.status == nil" -%}
	{%- assign current = current | concat: unspecified -%}

	{%- if pi.size > 0 -%}
	<h2 class="mt-3">PI</h2>
	{%- for person in pi -%}
	<div class="row mb-4 align-items-center person-row">
		<div class="col-12 col-md-3 text-center mb-3 mb-md-0">
				{%- if person.photo -%}
				<img src="{{ '/assets/img/people/' | append: person.photo | relative_url }}" alt="{{ person.name }}" class="img-fluid rounded">
				{%- endif -%}
		</div>
		<div class="col-12 col-md-9">
			<h3 class="mb-1">{{ person.name }}</h3>
			{%- if person.role -%}
			<p class="text-muted mb-2">{{ person.role }}</p>
			{%- endif -%}
			<p class="mb-2">{{ person.blurb }}</p>
			<p class="mb-0">
				{%- if person.email -%}<a href="mailto:{{ person.email }}" class="mr-3" aria-label="email"><i class="fas fa-envelope"></i></a>{%- endif -%}
				{%- if person.scholar -%}<a href="{{ person.scholar }}" class="mr-3" aria-label="scholar"><i class="fas fa-graduation-cap"></i></a>{%- endif -%}
				{%- if person.website -%}<a href="{{ person.website }}" class="mr-3" aria-label="website"><i class="fas fa-link"></i></a>{%- endif -%}
				{%- if person.github -%}<a href="{{ person.github }}" class="mr-3" aria-label="github"><i class="fab fa-github"></i></a>{%- endif -%}
			</p>
		</div>
	</div>
	{%- endfor -%}
	{%- endif -%}

	{%- if current.size > 0 -%}
	<h2 class="mt-3">Current</h2>
	{%- for person in current -%}
	<div class="row mb-4 align-items-center person-row">
		<div class="col-12 col-md-3 text-center mb-3 mb-md-0">
				{%- if person.photo -%}
				<img src="{{ '/assets/img/people/' | append: person.photo | relative_url }}" alt="{{ person.name }}" class="img-fluid rounded">
				{%- endif -%}
		</div>
		<div class="col-12 col-md-9">
			<h3 class="mb-1">{{ person.name }}</h3>
			{%- if person.role -%}
			<p class="text-muted mb-2">{{ person.role }}</p>
			{%- endif -%}
			<p class="mb-2">{{ person.blurb }}</p>
			<p class="mb-0">
				{%- if person.email -%}<a href="mailto:{{ person.email }}" class="mr-3" aria-label="email"><i class="fas fa-envelope"></i></a>{%- endif -%}
				{%- if person.scholar -%}<a href="{{ person.scholar }}" class="mr-3" aria-label="scholar"><i class="fas fa-graduation-cap"></i></a>{%- endif -%}
				{%- if person.website -%}<a href="{{ person.website }}" class="mr-3" aria-label="website"><i class="fas fa-link"></i></a>{%- endif -%}
				{%- if person.github -%}<a href="{{ person.github }}" class="mr-3" aria-label="github"><i class="fab fa-github"></i></a>{%- endif -%}
			</p>
		</div>
	</div>
	{%- endfor -%}
	{%- endif -%}

	{%- if alumni.size > 0 -%}
	<h2 class="mt-3">Alumni</h2>
	{%- for person in alumni -%}
	<div class="row mb-4 align-items-center person-row">
		<div class="col-12 col-md-3 text-center mb-3 mb-md-0">
				{%- if person.photo -%}
				<img src="{{ '/assets/img/people/' | append: person.photo | relative_url }}" alt="{{ person.name }}" class="img-fluid rounded">
				{%- endif -%}
		</div>
		<div class="col-12 col-md-9">
			<h3 class="mb-1">{{ person.name }}</h3>
			{%- if person.role -%}
			<p class="text-muted mb-2">{{ person.role }}</p>
			{%- endif -%}
			<p class="mb-2">{{ person.blurb }}</p>
			<p class="mb-0">
				{%- if person.email -%}<a href="mailto:{{ person.email }}" class="mr-3" aria-label="email"><i class="fas fa-envelope"></i></a>{%- endif -%}
				{%- if person.scholar -%}<a href="{{ person.scholar }}" class="mr-3" aria-label="scholar"><i class="fas fa-graduation-cap"></i></a>{%- endif -%}
				{%- if person.website -%}<a href="{{ person.website }}" class="mr-3" aria-label="website"><i class="fas fa-link"></i></a>{%- endif -%}
				{%- if person.github -%}<a href="{{ person.github }}" class="mr-3" aria-label="github"><i class="fab fa-github"></i></a>{%- endif -%}
			</p>
		</div>
	</div>
	{%- endfor -%}
	{%- endif -%}
</div>
