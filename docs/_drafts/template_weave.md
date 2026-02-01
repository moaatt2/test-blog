---
layout: post
title:  "Post Template"
# date:   2025-04-20
families:
    - European
    - Japanese
    - Persian
image_path: "/assets/images/posts/2025_04_20_4_in_2_chain"
model_path: "/assets/models/posts/2025_04_20_4_in_2_chain"
main_image: "/4_in_2_chain_flat.jpg"
image: "/assets/images/posts/2025_04_20_4_in_2_chain/4_in_2_chain_flat.jpg"
description: Join me in exploring the 4-in-2 Chain chainmaille weave.
tags: weave chain kinged tutorial interactive_model
---

### Overview

TODO

Field                | Value
---------------------|---------
Weave Link           | N/A
Weave Author         | N/A
Weave Author Link    | N/A
tutorial Link        | N/A
Tutorial Author      | N/A
Tutorial Author Link | N/A


### Materials

TODO


### Tutorial

TODO



### Notes

TODO


### Pictures

#### Flat

<img src="{{ site.baseurl }}{{ page.image_path }}/4_in_2_chain_flat.jpg" style="width: min(750px, 100%)">


#### Flat: Angled

<img src="{{ site.baseurl }}{{ page.image_path }}/4_in_2_chain_flat_angled.jpg" style="width: min(750px, 100%)">


#### Flat: Profile

<img src="{{ site.baseurl }}{{ page.image_path }}/4_in_2_chain_flat_profile.jpg" style="width: min(750px, 100%)">


#### Vertical

<img src="{{ site.baseurl }}{{ page.image_path }}/4_in_2_chain_vertical.jpg" style="max-height: min(750px, 95vh)">


#### Vertical: Profile

<img src="{{ site.baseurl }}{{ page.image_path }}/4_in_2_chain_vertical_profile.jpg" style="max-height: min(750px, 95vh)">


#### In Process

<img src="{{ site.baseurl }}{{ page.image_path }}/4_in_2_chain_step_01.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/4_in_2_chain_step_02.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/4_in_2_chain_step_03.jpg" style="max-height: min(200px, 95vh)">

<br>

<img src="{{ site.baseurl }}{{ page.image_path }}/4_in_2_chain_step_04.jpg" style="max-height: min(200px, 95vh)">


### Interactive Model {% include 3d_model_instructions.html %}

{% assign path = site.baseurl | append: page.model_path | append: "/4_in_2_chain.glb" %}
{% include 3d_model.html model=path %}

<!-- Includes for tutorial models -->
{% assign path = site.baseurl | append: page.model_path | append: "/4_in_2_chain_tutorial_01.glb" %}
{% include  3d_model.html model=path canvas_id="step_01" ignore_canvas="Yes" is_secondary="Yes" %}
{% assign path = site.baseurl | append: page.model_path | append: "/4_in_2_chain_tutorial_02.glb" %}
{% include  3d_model.html model=path canvas_id="step_02" ignore_canvas="Yes" is_secondary="Yes" %}

<!-- 
* Model Rings:
    * AR 3.7 - Minor 0.2 | Major 0.94
-->
