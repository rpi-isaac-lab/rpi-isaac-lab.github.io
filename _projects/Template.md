---
layout: page
title: Template
description: "Lead Researcher: Researcher_Name"
img: assets/img/carla.png
importance: 1
category: current
related_publications: true
---

Come up with some info about your project. Make sure to fill out the info at the top of the file including "title", the lead researcher's name, "img", "category", and "related_publications". Specifically, the category should be one of: ["current","past"], and related_publications should be one of: ["true","false"], depending on whether or not you will be referencing papers in the bibliography.

## Here is a link

[link](https:/google.com)

## Here is an image

![carla_image](/assets/img/carla.png)

## Here is an embedded youtube video

{% include video.liquid path="https://www.youtube.com/embed/W6ZOeesjFHM?si=bzFPxjbYewp5I3I5" class="img-fluid rounded z-depth-1" width="100%" height="100%" %}

Here, you'll want to exchange the path for your new path.

## Here is a locally hosted video

{% include video.liquid path="/assets/video/carla_demo.webm" class="img-fluid rounded z-depth-1" width="100%" height="100%" autoplay=true caption="Fig 1: Video of the CARLA simulation platform, currently under development for use in human-in-the-loop testing." loop=true controls=true %}

Here, you'll want to exchange the path for your new path and the caption for you own.

## Citations

Cite papers from the bibliography like this: {% cite paper_cite_key %}. In order to cite papers, the "related_publications" key in the top section of this file should be set to "true"
