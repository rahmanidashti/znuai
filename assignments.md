---
layout: page
title: TAs and Assignments
permalink: /assignments/
---

# Assignments
The following contains link to the assignments I give throughout the semester.

<!--
embedded in the user's browser, by default. The bottom right icons link to the Github directory for the lecture (<i class="fab fa-github"></i>), the R Markdown document for the lecture (<i class="fab fa-r-project"></i>), and a PDF, embedded on Github, for the lecture (<i class="fas fa-file-pdf"></i>).
-->

<ul id="archive">
	{% for assignments in site.data.assignments %}
	<li class="archiveposturl">
		<span>
			<a href="{{ site.url }}/{{ assignments.dirname }}/{{ assignments.filename }}.pdf">{{ assignments.title }}</a>
		</span>
		<br>
		<span>
			<strong> Due Date: </strong> <span style="font-color:red"> {{ assignments.duedate }} </span>
		</span>
		<br>
		<span class = "postlower">
		<strong>
			Details:
		</strong>
			{{ assignments.tldr }}
		</span>
		<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right">
			<!-- <a href="https://github.com/{{ site.githubdir}}/tree/master/{{ assignments.dirname }}">
				<i class="fab fa-github"></i></a>
			&nbsp;&nbsp; -->
			<a href="https://github.com/{{ site.githubdir}}/tree/master/{{ assignments.dirname }}/{{ assignments.filename}}.zip">
				<i class="fab fa-r-project"></i></a>
			&nbsp;&nbsp;
			<!-- <a href="https://github.com/{{ site.githubdir}}/blob/master/{{ assignments.dirname }}/{{ assignments.filename}}.pdf">
				<i class="fas fa-file-pdf"></i></a> -->
		</strong>
	</li>
	{% endfor %}
</ul>
