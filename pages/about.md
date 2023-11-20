---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi I am **{{ site.author.name }}**,<br>
<p>
A young programmer, not that young actually. Takes coding as both the job and hobby. Passionate about exploring and learning various new technologies.
</p>

<p>Get a little confused about both the World and Self. May pause or rest for some time, always chasing for better life and self-achievement. Interested in Distrubuted Systems and Deep Learning.
</p>


<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>
