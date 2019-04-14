---
layout: page
title: Course Materials
permalink: /materials/
---

# Books
The required textbook for this course is [Artificial Intelligence: A Modern Approach (Third Edition)](http://aima.cs.berkeley.edu/), and a supplementary textbook (recommended, but not required) is [Artificial Intelligence: A New Synthesis](http://www.amazon.com/Artificial-Intelligence-Synthesis-Morgan-Kaufmann/dp/1558604677). Lecture material will be drawn from both textbooks, as well as from some of the recent online AI literature.

# Lectures
The following contains link to the lectures I give throughout the semester. Clicking the title of the week's lecture will go to a PDF.

<!--
embedded in the user's browser, by default. The bottom right icons link to the Github directory for the lecture (<i class="fab fa-github"></i>), the R Markdown document for the lecture (<i class="fab fa-r-project"></i>), and a PDF, embedded on Github, for the lecture (<i class="fas fa-file-pdf"></i>).
-->

<ul id="archive">
	{% for lectures in site.data.lectures %}
	<li class="archiveposturl">
		<span>
			<a href="{{ site.url }}/{{ lectures.dirname }}/{{ lectures.filename }}.pdf">{{ lectures.title }}</a>
		</span>
		<br>
		<span>
			<strong> Week: </strong> {{ lectures.week }}
			<strong> Date: </strong> {{ lectures.date }}
		</span>
		<br>
		<span class = "postlower">
		<strong>
			Details:
		</strong>
			{{ lectures.tldr }}
		</span>
		<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right">
			<a href="https://github.com/{{ site.githubdir}}/tree/master/{{ lectures.dirname }}">
				<i class="fab fa-github"></i></a>
			&nbsp;&nbsp;
			<a href="https://github.com/{{ site.githubdir}}/tree/master/{{ lectures.dirname }}/{{ lectures.filename}}.Rmd">
				<i class="fab fa-r-project"></i></a>
			&nbsp;&nbsp;
			<a href="https://github.com/{{ site.githubdir}}/blob/master/{{ lectures.dirname }}/{{ lectures.filename}}.pdf">
				<i class="fas fa-file-pdf"></i></a>
		</strong>
	</li>
	{% endfor %}
</ul>

# Additional Course Materials
- [MIT Open Courseware - Artificial Intelligence Fall 2010](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-034-artificial-intelligence-fall-2010/)
- [Old Course Page - Dr. Mohsen Afsharchi](http://cv.znu.ac.ir/afsharchim/AI/AI.htm)
