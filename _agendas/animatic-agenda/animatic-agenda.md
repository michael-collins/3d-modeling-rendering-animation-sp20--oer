---
layout: post
title: Editing Animatics – Camera shots and animating to sound
categories: agenda
comments: false
published: true
excerpt:
---

### Agenda

1. Framing and composition theory for film
  - [Studiobinder.com](https://www.studiobinder.com/blog/rules-of-shot-composition-in-film/)
1. Tutorials
  - [Blender 2.8 Tutorial: Viewport Render Animation \( make preview \)](https://www.youtube.com/watch?v=QuVZGDbly3g)
  - If you need to do precise animation timing: [Import audio into Blender](https://www.youtube.com/watch?v=9w-6Lk1OJbg)
  - [Cutting Between Multiple Cameras - Blender Tutorial](https://www.youtube.com/watch?v=93bBtxuf9Dg)
2. **Terminology**
  - Film blocking (Space, shapes, lines)
  - Eye level framnig
  - Leading lines (drawing our eyes to the focal point)
  - Depth of field, focal point, and rack focus
  - Deep space composition
  - Add Camera
  - Blender Editor: Timeline
  - Blender Editor: Video sequencer
    - Add --> Sound
  - Blender Editor: Graph Editor
  - Editor Menu Item: Marker
    - Add Marker
    - Bind Camera to Marker (binds the selected camera to the marker position)
  - Sequence render animation
3. Demo
  - Camera
     - Set up camera shots (framing and composition, animation)
     - Add markers and attach cameras
  - If your animation must be precisely synced with audio, import audio into blender
     - [Audio import tutorial](https://www.youtube.com/watch?v=qjSSiltPMyk)
  - Rendering animation preview videos
     - [Make preview tutorial](https://www.youtube.com/watch?v=QuVZGDbly3g)
    **Output Properties** –> configure frame start and end each time to render a viewport animation.
     - **Output Properties** –> Configure output directory
     - Framerate set to 24fps
     - Instead of PNG, choose FFMPEG, encoding video codec to H.264, container to MP4, and High Quality, no audio.
     - In **Output Properties** –> **Metadata**, Check the **Burn into Image** setting. Increase font size to 24 and adjust color as needed.
  - Importing into after effects
     - Import animation video files into the project area.
     - Import audio
     - [Freesound.org](https://freesound.org)
     - Edit the shots and sound
     - Sound conversion: [Audacity](https://www.audacityteam.org/)
  - Export final video in H.264, vimeo 1080P Preset with Media Encoder
