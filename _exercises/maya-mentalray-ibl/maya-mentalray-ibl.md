---
title: Maya Mentalray IBL
subtitle: 
layout: exercise
submission-id: mr-ibl-YOURSTUDENTID
assignment-dropbox: https://psu.box.com/signup/collablink/d_6058206453/11f0247848da9c
asset-path: /assets/exercise-downloads
---

In this exercise, you will practice uv mapping, lighting, and rendering. There are different tutorials and exercise submission requirements for three experience levels. Choose the experience level that matches your own.

# Learning Resources

## Tutorials:

**Level 1: Novice Students**  
[Image Based Lighting](https://www.youtube.com/watch?v=cKul2-bmBwY)  
[Digital Tutors: Building a Backdrop](http://www.digitaltutors.com/lesson/5996-Building-a-backdrop-for-studio-lighting)  
[Lynda - mia_material_x](http://www.lynda.com/Maya-tutorials/mia-material-X-overview/167357/367262-4.html)

**Level 2: Intermediate Students**  
[Make your own HDR Environment Map](http://cgalter.com/custom-studio-hdr/)  
[MILA Material and Passes:](http://lesterbanks.com/2015/10/mila-render-passes-in-maya-2016-how-to-enable-the-legacy-system/)  
[MILA Material](http://www.digitaltutors.com/tutorial/2284-Building-a-Toy-Plane-for-3D-Printing-in-Maya-and-Mudbox#play-53382)  
[Layering with MILA](https://www.youtube.com/watch?v=_LhQgRiZknE)  
[Ambient Occlusion in MILA](http://forums.autodesk.com/t5/shading-lighting-and-rendering/maya-2016-ambient-occlusion-with-mila/td-p/5740868)  

**Level 3: Experienced Students**  
[Image Based Lighting](https://www.youtube.com/watch?v=cKul2-bmBwY)  
[MILA Material and Passes:](http://lesterbanks.com/2015/10/mila-render-passes-in-maya-2016-how-to-enable-the-legacy-system/)  
[MILA Material](http://www.digitaltutors.com/tutorial/2284-Building-a-Toy-Plane-for-3D-Printing-in-Maya-and-Mudbox#play-53382)  
[Layering with MILA](https://www.youtube.com/watch?v=_LhQgRiZknE)  
[MILA Subsurface Scattering](https://www.youtube.com/watch?v=vU-iL1HnEm0)  
[Ambient Occlusion in MILA](http://forums.autodesk.com/t5/shading-lighting-and-rendering/maya-2016-ambient-occlusion-with-mila/td-p/5740868)  

**Website References**

[Autodesk MIA_Material](http://docs.autodesk.com/MENTALRAY/2013/ENU/mental-ray-help//files/shaders/architectural/arch_mtl.html) 
[Image Based Lighting](https://www.youtube.com/watch?v=cKul2-bmBwY)

**Downloads**  
[EXR Image Pack]({{ site.baseurl }}{{ page.asset-path }}/IBL-pack.zip)

**More Information:**

Textbook: Mastering Autodesk Maya 2016 (Page 355)

## Steps to Completion

**Choose a single level to complete based on your level of experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.**

[Level 1 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Watch tutorials on Image Based Lighting (IBL).
2. Create and set a project folder called **_{{ page.submission-id }}-L1_**.
3. Set your project folder by choosing **File** → **Set Project**.
4. Create your folder structure by choosing **File** → **Project Window** → **_Accept_**.
5. After researching [thrown ceramic mug](https://www.google.com/search?q=ceramic+mug&espv=2&biw=1239&bih=1013&source=lnms&tbm=isch&sa=X&ved=0ahUKEwi7lN_g7MbKAhWktoMKHRoKC1AQ_AUIBygC#tbm=isch&q=thrown+ceramic+mug), create a new scene and create a polygon model of a **thrown ceramic mug**.
6. Create a new perspective called **_cam1_**. In the camera attributes, change the film gate to **35mm Academy**.
7. In your Cam1 viewport, enable the Resolution Gate: **View** → **Camera** **Settings** → **Resolution** **Gate.**
8. Create an Image Based Lighting node and create your own or select an [existing EXR image to use]({{ site.baseurl  }}/exercises/IBL-pack.zip). Name it **_ibl-{{ page.submission-id }}.exr_**
9. Unfold your UVs using the UV Texture editor other UV tools.
10. Assign a new Mentalray material called a **mia_material** to your object.
11. Apply a texture to the **color channel** that you’ve created and name it **_color-{{ page.submission-id }}.jpg_** in the *sourceimages* folder.
12. Create and apply a bump map to **overall bump** called **_bump-{{ page.submission-id }}.jpg_** in the **sourceimages** folder.
13. Adjust the Bump Depth to **0.200** on the bump2d node connected to your bump map channel.
14. Enable Mental Ray as the rendering engine in the render settings.
15. Match the following render settings:  
  Render using **Mental Ray**  
  **Quality Tab**  
    a. Overall Quality: 2 
    b. Indirect Diffuse (GI) Mode: Finalgather	
  **Common Tab**  
    a. Presets: HD 1080
16.  Position **_Cam1_** so that the object is in the center, filling most of the composition.
17. Render the image from **_Cam1_** and save it as **_render-{{ page.submission-id }}.exr_** in the images folder using OpenEXR format. (Not JPG)
18. Import your rendered EXR image into Photoshop and use HDR Tone to improve the image's contrast. You can perform additional manipulations to the image in Photoshop to finalize the render.
19. Save the final image as final-{{ page.submission-id }}.jpg
20. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
21. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L1.zip._**
22. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
23. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 1_ folder structure**

```

{{ page.submission-id }}-L1.zip
|
└── {{ page.submission-id }}-L1
    |
    ├── sourceimages/
    |   |
    |   ├── ibl-{{ page.submission-id }}.exr
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
    |   ├── final-{{ page.submission-id }}.jpg
    |   └── render-{{ page.submission-id }}.exr
    |   
    ├── data/
    ├── clips/
    ├── cache/
    ├── autosave/
    └── assets/

```

### <a name="level-2"></a>Level 2:

1. Watch and read tutorials on Image Based Lighting (IBL).
2. Create and set a project folder called **_{{ page.submission-id }}-L2_**.
3. Set your project folder by choosing **File** → **Set Project**.
4. Create your folder structure by choosing **File** → **Project Window** → **_Accept_**.
5. After researching [thrown ceramic mug](https://www.google.com/search?q=ceramic+mug&espv=2&biw=1239&bih=1013&source=lnms&tbm=isch&sa=X&ved=0ahUKEwi7lN_g7MbKAhWktoMKHRoKC1AQ_AUIBygC#tbm=isch&q=thrown+ceramic+mug), create a new scene and create a polygon model of a **thrown ceramic mug**.
6. Create a new perspective called **_cam1_**. In the camera attributes, change the film gate to **35mm Academy**.
7. In your Cam1 viewport, enable the Resolution Gate: **View** → **Camera** **Settings** → **Resolution** **Gate.**
8. Create an Image Based Lighting node and create your own or select an [existing EXR image to use]({{ site.baseurl }}{{ page.asset-path }}/IBL-pack.zip). Name it **_ibl-{{ page.submission-id }}.exr_**
9. Unfold your UVs using the UV Texture editor other UV tools.
10. Assign a new Mentalray material called a **mila_material** to your object.
11. Add at least two **weighted** layers. (You may add as many additional as needed to create the desired look)
  1. Diffuse Reflection (add a texture to the **weight**, **bump**, and **color** channels)
    - **_diffuse-weight-{{ page.submission-id }}.jpg_**
    - **_diffuse-color-{{ page.submission-id }}.jpg_**
    - **_diffuse-bump-{{ page.submission-id }}.jpg_**
  2. Specular Reflection (add a texture to the **weight** and **bump** channels)
    - **_specular-weight-{{ page.submission-id }}.jpg_**
    - **_specular-bump-{{ page.submission-id }}.jpg_**
11. Save all textures in the **sourceimages** folder.
13. Adjust the Bump Depth to **0.200** on the bump2d node connected to your bump map channels.
14. Enable Mental Ray as the rendering engine in the render settings.
15. Match the following render settings:  
  Render using **Mental Ray**  
  **Quality Tab**  
    a. Overall Quality: 2 
    b. Indirect Diffuse (GI) Mode: Finalgather  
  **Common Tab**  
    a. Presets: HD 1080
16. Position **_Cam1_** to create a nice composition.
17. Render the image from **_Cam1_** and save it as **_render-{{ page.submission-id }}.exr_** in the images folder using OpenEXR format. (Not JPG)
18. Import your rendered EXR image into Photoshop or Aftereffects and use HDR Tone (Photoshop) or EXtracteR (Aftereffects) to improve the image's contrast. You can perform additional manipulations to the image to finalize the render.
19. Save the final image as final-{{ page.submission-id }}.jpg
18. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
19. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L2.zip._**
20. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
21. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 2_ folder structure**

```

{{ page.submission-id }}-L2.zip
|
└── {{ page.submission-id }}-L2
    |
    ├── sourceimages/
    |   |
    |   ├── ibl-{{ page.submission-id }}.exr
    |   ├── diffuse-color-{{ page.submission-id }}.jpg
    |   ├── diffuse-weight-{{ page.submission-id }}.jpg
    |   ├── diffuse-bump-{{ page.submission-id }}.jpg
    |   ├── specular-bump-{{ page.submission-id }}.jpg
    |   └──specular-weight-{{ page.submission-id }}.jpg
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
    |   ├── final-{{ page.submission-id }}.jpg
    |   └── render-{{ page.submission-id }}.exr
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
3. Light your image with an Image Based Lighting node and additional lights as needed.
4. Add a **mila_material** layer shader to your model with diffuse(scatter) set as the base. Add as many layers as needed to reach a high level of detail and visual interest to your model as desired. 
5. Enable Mental Ray as the rendering engine in the render settings.
6. Match the following render settings:  
  Render using **Mental Ray**  
  **Quality Tab**  
    a. Overall Quality: 2 
    b. Indirect Diffuse (GI) Mode: Finalgather  
  **Common Tab**  
    a. Presets: HD 1080
7. Position your camera to create a nice composition.
8. Render the image and save it as **_render-{{ page.submission-id }}.exr_** in the images folder using OpenEXR format. (Not JPG)
9. Import your rendered EXR image into Photoshop or Aftereffects and use HDR Tone (Photoshop) or EXtracteR (Aftereffects) to improve the image's contrast. You can perform additional manipulations to the image to finalize the render.
10. Save the final image as final-{{ page.submission-id }}.jpg
11. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L3.zip._**
12. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
13. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 3_ folder structure**

```

{{ page.submission-id }}-L3.zip
|
└── {{ page.submission-id }}-L3
    |
    ├── sourceimages/
    |   |
    |   └── [texture-names]-{{ page.submission-id }}.jpg
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
    |   ├── final-{{ page.submission-id }}.jpg
    |   └── render-{{ page.submission-id }}.exr
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
