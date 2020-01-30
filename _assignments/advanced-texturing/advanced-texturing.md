---
title: Advanced Texturing # In the future, change this assignment title to PBR Modeling, Texturing, and Rendering
subtitle: 
layout: exercise
submission-id: advanced-texturing-YOURNAME
asset-path: /assets/exercise-images
exercise: exercise-3
---
![advanced texturing image]({{site.baseurl}}{{page.asset-path}}/adv-texturing-exercise.jpg)

In this exercise, you will use a PBR workflow to add realistic textures, set up lights, and configure render settings.

## Learning Resources

***

**Level 1 & 2: Beginner and Intermediate Students**

Physically based materials:

- Blender: [Principled shader documentation](https://docs.blender.org/manual/en/dev/render/cycles/nodes/types/shaders/principled.html)
- [Secrets to photorealism](https://www.youtube.com/watch?v=m9AT7H4GGrA)
- [Ways to Speed Up Blender Cycles Rendering](https://www.youtube.com/watch?v=8gSyEpt4-60)
- [Removing render "fireflies"](https://www.blenderguru.com/articles/7-ways-get-rid-fireflies)

Example texture packs:

- [Texture Haven](https://texturehaven.com/textures/)
- [HDR Environment Assets](https://drive.google.com/drive/folders/1L6gc6B0RFNEZX780XSKj6GXMGo8vEkpY)
- [Rock Texture Pack]({{ site.baseurl }}/assets/exercise-downloads/RockGrey009.zip)
- [Wood Texture Pack]({{ site.baseurl }}/assets/exercise-downloads/WoodFine08.zip)

Blender:

- Blender Foundation - Videos 21-27: [Blender Fundamentals 2.8](https://www.youtube.com/playlist?list=PLa1F2ddGya_-UvuAqHAksYnB0qL9yWDO6)
- [Grant Abbitt - Part 6 Rendering and Atmosphere](https://www.youtube.com/watch?v=g8683RF1COo)
- Blender Reference Sheet: [Blender Hotkeys](http://download.blender.org/documentation/BlenderHotkeyReference.pdf)
- Lynda - Watch Chapters 4 and 7: [Blender Essentials](https://www.linkedin.com/learning/blender-2-8-essential-training-2)
- [Setting up the redner camera in Blender](https://www.youtube.com/watch?v=SG6yOoq7FKI)
- [PBR Materials Demo](https://www.youtube.com/watch?v=FRNCp9GueUs) By Joe Foresman

***

**Level 3: Experienced Students**

- Flipped Normals - [Introduction to Sculpting in Blender 2.8 - Sculpting Essentials](https://www.youtube.com/watch?v=A-Wq8K8icpQ&list=PLBX-X8mPyxIqV8Uto03OdvfnGUHCu9Hxz&index=2)
- [Blender 2.8 - How to bake textures - Tutorial](https://www.youtube.com/watch?v=2ClzsuExtCo)
- [Retopology for Beginners in Blender 2.8 - Retopo the Correct Way](https://www.youtube.com/watch?v=CuQzPDs99yM&list=PLBX-X8mPyxIqV8Uto03OdvfnGUHCu9Hxz&index=1)
- [How To Setup PBR and Displacement in EEVEE AND Cycles Blender 2.8](https://www.youtube.com/watch?v=UkU0-QeWUcU)


***

## Steps to Completion

Choose a either level 1, level 2, or level 3 to complete based on your prior experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.

[Level 1 and 2 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Create a polygonal model of an scultpure that features some illuminated elements set in a room. Focus on using Principled BSDF shaders.
  - The object should have a bulb with an emission (emissive) material and act as a light source
  - You can download and use [texture packs](https://texturehaven.com/textures/).
  - There should be a background environment HDR image.
  - There should be a floor and one more walls of a room visible in the render, use any material you'd like for these. The sculpture should not be "floating in space."
2. Unwrap the UVs for each object if you intend to use textures. Ensure that your materials are mapping with your object's UVs.
3. Select render camera. In camera settings, adjust the camera's framing and focal length to create a good composition. Explore the camera presets. See video tutorial linked in resources.
4. Check the "Lock camera to view" to frame composition with render camera.
5. In Blender, **render** and image using Cycles renderer with the following settings:
  - Image size: X=1920px, Y=1080px
6. In the render window, Image --> Save As **_{{ page.submission-id }}_**.png in the project folder.
7. Save the blend file as **_{{ page.submission-id }}.blend_** in the project folder.
8. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}.zip._**
9. Upload the .zip file to the assignment dropbox.
10. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

### <a name="level-2"></a>Level 2:

1. Create an abstract self portrait using Principled BSDF shaders. See [Adobe Creative Types](https://mycreativetype.com/the-creative-types/) for inspiration.
  - The object should have a studio lighting setup for even lighting.
  - There should be a solid color in the background.
  - You can download and use [texture packs](https://texturehaven.com/textures/).
2. Unwrap the UVs for each object if you intend to use textures. Ensure that your materials are mapping with your object's UVs.
3. Select render camera. In camera settings, adjust the camera's framing and focal length to create a good composition. Explore the camera presets. See video tutorial linked in resources.
4. Check the "Lock camera to view" to frame composition with render camera.
5. In Blender, **render** and image using Cycles renderer with the following settings:
  - Image size: X=1920px, Y=1080px
6. In the render window, Image --> Save As **_{{ page.submission-id }}_L2_**.png in the project folder.
7. Save the blend file as **_{{ page.submission-id }}.blend_** in the project folder.
9. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}.zip._**
10. Upload the .zip file to the assignment dropbox.
11. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

### <a name="level-3"></a>Level 3:

1. Continue your work from the previous exercises.
2. Your model should be a low to medium resolution mesh with a detailed normal map applied. There should also be a finished diffuse texture map.
3. Add an emissive texture to create glowing spots on the creature.
4. Save your **emissive** map in the project folder as **_emissive-{{ page.submission-id }}.png_**.
5. Use an HDR environment map and PBR workflow to light and render your creature.
6. Save the render as **_render-{{ page.submission-id }}.png_**..
7. Save your file as **_{{ page.submission-id }}-L3_.blend**
8. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L3.zip._**
9. Upload the .zip file to the assignment dropbox.
10. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 3_ folder structure**

```

{{ page.submission-id }}-L3.zip
|
├── {{ page.submission-id }}-L3
├── normal-{{ page.submission-id }}.png
├── diffuse-{{ page.submission-id }}.png
├── emissive-{{ page.submission-id }}.png
├── {{ page.submission-id }}.png (you may include additional texture maps as needed)
├── render-{{ page.submission-id }}.png
└── {{ page.submission-id }}.blend

```