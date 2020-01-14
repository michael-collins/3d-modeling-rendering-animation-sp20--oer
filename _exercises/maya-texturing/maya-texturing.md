---
title: Maya Texturing
subtitle: 
layout: exercise
submission-id: texturing-YOURSTUDENTID
assignment-dropbox: https://psu.box.com/signup/collablink/d_6058204921/115199876a709b
asset-path: /assets/exercise-images
---

 In this exercise, you will practice UV mapping and applying textures to surface shaders. There are different tutorials and exercise submission requirements for three experience levels. Choose the experience level that matches your own.

## Learning Resources

**Level 1: Novice Students**  
[Lynda.com - Textures and Materials](http://www.lynda.com/Maya-tutorials/Maya-Essentials-4-Creating-Textures-Materials/96717-2.html)

**Level 2: Intermediate Students**  
[Digital Tutors - UV Mapping](http://www.digitaltutors.com/11/training.php?vid=9346&autoplay=1)  
[Digital Tutors - AO Texture Baking](http://www.digitaltutors.com/11/training.php?vid=9348&autoplay=1)  
[Tutorial - AO](https://www.youtube.com/watch?v=v3SXSffuvnk)  
[Digital Tutors - Diffuse texture workflow](http://www.digitaltutors.com/11/training.php?vid=9350&autoplay=1)  

**Level 3: Experienced Students**  
[Lynda.com - ZBrush Essential Training](http://www.lynda.com/ZBrush-4-tutorials/Essential-Training/76980-2.html) (Lessons 7 - 10)  
[Lynda.com - ZBrush Character](http://www.lynda.com/3D-Animation-Character-Design-tutorials/Digital-Creature-Creation-in-ZBrush-Photoshop-and-Maya/83781-2.html) (Lessons 6 - 9)

## Steps to Completion

**Choose a single level to complete based on your level of experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.**

[Level 1 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Watch tutorials from Lynda on modeling with Polygons and Nurbs.
2. Create a new project folder called **_{{ page.submission-id }}-L1_***.*
3. Set your project to the downloaded folder by choosing **File** → **Set Project**.
4. Create your folder structure by choosing **File** → **Project Window → ****_Accept_**.
5. Build a spaceship using no more than 150 tris. Example: [Low Poly Spaceship](https://sketchfab.com/models/0254f0be6e3142ec942428aa59370d6d)
6. Go to **Create UVs** and choose an appropriate mapping tool.
7. Organize your UV layout with the **UV Texture Editor **tool.
8. Export your UV layout from the **UV Texture Editor → Polygons → ****UV Snapshot** with a resolution of 1024px by 1024px to the *sourceimages* folder as **_uv-{{ page.submission-id }}.jpg_**.
9. Open the UV layout image into Photoshop. Paint a **color** texture using the UV snapshot as a guide.
10. Save your color texture as **_color-{{ page.submission-id }}.jpg_** in the *sourceimages* folder.
11. Use Photoshop to create a grayscale bump map texture (1024px by 1024px) using the color texture and UV snapshot as a guide.
12. Save your bump map texture as **_bump-{{ page.submission-id }}.jpg_** in the *sourceimages* folder.
13. Apply your color and bump textures to your model’s Lambert shader on the Color and Bump Mapping channels respectively. If you can’t see your textures, ensure that the viewport’s **View → Hardware Texturing** feature is enabled. Click on render to check that the bump map is functioning properly.
14. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
15. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L1.zip._**
16. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
17. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 1_ folder structure**

```

{{ page.submission-id }}-L1.zip
|
└── {{ page.submission-id }}-L1
    |
    ├── sourceimages/
    |   |
    |   ├── color-{{ page.submission-id }}.jpg
    |   ├── uv-{{ page.submission-id }}.jpg
    |   └── bump-{{ page.submission-id }}.jpg
    |   
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

1. Duplicate your project folder from Exercise 2 and rename it to **_{{ page.submission-id }}-L2_**.
2. For each of the three objects you modeled in the last exercise:
  a. Unwrap the object’s UVs
  b. Export a UV snapshot
  c. Bake an Ambient Occlusion (AO) texture *(*[Tutorial - AO](https://www.youtube.com/watch?v=v3SXSffuvnk)*, *[Digital Tutors - AO Texture Baking](http://www.digitaltutors.com/11/training.php?vid=9348&autoplay=1)*)*
  d. Create a color texture in Photoshop (1024px by 1024px) and overlay the AO shadow image into the color texture.
3. Save each of the three scenes in the scenes folder as:  
  **_obj1-{{ page.submission-id }}_**  
  **_obj2-{{ page.submission-id }}_**  
  **_obj3-{{ page.submission-id }}_**  
4. Save your UV snapshots in the sourceimages folder as:  
  **_uv1-{{ page.submission-id }}.jpg_**  
  **_uv2-{{ page.submission-id }}.jpg_**  
  **_uv3-{{ page.submission-id }}.jpg_**  
5. Save your color textures combined with AO texture in the sourceimages folder as:  
  **_color1-{{ page.submission-id }}.jpg_**  
  **_color2-{{ page.submission-id }}.jpg_**  
  **_color3-{{ page.submission-id }}.jpg_**  
6. Save your AO textures in the sourceimages folder as:  
  **_ao1-{{ page.submission-id }}.jpg_**  
  **_ao2-{{ page.submission-id }}.jpg_**  
  **_ao3-{{ page.submission-id }}.jpg_**  
7. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L2.zip._**
8. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
9. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 2_ folder structure**

```

{{ page.submission-id }}-L2.zip
|
└── {{ page.submission-id }}-L2
    |
    ├── sourceimages/
    |   |
    |   ├── uv1-{{ page.submission-id }}.jpg
	|   ├── uv2-{{ page.submission-id }}.jpg
    |   ├── uv3-{{ page.submission-id }}.jpg
    |   ├── color1-{{ page.submission-id }}.jpg
    |   ├── color2-{{ page.submission-id }}.jpg
    |   ├── color3-{{ page.submission-id }}.jpg
    |   ├── ao1-{{ page.submission-id }}.jpg
    |   ├── ao2-{{ page.submission-id }}.jpg
    |   └── ao3-{{ page.submission-id }}.jpg
    |
    ├── sound/
    ├── scripts/
    ├── scenes/
    |   |
    |   ├── obj1-{{ page.submission-id }}.mb
    |   ├── obj2-{{ page.submission-id }}.mb
    |   └── obj3-{{ page.submission-id }}.mb
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

1. Watch the Essential Training and Digital Character Creation tutorials from Lynda on modeling with ZBrush.
2. Using the techniques learned in the Digital Creature Creation tutorials, continue working on your model from the Maya Modeling Exercise.
3. Create the textures covered in the Digital Character Creation tutorials.
4. Import your model into Maya and connect the textures to the creature’s shader.
5. Save your scene as **_{{ page.submission-id }}-L3_** in the scenes folder.
6. Save your PSD texture in the *sourceimages* folder as **_{{ page.submission-id }}-L3.psd_**. ([See Organizing the maps into Photoshop layers](http://www.lynda.com/3D-Animation-Character-Design-tutorials/Digital-Creature-Creation-in-ZBrush-Photoshop-and-Maya/83781-2.html) on Lynda.com)
7. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L3.zip._**
8. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
9. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 3_ folder structure**

```

{{ page.submission-id }}-L3.zip
|
└── {{ page.submission-id }}-L3
    |
    ├── sourceimages/
    |   |
    |   ├── {{ page.submission-id }}.jpg
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