---
layout: post
title:  "Double Step"
# date:   2025-09-07
date: 2025-07-22
families:
    - European
    - Japanese
image_path: "/assets/images/posts/2025_09_07_double_step"
model_path: "/assets/models/posts/2025_09_07_double_step"
main_image: "/double_step_flat.jpg"
image: "/assets/images/posts/2025_09_07_double_step/double_step_flat.jpg"
description: Join me in exploring the Double Step chainmaille weave.
tags: weave chain kinged tutorial interactive_model
---

### Overview

While looking for new weaves to create, I discovered [Double Step](https://www.mailleartisans.org/gallery/gallerydisplay.php?key=8464) on [M.A.I.L.](https://www.mailleartisans.org/) by [Minigal](https://www.mailleartisans.org/members/memberdisplay.php?key=12389). This member of the [European]({{ site.baseurl }}{{ site.family_page }}#European) and [Japanese]({{ site.baseurl }}{{ site.family_page }}#Japanese) weave families is essentially a kinged [2-in-1 Chain]({{ site.baseurl }}{% post_url 2023-09-03-2-in-1-chain %}). If you are interested in making this weave yourself, I have created [this tutorial](#tutorial) as I couldn’t find any pre-existing ones.


### Materials

For the sample peice showcased in this post, I used three sizes of rings. The small rings, purchased from [The Ring Lord](https://theringlord.com/) are made from 18 {% include abbreviations/swg.html %} Copper wire with an {% include abbreviations/id.html %} of 3/16" for an {% include abbreviations/ar.html %} of 3.4. The medium rings, also purchased from [The Ring Lord](https://theringlord.com/), are made from 16 SWG Bright Aluminum wire with an {% include abbreviations/id.html %} of 1/4" for an {% include abbreviations/ar.html %} of 4. The large rings, which I [made myself]({{ site.baseurl }}{% post_url 2025-01-25-making-rings-at-home %}), have an {% include abbreviations/id.html %} of 10mm for an {% include abbreviations/ar.html %} of 6.15


### Tutorial

1. Pick either right or left as your direction and remember your choice. The images and models in this tutorial use right as the choice of direction.

2. Place the center of 1 medium ring in the center of 1 large ring. The medium ring should fit in the large ring, and the less space between them, the better. When done, it should look like this:

    <img src="{{ site.baseurl }}{{ page.image_path }}/double_step_step_01.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_01"></canvas>

3. Lay 1 new large ring and 1 new medium ring (green in the image below) on the rings from the previous step (blue in the image below) in the direction you chose in step 1. The edges of the rings should overlap. When done, it should look like this:

    <img src="{{ site.baseurl }}{{ page.image_path }}/double_step_tutorial_02_c.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_02"></canvas>

4. Join the rings from the last step (red in the image below) and the step before that (blue in the image below) together with 2 new small rings (green in the image below). When done, it should look like this:

    <img src="{{ site.baseurl }}{{ page.image_path }}/double_step_tutorial_03_c.jpg" class="post-tutorial-image-300">

    <canvas class="tutorial_canvas" id="step_03"></canvas>

5. Repeat steps 2 and 3 until you are happy with the length of your chain.

6. Enjoy your length of Double Step chain, or integrate it into a larger project.


### Notes

The Double Step weave is easy to understand and create, making it a great choice for beginners. It has an attractive appearance, although in my case, the AR difference between rings was a bit too high, resulting in a visible gap. For the weave to work, the large rings must have an AR at least 2 higher than the medium rings; however, the greater the AR gap, the larger the visible space between them. As a flat and wide chain weave, Double Step is great for making chokers and bracelets, but not cordage, as the small and thin rings joining units together make it weaker. Overall, given its good looks, ease of learning, and smooth creation process, I recommend learning how to make this weave.


### Pictures

#### Flat

<img src="{{ site.baseurl }}{{ page.image_path }}/double_step_flat.jpg" style="width: min(750px, 100%)">


#### Flat: Angled

<img src="{{ site.baseurl }}{{ page.image_path }}/double_step_flat_angled.jpg" style="width: min(750px, 100%)">


#### Flat: Profile

<img src="{{ site.baseurl }}{{ page.image_path }}/double_step_flat_profile.jpg" style="width: min(750px, 100%)">


#### Vertical

<img src="{{ site.baseurl }}{{ page.image_path }}/double_step_vertical.jpg" style="max-height: min(750px, 95vh)">


#### Vertical: Profile

<img src="{{ site.baseurl }}{{ page.image_path }}/double_step_vertical_profile.jpg" style="max-height: min(750px, 95vh)">


#### In Process

<img src="{{ site.baseurl }}{{ page.image_path }}/double_step_step_01.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/double_step_step_02.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/double_step_step_03.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/double_step_step_04.jpg" style="max-height: min(200px, 95vh)">


### Interactive Model {% include 3d_model_instructions.html %}

{% assign path = site.baseurl | append: page.model_path | append: "/double_step.glb" %}
{% include 3d_model.html model=path %}

<!-- Includes for tutorial models -->
{% assign path = site.baseurl | append: page.model_path | append: "/double_step_tutorial_01.glb" %}
{% include  3d_model.html model=path canvas_id="step_01" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/double_step_tutorial_02.glb" %}
{% include  3d_model.html model=path canvas_id="step_02" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/double_step_tutorial_03.glb" %}
{% include  3d_model.html model=path canvas_id="step_03" ignore_canvas="Yes" is_secondary="Yes" %}

<!-- 
* Model Rings:
    * AR Large  - Minor 0.20 | Major 1.40
    * AR Medium - Minor 0.20 | Major 0.95
    * AR Small  - Minor 0.15 | Major 0.73
-->
