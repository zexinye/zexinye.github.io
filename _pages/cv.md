---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---


{% include base_path %}

Education
======
* Ph.D. in Economics, The Ohio State University, 2020–2026 (expected)
* M.S. in Economics, Southwestern University of Finance and Economics, 2016–2020
* B.A. in Economics, Southwestern University of Finance and Economics, 2012–2016



Field of Interest
======
Industrial Organization, Algorithm, Experiment
  


Working Papers
======
{% assign publications = site.research | where: "category", "workingpaper" | sort: "date" | reverse %}
{% for post in publications %}
  {% include archive-single_cv_wp.html %}
{% endfor %}
  
Publications
======
{% assign publications = site.research | where: "category", "publication" | sort: "date" | reverse %}
{% for post in publications %}
  {% include archive-single_cv_pub.html %}
{% endfor %}

Other Publications
======
{% assign others = site.research | where: "category", "others" | sort: "date" | reverse %}
{% for post in others %}
  {% include archive-single_cv_others.html %}
{% endfor %}