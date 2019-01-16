Steve's No-Good-Very-Bad Course Website Jekyll Template
=======================================================

This repository contains a Jekyll template, patterned entirely off my no-good-very-bad Jekyll Template at [svmiller.com](http://svmiller.com), for organizing a course website. I should note that because I ganked it from my website template, there's a lot of empty tags in the template that make reference to things that don't appear in the main `.yml` file. In other words, they reference things that should be there but, because they're not there, ultimately won't interfere with how the site renders.

Here are the things you should tweak to make it your own:

- `_config.yml`. Naturally. This should be familiar if you're accustomed to Jekyll. Do note, for convenience, that I made the `syllabus` field a full URL entry. You should also fill out the `githubdir` field since the goal is to make your course (and, by extension, the knowledge you propose to communicate) open source and reproducible on Github. Let us know where it is.
- `course-materials.md`: Fudge this to add in helpful information about your course (e.g. the book and whatever else you want to communicate).
- `index.html`: You won't need to edit much but, if you want your own lead image for your course website that's *not* from *Stand and Deliver* (I don't know why you would do this, but, hey, it's your class...), edit that Jekyll liquid tag I created that embeds images in my spiffy way. This should be intuitive. Just specify a relative path for the image you want to use, how wide you want it to be, and whatever caption you want to add to it.
- `_data/lectures.yml`: This uses YAML data to render Github and local links to lectures. This should be straightforward (see my example file) but [feel free to look at this tutorial](https://jekyllrb.com/docs/datafiles/) if you want to better understand what's happening here. You could also edit `lectures.md` if, for example, you render your lectures to HTML in lieu of PDF. I do PDF. Changing this isn't hard, though, and should be straightforward. Basically, change ".pdf" to ".html" as you see it and then, probably, find a nice icon for HTML on [Font Awesome](https://fontawesome.com/).
- `_includes/nav.html`: You won't have to tweak this, per se, but you may want to if, for example, you want to add a course blog. I don't do that, but I do prove a `blog.md` file. Head to [Font Awesome](https://fontawesome.com/) if you're looking for the perfect icon to go with it.
- `CNAME`: Adding a special domain or subdomain to your course website? Change it here. Is its own Github page on a special account you created on Github (but you're *not* using a special domain on top of that [[example](https://github.com/uw-csss-564)])? Delete it.

You can see a snapshot of what it looks like below. You can also try it out here: [http://course-website.svmiller.com/](http://course-website.svmiller.com/)

![Snapshot](_images/snapshot.png)

Feel free to contact me at svmille@clemson.edu. Send along some cheers too if you find it useful.