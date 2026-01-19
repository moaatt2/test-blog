---
layout: post
title:  "Tetraorb Line"
date:   2026-01-18
families:
    - Japanese
image_path: "/assets/images/posts/2026_01_18_tetraorb_line"
model_path: "/assets/models/posts/2026_01_18_tetraorb_line"
main_image: "/tetraorb_line_flat.jpg"
image: "/assets/images/posts/2026_01_18_tetraorb_line/tetraorb_line_flat.jpg"
description: Join me in exploring the Tetraorb Line chainmaille weave.
tags: weave chain orbital tutorial interactive_model
---

### Overview

Continuing from the wonderful [Tetra Orb]({{ site.baseurl }}{% post_url 
2024-12-16-tetra-orb %}) weave (a personal top 10) is [Tetraorb Line](https://www.mailleartisans.org/weaves/weavedisplay.php?key=1046) as recorded by [Dr. T](https://www.mailleartisans.org/members/memberdisplay.php?key=3550) on [M.A.I.L.](https://www.mailleartisans.org/) This member of the [Japanese]({{ site.baseurl }}{{ site.family_page }}#Japanese) weave family is a very straightforward variant of Tetra Orb. Unfortunately, I was unable to find a preexisting tutorial, so I wrote and included [this one](#tutorial) for anyone who wanted to follow along.


### Materials

For the sample piece showcased in this post, I [made the rings myself]({{ site.baseurl }}{% post_url 2025-01-25-making-rings-at-home %}). I used 16 {% include abbreviations/swg.html %} Bright Aluminum wire from [The Ring Lord](https://theringlord.com/) coiled around a 10mm mandrel (for an approximate {% include abbreviations/id.html %} of 10mm) for an {% include abbreviations/ar.html %} of 6.15.


### Tutorial

This tutorial assumes you are familiar with creating Tetra Orbs. If you are not, please review [this tutorial](https://www.mailleartisans.org/articles/articledisplay.php?key=300) by [The Mad Mailler](https://www.mailleartisans.org/members/memberdisplay.php?key=2244).


1. Start with a single Tetra Orb. When done, it should look like this:

    <img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_step_01.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_01"></canvas>

2. Pick one of the six faces of the Tetra Orb for a direction to expand on. The direction I have chosen to expand is red in the image below:

    <img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_tutorial_02.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_02"></canvas>

3. Make a new Tetra Orb (green in the image below), and line it up with the face you chose to expand on. When done, it should look like this:

    <img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_tutorial_03.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_03"></canvas>

4. On the new Tetra Orb, remove the outside ring on the side opposite to where you will extend your chain (red in the image below).

    <img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_tutorial_04a.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_04"></canvas>

    When done, it should look like this:

    <img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_tutorial_4b.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_05"></canvas>

5. Join the new Tetra Orb to your chain by weaving the outermost ring on the side you are extending your chain (orange in the image below) through the same rings the ring you removed in the previous step went through (blue in the image below). Make sure to keep the orbital ring (yellow in the image below) in place, as it no longer orbits a connection:

    <img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_tutorial_5a.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_06"></canvas>

    When done, it should look like this:

    <img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_tutorial_5b.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_07"></canvas>

6. Repeat steps 2 through 5 until you are happy with the length of your chain.


### Notes

The Tetraorb Line weave is quite simple to understand, though it can be a bit tricky to make, particularly when joining units. Pay close attention, as mistakes can change the pattern of the rings joining the orbs. I find that the weave looks quite nice. While this is a chain weave, the large unit size makes it impractical for bracelets and chokers; instead, it is better suited for longer necklaces or for using shorter sections as earrings. Additionally, the weave has an internal cavity that allows for capturing small items such as marbles or minerals. I highly recommend using bent-nose pliers and, when joining units, to make it easier. Given its aesthetic appeal, relative ease of learning, and unique ability to capture multiple items, I highly recommend learning how to make the Tetraorb Line weave.


### Pictures

#### Flat

<img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_flat.jpg" style="width: min(750px, 100%)">


#### Flat: Angled

<img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_flat_angled.jpg" style="width: min(750px, 100%)">


#### Flat: Profile

<img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_flat_profile.jpg" style="width: min(750px, 100%)">


#### Vertical

<img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_vertical.jpg" style="max-height: min(750px, 95vh)">


#### Vertical: Profile

<img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_vertical_profile.jpg" style="max-height: min(750px, 95vh)">


#### In Process

<img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_step_01.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_step_02.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_step_03.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/tetraorb_line_step_04.jpg" style="max-height: min(200px, 95vh)">


### Interactive Model {% include 3d_model_instructions.html %}

{% assign path = site.baseurl | append: page.model_path | append: "/tetraorb_line.glb" %}
{% include 3d_model.html model=path %}

<!-- Includes for tutorial models -->
{% assign path = site.baseurl | append: page.model_path | append: "/tetraorb_line_step_01.glb" %}
{% include  3d_model.html model=path canvas_id="step_01" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/tetraorb_line_step_02.glb" %}
{% include  3d_model.html model=path canvas_id="step_02" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/tetraorb_line_step_03.glb" %}
{% include  3d_model.html model=path canvas_id="step_03" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/tetraorb_line_step_04.glb" %}
{% include  3d_model.html model=path canvas_id="step_04" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/tetraorb_line_step_05.glb" %}
{% include  3d_model.html model=path canvas_id="step_05" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/tetraorb_line_step_06.glb" %}
{% include  3d_model.html model=path canvas_id="step_06" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/tetraorb_line_step_07.glb" %}
{% include  3d_model.html model=path canvas_id="step_07" ignore_canvas="Yes" is_secondary="Yes" %}
