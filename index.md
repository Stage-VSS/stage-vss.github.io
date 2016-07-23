---
layout: default
title: Home
---

<img src="public/images/logo.png" srcset="public/images/logo.png 1x, public/images/logo@2x.png 2x" alt="Stage Logo">

<h1>Simple, Powerful, Flexible<br>
OpenGL Visual Stimuli in MATLAB&reg;</h1>

<a href="{{ site.github.repo }}/releases/download/{{ site.version }}/Stage.mltbx" class="btn">Download</a>
<a href="{{ site.github.repo }}" class="btn">GitHub</a>

<hr>

## What is Stage?
Stage is a MATLAB based visual stimulus system for vision research. It provides a toolbox for writing visual stimulus routines.

![hero](public/images/hero.png)

<hr>

## Built-in Stimuli
Stage comes with a wide variety of built-in stimuli. You can layer stimuli and animate their attributes (position, size, orientation, color, opacity, etc.) to create complex presentations.

<div class="features">
  {% for stimulus in site.stimuli %}
  <div class="feature">
    <h3>{{ stimulus.title }}</h3>

    <div class="gfyitem" data-title="false" data-autoplay="false" data-controls="false" data-expand="false" data-id="{{ stimulus.gfyitem }}"></div>

    <p><label class="btn collapse-toggle">View Code</label></p>
    <div class="collapse">
      <script src="https://gist.github.com/{{ stimulus.gist }}.js"></script>
    </div>
  </div>
  {% endfor %}
</div>

<hr>

## Masks and Filters
Stage supports real-time transparency masks and convolution filters. The use of shaders enable all effects processing to occur on the GPU.

<div class="features">
  {% for effect in site.effects %}
  <div class="feature">
    <h3>{{ effect.title }}</h3>

    <div class="gfyitem" data-title="false" data-autoplay="false" data-controls="false" data-expand="false" data-id="{{ effect.gfyitem }}"></div>

    <p><label class="btn collapse-toggle">View Code</label></p>
    <div class="collapse">
      <script src="https://gist.github.com/{{ effect.gist }}.js"></script>
    </div>
  </div>
  {% endfor %}
</div>

<hr>

## Stage Server
Stage includes a Stage Server app to enable remote stimulus presentation across MATLAB sessions. The sessions may be running on the same machine or on separate machines across a network.

![server](public/images/server.png)

<hr>

## Symphony Integration
Stage integrates seamlessly with [Symphony](http://symphony-das.github.io). You can create and display Stage presentations directly in your Symphony protocols.

![symphony](public/images/symphony.png)

<p><label class="btn collapse-toggle">View an Example Protocol</label></p>
<div class="collapse">
  <script src="https://gist.github.com/cafarm/4ede658fd504a979b511f62092614441.js"></script>
</div>

<hr>

## Built for Modern OpenGL
Stage was built for core OpenGL 3.2+ which enables it to be more efficient, flexible, and future-proof. The toolbox makes extensive use of vertex buffer and array objects as well as shaders.

<img src="public/images/opengl.png" srcset="public/images/opengl.png 1x, public/images/opengl@2x.png 2x" alt="OpenGL Logo">

<hr>

## Free and Open Source
Stage is released under the [MIT License](https://opensource.org/licenses/MIT), which is an [open source license](https://opensource.org/docs/osd). You can share and change the source code to your heart's content!

<img src="public/images/osi.png" srcset="public/images/osi.png 1x, public/images/osi@2x.png 2x" alt="OSI Logo">

<hr>

&copy; {{ site.time | date: '%Y' }} Stage-VSS. MATLAB is a registered trademark of The MathWorks, Inc. OpenGL and the oval logo are trademarks or registered trademarks of Silicon Graphics, Inc. in the United States and/or other countries worldwide. The OSI logo trademark is the trademark of Open Source Initiative.
