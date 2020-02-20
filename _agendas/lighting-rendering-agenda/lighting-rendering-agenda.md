---
layout: post
title: Camera, Lighting, and Rendering
categories: agenda
comments: false
published: true
excerpt: Introduction to lighting and rendering
---

### Agenda

1. **Video Screening**
  - ["Spectacle, Speculation, Spam"](https://vimeo.com/194963450) by Alan Warburton
2. Reading
  - [FX Guide: "Art of Rendering"](https://www.fxguide.com/fxfeatured/the-state-of-rendering/)
3. **Terminology**
  - Light types: Area, Spot, Directional or Sun, Point, Volumetric
  - Lighting setups
    - [3 point lighting](https://m5designstudio.com/2011/maya-3d-tutorials/studio-three-point-lighting/) (key, fill, rim)
    - Geometry-based lighting using Emission shader
    - Geometry-based lighting using [Principled Volumetric shader](https://www.youtube.com/watch?v=AXjE-t6dFZ8)
    - Staging lights: Light box with side and top lights, curved color background and floor
    - Image based lighting (IBL) [using HDR images](https://area.autodesk.com/tutorials/studio-lighting/)
      - Shadows: The larger the light source, the softer the shadows
      - Create edge bevels to capture highlights on hard surfaces
  - Camera
    - Perspective vs Orthographic
    - Sensor size
    - Depth of field using aperture F-Stop: Shallow depth of field is created with lower settings. (In Blender, very low settings may be needed such as 0.1)
    - Blades add flat sides to the Bokeh
    - You can create custom [Bokeh shapes](https://blender.stackexchange.com/questions/133191/custom-bokeh-shapes)
    - Safe area
    - Composition guides for layouts (golden ratio, golden tringle, thirds, etc.)
  - Render quality in Cycles
    - To redue render times, keep material shaders simple. Use principled shader if working with photoreal renders.
    - 500 samples are usually needed to reduce noise.
    - Use [advanced denoising workflow](https://www.youtube.com/watch?v=Pw-OxOHHu5I) in the compositor
    - If using motion blur or depth of field, sample sizes must inrease dramatically.
    - You can get away with 120 samples if you use denoising in the Compositor 
  - Render quality in EEVEE
    - [EEVEE Lighting](https://www.youtube.com/watch?v=MFNurQ1AF2I)
    - Enable render settings including: Ambient Occlusion, Depth of Field, and Screen Space Reflections
    - Shadows: Increase the shadow map to 4K
4. **Lighting and Rendering Demo**