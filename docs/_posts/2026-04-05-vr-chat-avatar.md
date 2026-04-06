---
layout: project_post
title:  "Chainmail VRChat Avatar"
date:   2026-04-05
start_date: 2026-03-14
completion_date: 2026-04-05
weaves:
    - 2-in-1 Chain
image_path: "/assets/images/posts/2026_04_05_vr_chat_avatar"
model_path: "/assets/models/posts/2026_04_05_vr_chat_avatar"
main_image: "/mr_chain_vrc_standing.png"
image:      "/assets/images/posts/2026_04_05_vr_chat_avatar/mr_chain_vrc_standing.png"
description: Joing me on a journey of learning how to create custom avatars for VRChat.
tags: project colorful vrchat 3d_modelling interactive_model
---

<!-- General thoughts: -->
<!--    Should I replace (photo) with a plain link where possible? -->
<!--    Should Mr Stick V2 get 2 limb adjustment photos? -->
<!--    Investigate making some photos taller -->

### Overview

I have always enjoyed [VRChat](https://hello.vrchat.com/) for both the creativity on display and the unique social experiences it allows. Ever since I started learning 3D modelling for chainmail, I have thought about making a custom avatar made of individual rings. With my other project blocked by shipping delays, I thought that it was a great time to make a chainmail-inspired VRChat avatar.I ended up making [this free avatar](https://vrchat.com/home/avatar/avtr_d45d5028-e101-481c-ae7d-069af28b8414). Read on to learn more about how I made it.


### Materials

For this project, there were no physical rings involved; instead, I used the following programs:
* [Blender](https://www.blender.org/)
* [VRChat (Steam)](https://store.steampowered.com/app/438100/VRChat/?utm-source=hello-home)
* [VRChat Creator Companion](https://vcc.docs.vrchat.com/)
* [Unity (Managed by VRChat Creator Companion)](https://unity.com/)


### Notes

#### Coming Up With The Idea

Originally, my plan for this month was to make chainmail coasters (coming next month). However, shipping delays on the ordered rings made it impossible to release this month. Without the ability to buy rings, I had two choices: make coasters with the rings I have on hand or find another project. Since I didn't have enough rings on hand to make anything interesting, I spent some time thinking about what to make. After some time thinking about what I could make without rings, I remembered my previous idea of making a custom VRChat avatar from rings; this was a perfect project given my current constraints and something I have wanted to do for a long time.


#### Making My First Avatar

This was the first time I had tried making a non-chainmail 3d model outside of following a step-by-step tutorial. So I decided to start as simply as possible by making a stick figure avatar. I opened Blender and laid out five cylinders for the limbs and torso, and a torus for the head ([photo](#mr-stick-v1-starting-body)). After that, I followed [FreedomArts3D](https://www.youtube.com/@FreedomArts3D)’s [tutorial](https://www.youtube.com/watch?v=tiKTq13ZA4I) on rigging models in Blender, resulting in attaching an armature to my model ([photo](#mr-stick-v1-with-skeleton)).


I was testing the newly rigged model in pose mode when I noticed that my arm looked quite bad as I bent it ([photo](#mr-stick-v1-bad-arm-bend)). I did some research and determined that it was because the arm had very few <abbr title="" data-tippy-content="Points where the object can bend.">verticies</abbr>. I decided to add more by doing some [loop cuts](https://docs.blender.org/manual/en/latest/modeling/meshes/tools/loop.html) ([photo](#mr-stick-v1-arm-loop-cuts)). The arm was able to bend much more cleanly with the loop cuts in place ([photo](#mr-stick-v1-good-arm-bend)). Assuming that would improve all other limbs and the torso, I applied loop cuts to them, applied my standard ring grey ([photo](#mr-stick-v1-standard-grey)), set smooth shading and added my favourite black outline ([photo](#mr-stick-v1-smoothed-and-outline)) before finally exporting the model as an FBX file ([settings photo](#fbx-export-settings)) in preparation for loading the model into Unity.


To learn the process of taking a 3d model and creating a VRChat avatar, I followed VRChat’s [Creating Your First Avatar tutorial](https://creators.vrchat.com/avatars/creating-your-first-avatar/). Following the tutorial, I installed the VRChat creator companion and created a project ([photo](#vrchat-creator-companion-project)) using the default packages ([photo](#vrchat-creator-default-packages)). Then I loaded up Unity, imported my model ([photo](#mr-stick-v1-in-unity)), added a VRC Avatar Descriptor ([photo](#unity-vrc-avatar-descriptor)), set the view height (red in [this image](#unity-vrc-avatar-descriptor)) and left the lip syncing alone (green in [this image](#unity-vrc-avatar-descriptor)) as the model has no mouth/facial features. Continuing with the tutorial, I opened the build tab to see if the avatar had issues. While I was there, I noticed that the avatar was missing an animator ([photo](#unity-missing-animator)).


Unfortunately, adding animators was not covered in the tutorial, but after some investigation, I found a solution. The first step was to create a rig ([photo](#unity-create-animator)) by going to the avatar asset’s rig tab (green in [this image](#unity-create-animator)), selecting the ‘Humanoid’ animation type (red in [this image](#unity-create-animator)), then clicking apply (blue in [this image](#unity-create-animator)). Followed by clicking 'configure' (white in [this image](#unity-create-animator)) to open up the bone map interface ([photo](#unity-bone-map-interface)) to map the Blender bones to the ones VRChat expects. It was a fairly simple process where all I had to do was [unmap the toe bones](#unity-unmap-toes) and [unmap the right eye](#unity-unmap-right-eye). To cement the mapping, all I had to do was hit apply (red in [this image](#unity-bone-map-interface)), then done (green in [this image](#unity-bone-map-interface)).


With my new animator, I reopened the build tab ([photo](#unity-final-prep-and-publish)) for the final prep. First, I set a name, styles, image, and description (green in [this image](#unity-final-prep-and-publish)). Then I clicked Auto Fix for all issues where it was available (orange in [this image](#unity-final-prep-and-publish)). I ignored the degraded ik/full-body tracking issues (yellow in [this image](#unity-final-prep-and-publish)) and planned to address the issues related to using multiple objects (white in [this image](#unity-final-prep-and-publish)) in the next version. Finally, I pressed ‘Build & Publish’ (blue in [this image](#unity-final-prep-and-publish)), booted up VRChat, selected my new avatar and stood in front of a mirror ([photo](#mr-stick-version-1)).

When I stood in front of the mirror and selected my custom avatar, I was happy and proud that I had finally accomplished this task I had wanted to do for a long time. Then I noticed the shoulders being brought forward and separate from the torso, the knees bending backwards, and the torso flapping when I moved. This convinced me that I needed to try again with a new model and address these issues.


### Improving My First Avatar

After finishing my first custom avatar and recognizing its flaws, I wanted to try remaking it before moving on. This time, I started with a similar base model ([photo](#mr-stick-v2-base-model)); however, I chose a <abbr title="" data-tippy-content="Default model pose where arms are horizontal making the model look like a capital T.">T-Pose</abbr> instead of an <abbr title="" data-tippy-content="Default model pose where arms are partially stretched out making the model somewhat resemble a capital A.">A-Pose</abbr> since that is the default pose Unity expects, and I hoped it would avoid the weird arm stretch the last model had. Additionally, I merged all the meshes into one to de-duplicate <abbr title="" data-tippy-content="For these models materials define the color of an object.">materials</abbr> in the model and use a single mesh to address issues from the build menu of the last model. To view an interactive version of the model at this stage, go [here](#mr-stick-version-2-1).

With the base model in place, I only needed to add the rigging following the same tutorial as last time ([photo](#mr-stick-v2-model-with-armature)), with one small adjustment this time. Instead of having the arm and leg joints perfectly straight, I moved the middle arm joint slightly to the back and the middle leg joint slightly forward ([photo](#mr-stick-v2-slight-limb-armature-adjustments)) so that Unity can determine the proper bend angle.

After touching up the armature, I used the same export, project creation, model import ([photo](#mr-stick-v2-model-in-unity)), and model rig creation settings. With the improved armature, the model bones in Unity ([photo](#mr-stick-v2-model-with-unity-bones)) looked much better this time. Additionally, when I checked the VRC Build Menu ([photo](#mr-stick-v2-vrc-build-menu)), I had fewer problems since I had a single mesh and two distinct materials this time. In fact, I actually got a performance rating of ‘Good’.

After the build, I opened VRChat, selected my new avatar, and looked at it in a mirror ([photo](#mr-stick-version-2)). The shoulders were a bit awkward, there was some outline clipping where the limbs intersected the torso, and the crouch looked weird in the knees. I was still happy as this model was much better than the last one. The majority of the issues were minor and would not affect the next version due to differences in construction, so I saw fit to move on to the next stage.


### Making Mr Chain

Now that I had an avatar that met my standards, it was time to move to the main event, a VRChat avatar out of chainmail. I started with a base model made from [2-in-1 Chain]({{ site.baseurl }}{% post_url 2023-09-03-2-in-1-chain %}) ([photo](#mr-chain-base-model), [interactive model](#mr-chain-1)). I added an armature ([photo](#mr-chain-model-with-armature)) following the steps I learned making Mr Stick V2, imported the model into Unity ([photo](#mr-chain-in-unity)), mapped the bones to Unity ([photo](#mr-chain-unity-bone-mapping)), and published using the VRC Build Menu ([photo](#mr-chain-vrc-build-menu)) with an overall performance rating of ‘Good’.


After the build, I opened VRChat, selected my new avatar, and looked at it in a mirror ([photo](#mr-chain)). The rings for the shoulders, hands, feet, and pelvis did bend; however, I felt elated at seeing my vision come to life. If you want to use it as your avatar, you can find it [here](https://vrchat.com/home/avatar/avtr_d45d5028-e101-481c-ae7d-069af28b8414).


### Making Custom Variants

After making Mr Chain, I knew I wanted to make the model public. I still wanted a custom version for myself, so I made [Mr Chain M Special](#mr-chain-m-special). To do this, modified the materials I used to make Mr Chain so that I would have a special avatar just for me that fit my favourite colour scheme.

A friend whom I typically play VRChat saw my unique variant and asked for one of their own, so I made her [Mrs Chain T Special](#mrs-chain-t-special). This one called for [three different materials](#mrs-chain-t-special-3-materials), which meant I had to [tweak](#mrs-chain-t-special-tweaked-solidfy-modifier) my usual <abbr title="" data-tippy-content="This is what I use to give my rings an outline regardless of the angle you look at them.">solidify modifier</abbr>. The last change I incorporated was making a [bow](#mrs-chain-t-special-cute-bow) by sticking two cones together, and moving that to the head ring of the model.


### Future Improvement Notes

Given the time constraints I worked under, I am happy with the amount I learned, and I think the avatars I made are a great initial step into the world of 3D modelling and rigging. I can see three primary ways to improve upon the current Mr Chain: make each ring solid and non-deforming, replace the 2-in-1 chain with a more complex weave, and add more details for more complex rigging.

I used Rigify's automatic weights for each avatar I made this month. These automatic weights were very easy to set up and performed wonderfully, although some rings had their verticies influenced by more than one bone. A ring whose vertices belong to more than one bone can be deformed when the model moves. To ensure that each ring is rigid during deformation, each ring must have its vertices influenced by only one bone. Doing this requires manually assigning the rings to the bones. Unfortunately, I did not have time to experiment with that this month.

Right now, Mr. Chain uses a very simple 2-in-1 Chain weave. I would like to use a more complex and visually appealing weave, as it is already more than halfway to VRChat's soft cap on the number of <abbr title="" data-tippy-content="Triangles are the fundamental primitive shapes that make up the mesh of all 3D models.">triangles</abbr> in a mesh. I can see two options to use a more complex weave while staying under the triangle limit: reduce the number of triangles per ring, or investigate texture painting and paint a weave texture on a simpler object.

Another interesting expansion that could be fun to try is setting up more complex rigging. I could try adding rings for eyes, a mouth or even fingers. Adding and rigging these additional features would require a more complex rig but would result in a more fleshed-out and expressive avatar that would map to the user’s body more closely.

Additionally, these three improvements are not mutually exclusive and could be combined to create an even better model. However, a rigged model VRChat avatar is not the only use case; it could be a VTuber avatar,  a game character, or a character in an animation. If I expand the scope of use cases for these skills beyond avatars, I could make VRChat worlds, video game assets, or interactive educational experiences. There is an amazing variety of uses for these skills. I found this project highly rewarding, and I get excited thinking about what else I could use these skills for. If I ever run out of ideas or experience another shipping delay, I may come back to this and try some of these extension ideas.


### Pictures

#### Mr Stick Version 1

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v1_vrc_standing.png" style="max-height: min(200px, 95vh)">
<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v1_vrc_sitting.png" style="max-height: min(200px, 95vh)">
<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v1_vrc_crouching.png" style="max-height: min(200px, 95vh)">


#### Mr Stick Version 2

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v2_vrc_standing.png" style="max-height: min(200px, 95vh)">
<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v2_vrc_sitting.png" style="max-height: min(200px, 95vh)">
<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v2_vrc_crouching.png" style="max-height: min(200px, 95vh)">


#### Mr Chain

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_vrc_standing.png" style="max-height: min(200px, 95vh)">
<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_vrc_sitting.png" style="max-height: min(200px, 95vh)">
<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_vrc_crouching.png" style="max-height: min(200px, 95vh)">


#### Mr Chain M Special

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_m_special_vrc_standing.png" style="max-height: min(200px, 95vh)">
<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_m_special_vrc_sitting.png" style="max-height: min(200px, 95vh)">
<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_m_special_vrc_crouching.png" style="max-height: min(200px, 95vh)">

#### Mrs Chain T Special

<img src="{{ site.baseurl }}{{ page.image_path }}/mrs_chain_vrc_standing.png" style="max-height: min(200px, 95vh)">
<img src="{{ site.baseurl }}{{ page.image_path }}/mrs_chain_vrc_sitting.png" style="max-height: min(200px, 95vh)">
<img src="{{ site.baseurl }}{{ page.image_path }}/mrs_chain_vrc_crouching.png" style="max-height: min(200px, 95vh)">


#### Mr Stick V1 Starting Body

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_progress_01_initial_body.png" style="max-height: min(200px, 95vh)">

#### Mr Stick V1 With Skeleton

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_progress_02_with_bones.png" style="max-height: min(200px, 95vh)">

#### Mr Stick V1 Bad Arm Bend

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_progress_03_bad_arm_bend.png" style="max-height: min(200px, 95vh)">

#### Mr Stick V1 Arm Loop Cuts

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_progress_04_arm_loop_cuts.png" style="max-height: min(200px, 95vh)">

#### Mr Stick V1 Good Arm Bend

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_progress_05_improved_arm_bend.png" style="max-height: min(200px, 95vh)">

#### Mr Stick V1 Standard Grey

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_progress_06_now_in_color.png" style="max-height: min(200px, 95vh)">

#### Mr Stick V1 Smoothed and Outline

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_progress_07_outline_and_smooth.png" style="max-height: min(200px, 95vh)">

#### Mr Stick V1 In Unity

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_progress_08_in_unity.png" style="max-height: min(200px, 95vh)">

#### Mr Stick V1 Bone Map

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_progress_09_bone_mapping_in_unity.png" style="max-height: min(200px, 95vh)">


#### FBX Export Settings

<img src="{{ site.baseurl }}{{ page.image_path }}/unity_step_00_fbx_export_settings.png" style="max-height: min(400px, 95vh)">


#### VRChat Creator Companion Project

<img src="{{ site.baseurl }}{{ page.image_path }}/unity_step_01_creator_companion_project.png" style="max-height: min(200px, 95vh)">


#### VRChat Creator Default Packages

<img src="{{ site.baseurl }}{{ page.image_path }}/unity_step_02_default_packages.png" style="max-height: min(200px, 95vh)">


#### Unity VRC Avatar Descriptor

<img src="{{ site.baseurl }}{{ page.image_path }}/unity_step_03_vrc_avatar_descriptor.png" style="max-height: min(200px, 95vh)">


#### Unity Missing Animator

<img src="{{ site.baseurl }}{{ page.image_path }}/unity_step_04_missing_animator.png" style="max-height: min(200px, 95vh)">

#### Unity Create Animator

<img src="{{ site.baseurl }}{{ page.image_path }}/unity_step_05_create_animator.png" style="max-height: min(200px, 95vh)">

#### Unity Bone Map Interface

<img src="{{ site.baseurl }}{{ page.image_path }}/unity_step_06_bone_map_interface.png" style="max-height: min(200px, 95vh)">

#### Unity Unmap Toes

<img src="{{ site.baseurl }}{{ page.image_path }}/unity_step_07_unmap_toes.png" style="max-height: min(200px, 95vh)">

#### Unity Unmap Right Eye

<img src="{{ site.baseurl }}{{ page.image_path }}/unity_step_08_unmap_right_eye.png" style="max-height: min(200px, 95vh)">

#### Unity Final Prep And Publish

<img src="{{ site.baseurl }}{{ page.image_path }}/unity_step_09_final_prep_and_publish.png" style="max-height: min(200px, 95vh)">


#### Mr Stick V2 Base Model

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v2_progress_01.png" style="max-height: min(200px, 95vh)">


#### Mr Stick V2 Model With Armature

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v2_progress_02.png" style="max-height: min(200px, 95vh)">


#### Mr Stick V2 Slight Limb Armature Adjustments

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v2_progress_03.png" style="max-height: min(200px, 95vh)">


#### Mr Stick V2 Model In Unity

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v2_progress_04.png" style="max-height: min(200px, 95vh)">


#### Mr Stick V2 Model With Unity Bones

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v2_progress_05.png" style="max-height: min(200px, 95vh)">


#### Mr Stick V2 VRC Build Menu

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_stick_v2_progress_06.png" style="max-height: min(200px, 95vh)">


#### Mr Chain Base Model

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_progress_01.png" style="max-height: min(200px, 95vh)">


#### Mr Chain Model With Armature

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_progress_02.png" style="max-height: min(200px, 95vh)">


#### Mr Chain In Unity

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_progress_03.png" style="max-height: min(200px, 95vh)">


#### Mr Chain Unity Bone Mapping

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_progress_04.png" style="max-height: min(200px, 95vh)">


#### Mr Chain VRC Build Menu

<img src="{{ site.baseurl }}{{ page.image_path }}/mr_chain_progress_05.png" style="max-height: min(200px, 95vh)">


#### Mrs Chain T Special 3 Materials

<img src="{{ site.baseurl }}{{ page.image_path }}/mrs_chain_t_special_in_process_01_tri_material.png" style="max-height: min(200px, 95vh)">


#### Mrs Chain T Special Tweaked Solidfy Modifier

<img src="{{ site.baseurl }}{{ page.image_path }}/mrs_chain_t_special_in_process_02_solidify_modifier.png" style="max-height: min(200px, 95vh)">


#### Mrs Chain T Special Cute Bow

<img src="{{ site.baseurl }}{{ page.image_path }}/mrs_chain_t_special_in_process_03_bow.png" style="max-height: min(200px, 95vh)">


### Interactive Models

#### Mr Stick Version 2

{% assign path = site.baseurl | append: page.model_path | append: "/mr_stick_v1_0.glb" %}
{% include 3d_model.html model=path %}


#### Mr Chain

<canvas class="model_canvas" id="mr_chain">
{% assign path = site.baseurl | append: page.model_path | append: "/mr_chain_v0_1.glb" %}
{% include 3d_model.html model=path canvas_id="mr_chain" ignore_canvas="Yes" is_secondary="Yes" %}
