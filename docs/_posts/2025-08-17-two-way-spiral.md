---
layout: post
title:  "Two-Way Spiral"
date:   2025-08-17
families:
    - Mobius
image_path: "/assets/images/posts/2025_08_17_two_way_spiral"
model_path: "/assets/models/posts/2025_08_17_two_way_spiral"
main_image: "/two_way_spiral_flat.jpg"
image: "/assets/images/posts/2025_08_17_two_way_spiral/two_way_spiral_flat.jpg"
description: Join me in exploring the Two-Way Spiral chainmaille weave.
tags: weave chain spiral tutorial interactive_model aluminum
---

### Overview

I was recently browsing [M.A.I.L.](https://www.mailleartisans.org/) for new weaves to try, and I came across [Two Way Spiral](https://www.mailleartisans.org/weaves/weavedisplay.php?key=124) by [sakredchao](https://www.mailleartisans.org/members/memberdisplay.php?key=21). This member of the [Mobius]({{ site.baseurl }}{{ site.family_page }}#Mobius) weave family is an interesting weave that has spirals in two opposite directions. Unfortunately, I was unable to find any tutorials for this weave, so I wrote and included [this one](#tutorial).


### Materials

The rings used for the sample piece shown in this post are 16 {% include abbreviations/swg.html %} with a 1/4" {% include abbreviations/id.html %} for an {% include abbreviations/ar.html %} of 4.03 made of Bright Aluminum that I bought from the [Ring Lord](https://theringlord.com/).


### Tutorial

1. Start with 1 ring.

    <img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_tutorial_01.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_01"></canvas>

2. Add 1 new ring (green in the image below) through the ring from the last step (yellow in the image below). When done, it should look like this:

    <img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_tutorial_02_c.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_02"></canvas>

3. Add 1 new ring (green in the image below) around the <abbr title="" data-tippy-content='Read more about chainmail eyes <a href="{{ site.baseurl }}{{ site.glossary_page }}#eye">here<a>'>eye</abbr> (orange in the image below) formed by the ring from the last step (blue in the image below) and the ring from the step before that (yellow in the image below). Ensure you consistently add the new ring either under or over the ring from the previous step (blue in the image below). When done, it should look like this:

    <img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_tutorial_03_c.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_03"></canvas>

4. First, ensure that the ring from the previous step (red in the image below) and the ring from the step before that (blue in the image below) have different leans (they should not form a two-ring Mobius ball). Then add 1 new ring (green in the image below) through the rings from the last two steps (red and blue in the image below). The new ring should be perpendicular to the ring from three steps ago (yellow in the image below). When done, it should look like this:

    <img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_tutorial_04_c.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_04"></canvas>

5. Repeat steps 2 through 4 until you are happy with the length of the weave.

6. Enjoy the neat weave you just made.


### Notes

Two-way spiral is a fairly simple weave to understand and very easy to create. However, the ease of learning can be deceptive; maintaining a consistent ring order is essential. I find the weave to be quite visually appealing. With its round cross-section and small unit size, it is well suited for bracelets, necklaces, and dangling earrings. Given its attractive appearance, straightforward construction, and versatility, I recommend learning to make this weave.


### Pictures

#### Flat

<img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_flat.jpg" style="width: min(750px, 100%)">


#### Flat: Angled

<img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_flat_angled.jpg" style="width: min(750px, 100%)">


#### Flat: Profile

<img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_flat_profile.jpg" style="width: min(750px, 100%)">


#### Vertical

<img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_vertical.jpg" style="max-height: min(750px, 95vh)">


#### Vertical: Profile

<img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_vertical_profile.jpg" style="max-height: min(750px, 95vh)">


#### In Process

<img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_step_01.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_step_02.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_step_03.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/two_way_spiral_step_04.jpg" style="max-height: min(200px, 95vh)">


### Interactive Model {% include 3d_model_instructions.html %}

{% assign path = site.baseurl | append: page.model_path | append: "/two_way_spiral.glb" %}
{% include 3d_model.html model=path %}

<!-- Includes for tutorial models -->
{% assign path = site.baseurl | append: page.model_path | append: "/two_way_spiral_tutorial_01.glb" %}
{% include  3d_model.html model=path canvas_id="step_01" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/two_way_spiral_tutorial_02.glb" %}
{% include  3d_model.html model=path canvas_id="step_02" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/two_way_spiral_tutorial_03a.glb" %}
{% include  3d_model.html model=path canvas_id="step_03" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/two_way_spiral_tutorial_04.glb" %}
{% include  3d_model.html model=path canvas_id="step_04" ignore_canvas="Yes" is_secondary="Yes" %}

<!-- 
* Model Rings:
    * AR 4.0 - Minor 0.18 | Major 1.00
-->
