---
title: Maya Animation
subtitle: 
layout: exercise
submission-id: animation-YOURSTUDENTID
asset-path: /assets/exercise-images
---

In this exercise, you will practice keyframing, animating the camera, and creating deformers. Level 1 students will create a simple demonstration of basic animation and camera movement. Level 2 and 3 students will create an animation inspired by tetris.

## Learning Resources

### Tutorials: Levels 1, 2, and 3

**Animation Tools**  
Lynda Tutorials: [Maya 2017 Essential Training: Animate in Maya](https://www.lynda.com/Maya-tutorials/Understanding-animation-interface/432363/514813-4.html?org=psu.edu)  

### Tutorials: Levels 2 and 3

**Principles of Animation**  
Lynda: [12 Principles of Animation](https://www.lynda.com/3ds-Max-tutorials/12-Principles-Animation-CG-Animators/474685-2.html?org=psu.edu)  

## Steps to Completion

Choose a either level 1, level 2, or level 3 to complete based on your prior experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.

[Level 1 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Watch the animation tutorials from Lynda and Digital Tutors.
2. Create a new project folder called **_{{ page.submission-id }}-L1_**, set your scene to the project folder, and create the sub folders by choosing **_File_** → **_Project Window_** → **_Accept_**.
3. Create an animation with the following:
   - The duration of the animation should be 600 frames.  
   ![image alt text]({{ site.baseurl }}{{ page.asset-path }}/maya-animation-0.jpg)
   - Create a centered cube parented to **_group1_** in the Outliner. 
   - Create a sphere parented to **_group1_** in the Outliner. It should be at least 10 units away from the cube, and revolve concentrically around the cube. (HINT: Their [pivot points](https://vimeo.com/24713801) should be the same location)
   - Animate **pSphere1** to rotate concentrically in the y-axis around the **pCube1**, twice(720 degrees).
   - Animate the **group1** to move from 0 to positive 20 units in the y-axis direction from frame 0 to 300, and move back to the origin from frame 300 to 600. (The sphere should follow the cube as it moves up and down because they are both in **_group1_**.)
   - Create a perspective camera slightly above and looking at the cube. Include **_persp1_** within **group1** so that it can follow the cube as it moves up and down.  
   ![image alt text]({{ site.baseurl }}{{ page.asset-path }}/maya-animation-1.jpg)  
   - Go into the Graph Editor and make your **pSphere1** rotation tangents linear.  
   ![image alt text]({{ site.baseurl }}{{ page.asset-path }}/maya-animation-2.png)  
   ![image alt text]({{ site.baseurl }}{{ page.asset-path }}/maya-animation-3.png)  
   - Your sphere should now loop seamlessly with the beginning of the animation. 
4. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
5. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L1.zip._**
6. Upload the .zip file to the submission dropbox.
7. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 1_ folder structure**

```

{{ page.submission-id }}-L1.zip
|
└── {{ page.submission-id }}-L1
    |
    ├── sound/
    ├── scripts/
    ├── scenes/
    |   |
    |   └── {{ page.submission-id }}.mb
    |
    ├── renderData/
    ├── particles/
    ├── movies/
    ├── images/
    ├── data/
    ├── clips/
    ├── cache/
    ├── autosave/
    └── assets/

```

### <a name="level-2"></a>Level 2:

1. Watch the animation tutorials from Lynda and Digital Tutors.
2. Create a new project folder called **_{{ page.submission-id }}-L2_**, set your scene to the project folder, and create the sub folders by choosing **_File_** → **_Project Window_** → **_Accept_**.
3. Create an animated scene inspired by [Tetris](http://www.youtube.com/watch?v=qIAAmaS9n0Q). It must include the following:
   - At least 8 moving pieces
   - Camera movement
   - Easing applied to keyframes of moving objects (non-linear tangents in graph editor)
   - Camera shake
   - At least 10 seconds of animation at 24 frames per second (240 frames)
4. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
5. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L2.zip._**
6. Upload the .zip file to the submission dropbox.
7. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 2_ folder structure**

```

{{ page.submission-id }}-L2.zip
|
└── {{ page.submission-id }}-L2
    |
    ├── sound/
    ├── scripts/
    ├── scenes/
    |   |
    |   └── {{ page.submission-id }}.mb
    |
    ├── renderData/
    ├── particles/
    ├── movies/
    ├── images/
    ├── data/
    ├── clips/
    ├── cache/
    ├── autosave/
    └── assets/

```

### <a name="level-3"></a>Level 3:

1. Watch the animation tutorials from Lynda and Digital Tutors.
2. Create a new project folder called **_{{ page.submission-id }}-L3_**, set your scene to the project folder, and create the sub folders by choosing **_File_** → **_Project Window_** → **_Accept_**.
3. Create a creature animation using only primitives inspired by [Evolved Virtual Creatures](http://www.youtube.com/watch?v=JBgG_VSP7f8). It must include the following:
   - At least 2 creatures with 3 moving pieces appendages
   - Camera movement
   - Easing applied to keyframes of moving objects (non-linear tangents in graph editor)
   - Camera shake
   - At least 10 seconds of animation at 24 frames per second (240 frames)
4. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
5. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L3.zip._**
6. Upload the .zip file to the submission dropbox.
7. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 3_ folder structure**

```

{{ page.submission-id }}-L3.zip
|
└── {{ page.submission-id }}-L3
    |
    ├── sound/
    ├── scripts/
    ├── scenes/
    |   |
    |   └── {{ page.submission-id }}.mb
    |
    ├── renderData/
    ├── particles/
    ├── movies/
    ├── images/
    ├── data/
    ├── clips/
    ├── cache/
    ├── autosave/
    └── assets/

```

* * *

## Grading
Your grade will be assessed according to the [Exercise Grading Criteria]({{ site.baseurl }}/grading). 