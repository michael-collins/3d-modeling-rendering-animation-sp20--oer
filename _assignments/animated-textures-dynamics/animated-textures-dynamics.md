---
title: Animated Textures and Dynamics in Blender
layout: exercise
submission-id: anim-textures-YOURNAME
asset-path: /assets/exercise-downloads
exercise: exercise-7
asset-path: /assets/exercise-images
download-path: /assets/exercise-downloads
---

In this exercise, you will apply an image sequence as texture object in Blender, create dynamics, render a final Blender animation as an image sequence, and import it into after effects. You will create a compressed video in a web streaming format called H.264.

## Learning Resources

Example animated texture project download (Large ~200MB file): [face-texture-anim.zip](https://drive.google.com/open?id=10RnUpvyXGJWKltiRsUtpNE67k3tiGjhB)

### Tutorials:

**Rigid Body Dynamics**

* [Rigid Body with Animated Sphere](https://www.youtube.com/watch?v=Xj1QoznVUwc)
* [Blender Tutorial - Quick Rigid Body Fun](https://www.youtube.com/watch?v=nHVYYMG3QVY)
* [Simple Gravity animation](https://www.youtube.com/watch?v=-4uFt0m5I-U)

**Rendering an animated image sequence from Blender** 

[Blender 2.8 Tutorial\: Rendering an Animation](https://www.youtube.com/watch?v=LPbUuMs2i20)

**Transparency**

[Blender 2.8 Tutorial \| Alpha Transparency in the EEVEE engine](https://www.youtube.com/watch?v=lFWiU0a5CiQ)

**Importing and Exporting**

[Exporting compressed video from After Effects for Vimeo](https://vimeo.com/301944187)

***

## Steps to Completion

1. Watch the level tutorials. If you are confused, please see
2. Create and set a project folder called **_{{ page.submission-id }}_** save your .blend file in the project folder.
4. Create an anmiation with the following:
  * EEVEE render engine (Cycles is fine, but takes too long to render for this exercise)
  * Rigid body (active) – Two or more objects
  * Rigid body (passive) – At least one static object (can be the floor plane object)
  * One object with an animated texture
  * At least 1 second (24 frames of animation)
5. Render your animation as an image sequence (not a video file) to a folder.
6. Following the video importing and exporting tutorials. Import your image sequence to After Effects --> Interpret Footage --> Main and change the framerate to 24FPS. 
7. Export an H.264 MP4 movie file with the Vimeo preset. \(It should be well under 1MB in total file size\). \(See tutorials\).
8. Save your animation file as **_{{ page.submission-id }}_.mp4.
9. Save your blender file as **_{{ page.submission-id }}_.blend**.
10. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}.zip._**
11. Upload only the blend file and H.264 file. Upload the .zip file to the submission dropbox.
12. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

* * *

## Grading
Your grade will be assessed according to the [Exercise Grading Criteria]({{ site.baseurl }}/grading).
