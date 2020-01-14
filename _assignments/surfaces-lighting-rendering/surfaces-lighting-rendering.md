---
title: Surfaces, Lighting, and Rendering
subtitle: 
layout: exercise
submission-id: modeling-03-YOURNAME
asset-path: /assets/exercise-images
exercise: exercise-3
---

In this exercise, you will add surface materials, additional textures, set up lights, and configure render settings.

## Learning Resources

---
**Level 1 & 2: Beginner and Intermediate Students**

Physically based materials:

- Blender: [The BSDF material for Cycles](https://www.youtube.com/watch?v=4H5W6C_Mbck&vl=en)
- Blender: [Principled shader documentation](https://docs.blender.org/manual/en/dev/render/cycles/nodes/types/shaders/principled.html)
- Maya: [Physically based rendering in Arnold](https://www.solidangle.com/research/physically_based_shader_design_in_arnold.pdf)

Downloads:

- [Rock Texture Pack]({{ site.baseurl }}/assets/exercise-downloads/RockGrey009.zip)
- [Wood Texture Pack]({{ site.baseurl }}/assets/exercise-downloads/WoodFine08.zip)

Blender:

- Blender Reference Sheet: [Blender Hotkeys](http://download.blender.org/documentation/BlenderHotkeyReference.pdf)
- Lynda - Watch Chapters 5-9: [Blender Essentials](https://www.lynda.com/Blender-tutorials/Blender-Essential-Training/87088-2.html?org=psu.edu)
- [Setting up the redner camera in Blender](https://www.youtube.com/watch?v=SG6yOoq7FKI)
- [PBR Materials Demo](https://www.youtube.com/watch?v=FRNCp9GueUs) By Joe Foresman

Maya:

- Watch Chapters 9-12: [Maya Essential Training](https://www.lynda.com/Maya-tutorials/Maya-2018-Essential-Training/604210-2.html?org=psu.edu)

---

**Level 3: Experienced Students**

- [Lynda.com - ZBrush Essential Training](https://www.lynda.com/ZBrush-4-tutorials/Essential-Training/76980-2.html?org=psu.edu) (Lessons 1- 7) 
- [Lynda.com - Sculpting a Creature with ZBrush](https://www.lynda.com/Photoshop-tutorials/Welcome/366834/386733-4.html?org=psu.edu) (Lessons 1 - 3)  

---

## Steps to Completion

Choose a either level 1, level 2, or level 3 to complete based on your prior experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.

[Level 1 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Using Blender or Maya, create a polygonal model of a lamp.
  - The object should have a bulb with an emission (emissive) material and act as a light source
  - The lamp should have have a plastic body configured using the Principled BSDF shader. You can be clever with the design of the lamp.
  - There should be a floor and one more walls of a room visible in the render, use any material you'd like for these. The lamp should not be "floating in space."
2. Unwrap the UVs for each object if you intend to use textures. Ensure that your materials are mapping with your object's UVs.
3. Adjust the camera's framing and focal length to create a good composition. Explore the camera presets. See video tutorial linked in resources.
4. In Blender, **render** and image using Cycles renderer with the following settings:
  - Image size: X=1920px, Y=1080px
  - Sampling preset: Final
5. In the render window, Image --> Save As **_{{ page.submission-id }}_**.png in the project folder.
9. Save the 3D scene file as **_{{ page.submission-id }}_** in the project folder.
10. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L1.zip._**
11. Upload the .zip file to the [submission dropbox]({{ site.assignments.[page.exercise].dropbox-url }})
12. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

### <a name="level-2"></a>Level 2:

1. Using Blender or Maya, create a polygonal model of a lamp.
  - The object should have a bulb with an emission (emissive) material and act as a light source
  - The lamp should be configured using the Principled BSDF shader. You can be clever with the design of the lamp.
  - There should be a floor and one more walls of a room visible in the render, use any material you'd like for these. The lamp should not be "floating in space."
2. Unwrap the UVs for each object if you intend to use textures. Ensure that your materials are mapping with your object's UVs.
3. Adjust the camera's framing and focal length to create a good composition. Explore the camera presets. See video tutorial linked in resources.
4. In Blender, **render** and image using Cycles renderer with the following settings:
  - Image size: X=1920px, Y=1080px
  - Sampling preset: Final
5. Add the following three texture maps for the BSDF material (or equivilent in Maya):
  - Color map: **_{{ page.submission-id }}_**-color.png
  - Normal map: **_{{ page.submission-id }}_**-normal.png
  - Specular: **_{{ page.submission-id }}_**-spec.png
  - Note: You can ad additional maps as desired. These three are the minimum.
5. In the render window, Image --> Save As **_{{ page.submission-id }}_**.png in the project folder.
9. Save the 3D scene file as **_{{ page.submission-id }}_** in the project folder.
10. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L2.zip._**
11. Upload the .zip file to the [submission dropbox]({{ site.assignments.[page.exercise].dropbox-url }})
12. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

### <a name="level-3"></a>Level 3:

1. Watch the Essential Training and Digital Character Creation tutorials from Lynda on modeling with ZBrush.
2. Using the techniques learned in the Digital Creature Creation tutorials, continue working on your model.
3. Create the textures covered in the Digital Character Creation tutorials.
4. Import your model into Maya or Blender and connect the textures to the creature’s shader.
5. Save your scene as **_{{ page.submission-id }}-L3_** in the scenes folder.
6. Save your PSD texture in the *sourceimages* folder as **_{{ page.submission-id }}-L3.psd_**. ([See Organizing the maps into Photoshop layers](http://www.lynda.com/3D-Animation-Character-Design-tutorials/Digital-Creature-Creation-in-ZBrush-Photoshop-and-Maya/83781-2.html) on Lynda.com)
7. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L3.zip._**
8. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
9. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 3_ folder structure**

```

{{ page.submission-id }}-L3.zip
|
├── {{ page.submission-id }}-L3
├── {{ page.submission-id }}.jpg (as many textures as required)
└── {{ page.submission-id }}.blend or .mb

```