---
title: Animation with Blender
subtitle: 
layout: exercise
submission-id: animation-YOURSTUDENTID
asset-path: /assets/exercise-images
exercise: exercise-5
---
![cube and sphere in blender 3d]({{ site.baseurl }}{{ page.asset-path }}/blender-animation-intro.png)
In this exercise, level 1 students will practice keyframing, parenting, animating the camera with a target, and manipulating curves in the graph editor. Level 2 and 3 students will create advanced animations based on the requirements listed in the instructions.

## Learning Resources

- [12 Principles of Animation](https://www.youtube.com/playlist?list=PL-bOh8btec4CXd2ya1NmSKpi92U_l6ZJd)
- Blender Foundatiomn Training: [Videos 38-41](https://www.youtube.com/watch?v=SZJswvw9wEs&list=PLa1F2ddGya_-UvuAqHAksYnB0qL9yWDO6&index=39&t=0s)  
- [Create camera tracking target](https://www.youtube.com/watch?v=ageV_llb0Hk)
- [Parenting](https://en.wikibooks.org/wiki/Blender_3D:_Noob_to_Pro/Parenting)
- [Youtube: Parenting in Blender 2.8](https://www.youtube.com/watch?v=kd1O0oqQ3Uw)
- [Set Pivot Point](https://www.versluis.com/2016/05/how-to-set-the-origin-pivot-point-in-blender/)
- [Camera aim constraint](https://www.youtube.com/watch?v=ktqeSrj4e8Q)

## Steps to Completion

Choose a either level 1, level 2, or level 3 to complete based on your prior experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.

[Level 1 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Watch the animation tutorials.
2. Create an animation in Blender with the following:
   - The duration of the animation should be 120 frames.
   - Create a centered cube. 
   - Create a sphere [parented](https://www.youtube.com/watch?v=kd1O0oqQ3Uw) to the cube. The sphere should be 5 units away from the cube in the X or Y axis, and revolve concentrically around the cube. (HINT: Their [pivot points](https://www.versluis.com/2016/05/how-to-set-the-origin-pivot-point-in-blender/) should be the same location: 0,0,0)
   - Animate the sphere to rotate concentrically around the cube, twice(720 degrees).
   - Go into the Graph Editor and set **interpolation mode** to **linear**.
   - Your sphere should now loop seamlessly with linear motion. Press play in the timeline to see if it is looping seamlessly. The sphere should not be stopping at any point.
   - Animate the cube to move from 0 to positive 10 units in the z-axis from frame 1 to 60, and move back to the origin from frame 61 to 120. (The sphere will follow the cube as it moves up and down if it parented correctly)
   - Create a new perspective camera.
   - Create an 'empty' and use it at as a [camera tracking constraint](https://www.youtube.com/watch?v=ageV_llb0Hk).
   - Parent the 'empty' to the cube so the camera aims at the cube as it moves up and down.
   - Select the camera and choose **View** ⟶ **Camera** ⟶ **Set active object as camera** and choose "Lock Camera to viewport .
3. Save as **_{{ page.submission-id }}-L1.blend_** and upload to the submission dropbox.
6. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

### <a name="level-2"></a>Level 2:

1. Watch the animation tutorials.
2. Create an animated scene inspired by [Tetris](http://www.youtube.com/watch?v=qIAAmaS9n0Q). It must include the following:
   - At least 8 moving pieces
   - Camera movement
   - Easing applied to keyframes of moving objects (non-linear tangents in graph editor)
   - Camera shake
   - At least 10 seconds of animation at 24 frames per second (240 frames)
3. Save as **_{{ page.submission-id }}-L2.blend_** and upload to the submission dropbox.
7. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

### <a name="level-3"></a>Level 3:

1. Watch the animation tutorials.
2. Create a creature animation using only primitives inspired by [Evolved Virtual Creatures](http://www.youtube.com/watch?v=JBgG_VSP7f8). It must include the following:
   - At least 2 creatures with 3 moving pieces appendages
   - Camera movement
   - Easing applied to keyframes of moving objects (non-linear tangents in graph editor)
   - Camera shake
   - At least 10 seconds of animation at 24 frames per second (240 frames)
3. Save as **_{{ page.submission-id }}-L3.blend_** and upload to the submission dropbox.
4. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

* * *

## Grading
Your grade will be assessed according to the [Exercise Grading Criteria]({{ site.baseurl }}/grading). 