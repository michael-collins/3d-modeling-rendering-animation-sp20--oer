---
title: Non-Photorealistic Rendering
subtitle: 
layout: exercise
submission-id: npr-YOURNAME
asset-path: /assets/exercise-images
download-path: /assets/exercise-downloads
exercise: exercise-4
---
![NPR rendering example]({{site.baseurl}}{{page.asset-path}}/npr-exercise.png)

In this exercise, you will learn about NPR techniques to achieve expressive rendering styles using Blender.

## Learning Resources

- [NPR shader example 1 download]({{site.baseurl}}{{page.download-path}}/npr-shader-demo.blend)
- [NPR shader example 2 download]({{site.baseurl}}{{page.download-path}}/npr-demo.zip)

Examples:

- [BlenderNPR.org Downloads](http://blendernpr.org/downloads/)
- [Halftone Shading](https://sharkigator.wordpress.com/2016/01/23/screentone-shading/)
- [RWPY - Tutorial\: How to make a NPR Cartoon Animation](https://www.youtube.com/watch?v=9iHuw8mB0M4)


***

**Level 1: Beginner Students**

- [How to create an NPR Shader Material in Eevee](https://www.youtube.com/watch?v=t91X4eukZY4)
- [Freestyle](https://www.lynda.com/Blender-tutorials/Quick-strokes-freestyle-line-boil/573135/5024027-4.html?org=psu.edu)
- [Advanced Freestyle](https://www.lynda.com/Blender-tutorials/Quick-strokes-freestyle-line-boil/573135/5024027-4.html?org=psu.edu)
- [Cartoon Shading in Cycles](https://www.lynda.com/Blender-tutorials/Cartoon-shading-cycles/573135/5024029-4.html?org=psu.edu)

***

**Level 2: Intermediate Students**

- [Youtube Search - Blender 2.8 freestyle eevee](https://www.youtube.com/results?search_query=blender+2.8+freestyle+eevee)
- [Texture Painting in Blender and rendering for Comics](https://www.youtube.com/watch?v=vIBmH8rVoIA)
- [Advanced Character Freestyle Tutorial](https://www.youtube.com/watch?v=6Tm3yQHrqbE)
- [Comic book/ Manga ink shader / Toon Shader](https://www.youtube.com/watch?v=19yXM13sw6A)

**Level 3: Experienced Students**

- [Texture Painting in Blender and rendering for Comics](https://www.youtube.com/watch?v=vIBmH8rVoIA)
- [Comic Shading using the Compositor in Blender](https://www.youtube.com/watch?v=anIFTskTUKI)


**Resources**

[Blender NPR Posts](https://blendernpr.org/posts/)

***

## Steps to Completion

Choose a either level 1, level 2, or level 3 to complete based on your prior experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.

[Level 1 and 2 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Model an animal using a polygonal modeling workflow (not a human).
2. Follow the relevant tutorials.
3. Choose a style and experiment with shaders, materials, and freestyle lines.
  - Required nodes in the shader editor: Diffuse BSDF, Shader to RGB, ColorRamp, Material Output
  - Add Freestyle Outlines to give the render a more illustrated or drafted look
4. Save a 1920x1080 render as **_render-{{ page.submission-id }}.png_** in the project folder.
6. Save your file as **_{{ page.submission-id }}_.blend** in the project folder.
7. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}.zip._**
8. Upload the .zip file to the assignment dropbox.
9. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

### <a name="level-2"></a>Level 2:

1. Model a polygonal character in the [T pose](https://www.animatorisland.com/the-t-pose-all-about-the-mighty-blueprint/?v=7516fd43adaa). Choose a 'sci-fi' theme or 'zombie apocalypse' theme for the character.
2. Follow the level three tutorials.
3. Create shaders, materials, and freestyle lines to create a manga or comic book visual style.
4. Save a 1920x1080 render as **_render-{{ page.submission-id }}.png_** in the project folder.
6. Save your file as **_{{ page.submission-id }}-L2_.blend** in the project folder.
7. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L2.zip._**
8. Upload the .zip file to the assignment dropbox.
9. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 2_ folder structure**

```

{{ page.submission-id }}-L2.zip
|
├── render-{{ page.submission-id }}.png
└── {{ page.submission-id }}.blend

```

### <a name="level-3"></a>Level 3:

1. Model a hand painted landscape or environment for a comic book or graphic novel.
2. Follow the level three tutorials to learn texture painting and compositing.
3. Create textures, materials, and freestyle lines to create a manga or comic book visual style.
4. Save a 1920x1080 render as **_render-{{ page.submission-id }}.png_** in the project folder.
6. Save your file as **_{{ page.submission-id }}-L3_.blend** in the project folder.
7. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L3.zip._**
8. Upload the .zip file to the assignment dropbox.
9. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 3_ folder structure**

```

{{ page.submission-id }}-L3.zip
|
├── render-{{ page.submission-id }}.png
└── {{ page.submission-id }}.blend

```