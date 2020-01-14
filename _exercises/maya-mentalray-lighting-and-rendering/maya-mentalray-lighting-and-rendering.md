---
title: Maya Mentalray Lighting and Rendering
subtitle: 
layout: exercise
submission-id: mr-rendering-YOURSTUDENTID
assignment-dropbox: https://psu.box.com/signup/collablink/d_6058205621/11e086038985f5
asset-path: /assets/exercise-images
---

In this exercise, you will practice uv mapping, lighting, and rendering. There are different tutorials and exercise submission requirements for three experience levels. Choose the experience level that matches your own.

![image alt text]({{ site.baseurl }}{{ page.asset-path }}/maya-mentalray-lighting-and-rendering-0.png)


# Learning Resources

## Tutorials:

**Level 1: Novice Students**  
[Lynda.com - Essential Training](http://www.lynda.com/Maya-tutorials/Maya-2016-Essential-Training)
[Lynda.com - Lights and Rendering](http://www.lynda.com/Maya-tutorials/Render-Settings-menu/370380/413273-4.html)  
[Digital Tutors: Building a Backdrop](http://www.digitaltutors.com/lesson/5996-Building-a-backdrop-for-studio-lighting)

**Level 2: Intermediate Students**  
[Lynda Tutorials - Creating Textures and Shaders](http://www.lynda.com/Maya-2011-tutorials/creating-textures-and-shaders/62904-2.html)  
[Lynda Tutorials - Lighting and Rendering in Mental Ray](http://www.lynda.com/Maya-2011-tutorials/lighting-and-rendering-in-mental-ray/61222-2.html)  
[Digital Tutors: Building a Backdrop](http://www.digitaltutors.com/lesson/5996-Building-a-backdrop-for-studio-lighting)
[Color Management in Maya 2016](https://www.youtube.com/watch?v=uUmq8q23wJ8)

**Level 3: Experienced Students**  
[Lynda.com - ZBrush Essential Training](http://www.lynda.com/ZBrush-4-tutorials/Essential-Training/76980-2.html)
[Lynda.com - ZBrush Character](http://www.lynda.com/3D-Animation-Character-Design-tutorials/Digital-Creature-Creation-in-ZBrush-Photoshop-and-Maya/83781-2.html)

**Website References**

Chair History:** **[Random History](http://www.randomhistory.com/2008/11/11_chair.html)  
3 Point Lighting: [5M Design Studio](http://m5designstudio.com/2011/maya-3d-tutorials/studio-three-point-lighting/)

**More Information:**

Textbook: Introducing Autodesk Maya 2015  
Chapter 10 and 11

Textbook: Mastering Autodesk Maya 2015  
Chapter 9 and 10

## Steps to Completion

**Choose a single level to complete based on your level of experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.**

[Level 1 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Watch tutorials from Lynda on texturing and lighting.
2. Create and set a project folder called **_{{ page.submission-id }}-L1_**.
3. Set your project folder by choosing **File** → **Set Project**.
4. Create your folder structure by choosing **File** → **Project Window** → **_Accept_**.
5. After reading [this webpage](http://www.randomhistory.com/2008/11/11_chair.html), create a new scene and create a hi-res polygon model of a **chair** from one of the mentioned time periods approximately within 4 units wide, high, and deep as well as a patch of ground 10 units wide by 10 units deep by roughly 1 unit high. These can be a single polygonal mesh or modeled as separate objects.
6. Create a new perspective called **_cam1_**. In the camera attributes, change the film gate to **35mm Academy**.
7. In your Cam1 viewport, enable the Resolution Gate: **View** → **Camera** **Settings** → **Resolution** **Gate.**
8. Create a standard 3-point lighting setup with three **_area lights_** and name them **_KeyLight_**, **_FillLight_**, and **_RimLight_**. Read More about [three point lighting](http://m5designstudio.com/2011/maya-3d-tutorials/studio-three-point-lighting/).
9. Unfold your UVs using the UV Texture editor other UV tools.
10. Apply a texture that you’ve created or found online and name it **_color-{{ page.submission-id }}.jpg_** in the *sourceimages* folder.
11. Create and apply a bump map to your Lambert called **_bump-{{ page.submission-id }}.jpg_** in the **sourceimages** folder.
12. Adjust the Bump Depth to **0.200** on the bump2d node connected to your bump map channel.  
  ![image alt text]({{ site.baseurl }}{{ page.asset-path }}/maya-mentalray-lighting-and-rendering-1.jpg)
13. Enable Mental Ray as the rendering engine in the render settings.
14. Match the following render settings:  
  Render using **Mental Ray**  
  **Quality Tab**  
    a. Overall Quality: 3  
    b. Indirect Diffuse (GI) Mode: Finalgather	
  **Common Tab**  
    a. Presets: HD 1080
15.  Position **_Cam1_** so that the object is in the center, filling most of the composition.
16. Render the image from **_Cam1_** and save it as **_render-{{ page.submission-id }}.exr_** in the images folder using OpenEXR format. (Not JPG)
17. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
18. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L1.zip._**
19. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
20. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 1_ folder structure**

```

{{ page.submission-id }}-L1.zip
|
└── {{ page.submission-id }}-L1
    |
    ├── sourceimages/
    |   |
    |   ├── color-{{ page.submission-id }}.jpg
    |   └── bump-{{ page.submission-id }}.jpg
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
    |   |
    |   └── render-{{ page.submission-id }}.exr
    |   
    ├── data/
    ├── clips/
    ├── cache/
    ├── autosave/
    └── assets/

```

### <a name="level-2"></a>Level 2:

1. Watch the Lynda tutorials on lighting and rendering.
2. Duplicate your project folder from the last exercise and rename it to **_{{ page.submission-id }}-L2_***.*
3. Save each of the three scenes in the scenes folder as:  
  **_obj1-{{ page.submission-id }}_**  
  **_obj2-{{ page.submission-id }}_**  
  **_obj3-{{ page.submission-id }}_**  
4. Ensure all of your objects are using a mia_material_x material with your textures. ([introducing the mia_material](http://www.lynda.com/Maya-2011-tutorials/creating-textures-and-shaders/62904-2.html))
5. Compose your objects in their respective scenes
6. Create a new perspective called **_cam1_**. In the camera attributes, change the film gate to **35mm Academy**.
7. In your Cam1 viewport, enable the Resolution Gate: **View** → **Camera** **Settings** → **Resolution** **Gate.**
8. Create a standard 3-point lighting setup with three **_area lights_** and name them **_KeyLight_**, **_FillLight_**, and **_RimLight_**. Read More about [three point lighting](http://m5designstudio.com/2011/maya-3d-tutorials/studio-three-point-lighting/).
9. Create a backdrop for your models [Tutorial](http://www.digitaltutors.com/lesson/5996-Building-a-backdrop-for-studio-lighting) (You may use the same one in each scene by exporting the backdrop as an FBX). 
10. In the material attributes for each material, enable ambient occlusion.
11. Save your color texture maps in the sourceimages folder as:  
  **_color1-{{ page.submission-id }}.jpg_**  
  **_color2-{{ page.submission-id }}.jpg_**  
  **_color3-{{ page.submission-id }}.jpg_**
12. Add surface details with bump maps. Save your bump texture maps in the sourceimages folder as:  
  **_bump1-{{ page.submission-id }}.jpg_**  
  **_bump2-{{ page.submission-id }}.jpg_**  
  **_bump3-{{ page.submission-id }}.jpg_**
13. Enable **_Depth of Field_** on Cam1 and adjust the focus length with the aid of a **_Locator_**.
14. Enable the following render settings:  
  **Quality Tab**  
  a. Overall Quality: 2  
  b. Indirect Diffuse (GI) Mode: Finalgather  
  **Common Tab**  
  a. Presets: HD 1080
15.  Position **_Cam1_** so that the object is in the center, filling most of the composition.
16. Render your three scenes from **_Cam1_** and save them in the images folder using OpenEXR format. (Not JPG)
  **_render1-{{ page.submission-id }}.exr_**  
  **_render2-{{ page.submission-id }}.exr_**  
  **_render3-{{ page.submission-id }}.exr_**
17. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L2.zip._**
18. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
19. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 2_ folder structure**

```

{{ page.submission-id }}-L2.zip
|
└── {{ page.submission-id }}-L2
    |
    ├── sourceimages/
    |   |
    |   ├── bump1-{{ page.submission-id }}.jpg
	|   ├── bump2-{{ page.submission-id }}.jpg
    |   ├── bump3-{{ page.submission-id }}.jpg
    |   ├── color1-{{ page.submission-id }}.jpg
    |   ├── color2-{{ page.submission-id }}.jpg
    |   └── color3-{{ page.submission-id }}.jpg
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
    |   |
    |   ├── render1-{{ page.submission-id }}.exr
    |   ├── render2-{{ page.submission-id }}.exr
    |   └── render3-{{ page.submission-id }}.exr
    |
    ├── data/
    ├── clips/
    ├── cache/
    ├── autosave/
    └── assets/

```

### <a name="level-3"></a>Level 3:

1. Watch the Essential Training and Digital Character Creation tutorials from Lynda on modeling with ZBrush through to the end.
2. Using the techniques learned in the Digital Creature Creation tutorials, continue working on your model.
3. Complete the your image to the level of finish of the tutorial’s final result. Instead of rendering an animated turntable, render four EXR images (Top, Side, Front, 3/4 view) and name them:  
  **_top-{{ page.submission-id }}.exr_**  
  **_side-{{ page.submission-id }}.exr_**  
  **_front-{{ page.submission-id }}.exr_**  
  **_quarter-{{ page.submission-id }}.exr_**  
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
    |   ├── top-{{ page.submission-id }}.exr
    |   ├── side-{{ page.submission-id }}.exr
    |   ├── front-{{ page.submission-id }}.exr
    |   └── quarter-{{ page.submission-id }}.exr
    |   
    ├── data/
    ├── clips/
    ├── cache/
    ├── autosave/
    └── assets/

```

* * *

## Grading
Your grade will be assessed according to the [Exercise Grading Criteria]({{ site.baseurl }}/grading). 
