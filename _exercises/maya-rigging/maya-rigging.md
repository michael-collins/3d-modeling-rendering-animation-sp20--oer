---
title: Maya Rigging
subtitle: 
layout: exercise
submission-id: maya-rigging-YOURSTUDENTID
assignment-dropbox: https://psu.box.com/signup/collablink/d_6058207793/17af152633c7b9
asset-path: /assets/exercise-images
---

In this exercise, you will practice creating a rig for a polygon mesh and adding deformers. Level 1 students will create a simple biped rig starting with [this project file](https://drive.google.com/file/d/0BzXX6rmROMNWOEFkZ2hjZnJORU0/view?usp=sharing). Level 2 and 3 students will create more complex polygonal biped character meshes and rigs.


## Learning Resources:

**Level 1: Novice Students**

Lynda.com: [Animation Tools](http://www.lynda.com/Maya-tutorials/Maya-Essentials-5-Animation-Tools/96719-2.html)

Lynda.com: [Cartoon Rigging](https://www.lynda.com/Maya-tutorials/Rigging-Cartoon-Character-Maya/191956-2.html?org=psu.edu)

**Levels 2 and 3: Intermediate & Experienced Students**

Lynda.com: [Character Rigging](https://www.lynda.com/Maya-tutorials/Character-Rigging-in-Maya/92564-2.html?org=psu.edu)  

**Levels 3: Experienced Students**  
[Face rigging](https://www.lynda.com/Maya-tutorials/Facial-Rigging-Maya/149842-2.html?org=psu.edu)

Lynda Tutorials: [12 Principles of Animation](https://www.lynda.com/3ds-Max-tutorials/12-Principles-Animation-CG-Animators/474685-2.html?org=psu.edu)

## Steps to Completion

Choose a either level 1, level 2, or level 3 to complete based on your prior experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.

[Level 1 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Watch the level 1 rigging tutorials.
2. Download the base Maya [rigging project folder](https://drive.google.com/file/d/0BzXX6rmROMNWOEFkZ2hjZnJORU0/view?usp=sharing).
3. Rename the downloaded project folder to: **_{{ page.submission-id }}-L1_**
4. Set your project to the downloaded folder.
5. Add subdivisions (edge loops) to the polygonal mesh minimizing unwanted distortion that results from moving a joints bound to improperly created geometry. Add geometry to articulate the knee, elbows, and arms.
6. Create joints for the torso, hips, knees, legs, feet, shoulders, arms, neck, and head. Name and number them for your reference. See image below:
![image alt text]({{ site.baseurl }}{{ page.asset-path }}/maya-rigging-1.jpg)
7. Smooth bind the joints to the polygonal mesh by selecting both the mesh and the joints, and then choosing, *Skin* → *Bind*. Click on ‘Smooth Bind.’
8. Use the Component Editor and Paint Skin Weights tool to make adjustments to joint influences.
9. Pose the biped to be in natural sitting pose.
10. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
11. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L1.zip._**
12. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
13. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 1_ folder structure**

```

{{ page.submission-id }}-L1.zip
|
└── {{ page.submission-id }}-L1
    |
    ├── sourceimages/
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

1. Watch the level 2 cartoon character animation tutorials.
2. Create a new project folder called **_{{ page.submission-id }}-L2_**, set your scene to the project folder, and create the sub folders by choosing **_File_** → **_Project Window_** → **_Accept_**.
3. Build a simple biped character mesh.
4. Create joints, IKs, and controls for the head, arms, and legs.
5. Bind your rig to your mesh.
6. Create a text animation of your character’s movement, showing the versatility of your rig over 120 frames.
7. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
8. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L2.zip._**
9. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
10. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 2_ folder structure**

```

{{ page.submission-id }}-L2.zip
|
└── {{ page.submission-id }}-L2
    |
    ├── sourceimages/
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

1. Watch the tutorials from the learning resources.
2. Create a new project folder called **_{{ page.submission-id }}-L3_**, set your scene to the project folder, and create the sub folders by choosing **_File_** → **_Project Window_** → **_Accept_**.
3. Create a fully rigged character including a center of gravity control, limb and body part controls, rotation constraints, and set-driven keys.
4. Create a 10 second 240 frame animation expressing one of the 12 animation principles.
5. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
6. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L3.zip._**
7. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
8. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 3_ folder structure**

```

{{ page.submission-id }}-L3.zip
|
└── {{ page.submission-id }}-L3
    |
    ├── sourceimages/
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

