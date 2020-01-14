---
title: Modeling and Texturing
subtitle: 
layout: exercise
submission-id: modeling-02-YOURNAME
asset-path: /assets/exercise-images
exercise: exercise-2
project-file: /assets/exercise-downloads/airline-chair-1.blend
---

In this exercise, you will continue 3D modeling and begin texturing. There are different tutorials and exercise submission requirements for three experience levels. Choose the experience level that matches your own.

## Learning Resources

---

**Level 1: Novice Students**

Blender:

- Blender Reference Sheet: [Blender Hotkeys](http://download.blender.org/documentation/BlenderHotkeyReference.pdf)
- Lynda - Watch Chapters 1- 4 and 7: [Blender Essentials](https://www.lynda.com/Blender-tutorials/Blender-Essential-Training/87088-2.html?org=psu.edu)
- Lynda - Watch Chapters 1- 4: 
[Texturing](https://www.lynda.com/Blender-tutorials/Blender-UV-Mapping/169107-2.html?org=psu.edu)

Maya:

- Watch Chapters 1-6, and 10: [Maya Essential Training](https://www.lynda.com/Maya-tutorials/Maya-2018-Essential-Training/604210-2.html?org=psu.edu)

Reference:

- Airline Chair: [Download]({{ site.baseurl }}{{page.project-file}})
- Modeling reference: [Speed modeling a chair](https://www.youtube.com/watch?v=xvpcchM9AfA)

---

**Level 2: Intermediate Students**

Blender:

- Lynda - Watch up to Chapter 4 and 7: [Blender Essentials](https://www.lynda.com/Blender-tutorials/Blender-Essential-Training/87088-2.html?org=psu.edu)
- Lynda - Watch Chapter 1 - 4: 
[Texturing](https://www.lynda.com/Blender-tutorials/Blender-UV-Mapping/169107-2.html?org=psu.edu)

Maya:

- Lynda.com [Advanced Modeling](https://www.lynda.com/Maya-tutorials/Maya-Advanced-Modeling/622047-2.html?org=psu.edu)
- Lynda.com [Advanced texturing](https://www.lynda.com/Maya-tutorials/Maya-Advanced-Texturing/622048-2.html?org=psu.edu)

---

**Level 3: Experienced Students**

- [Lynda.com - ZBrush Essential Training](https://www.lynda.com/ZBrush-4-tutorials/Essential-Training/76980-2.html?org=psu.edu) (Lessons 1- 7)  
- [Lynda.com - Sculpting a Creature with ZBrush](https://www.lynda.com/Photoshop-tutorials/Welcome/366834/386733-4.html?org=psu.edu) (Lessons 1 - 3)  

---

## Steps to Completion

Choose a either level 1, level 2, or level 3 to complete based on your prior experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.

[Level 1 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Duplicate the project folder and continue working on your model from the previous exercise. Optionally, you can start with this [project file]({{ site.baseurl }}{{page.project-file}}).
2. Refine the [Kem Weber Airline Chair](https://collection.cooperhewitt.org/objects/404536651/images/) you began modeling. (Be careful not to accidentally create nurbs primitives when modeling)
   - Skills to practice include:
     - [Subdivision surfaces](https://docs.blender.org/manual/en/dev/modeling/meshes/editing/subdividing/bevel.html?highlight=bevel)
     - Adding [bevels](https://docs.blender.org/manual/en/dev/modeling/meshes/editing/subdividing/bevel.html?highlight=bevel) and [edges](https://docs.blender.org/manual/en/dev/modeling/meshes/editing/edges.html#edge-slide)
     - Ensure [normals](https://docs.blender.org/manual/en/dev/modeling/meshes/editing/normals.html) are facing the proper direction
3. Clean up your [edge flow](https://www.youtube.com/watch?v=Lip59doQQRk).
4. Unwrap the chair's parts' UVs using the various methods and tools described in the tutorials.
5. Export a UV map for each part and save it in the project folder as **_uv_1.jpg_**, **_uv_2.jpg_**, etc.
6. Import the UV maps into Photoshop and create textures to match the Airline Chair as closely as possible.
7. Save the textures as _**arm_color.jpg**_, _**cushion1_color.jpg**_, etc. in the project folder. Name the files in an organized and logical way.
8. In Blender or Maya, set up the chair's textures so they are visible on the model.
9. Save the 3D scene file as **_{{ page.submission-id }}_** in the project folder.
10. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L1.zip._**
11. Upload the .zip file to the [submission dropbox]({{ site.assignments.[page.exercise].dropbox-url }})
12. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 1_ folder structure**

```

{{ page.submission-id }}-L1.zip
|
├── [chair part]_uv-{{ page.submission-id }}.jpg (as many as needed)
├── [chair part]_color-{{ page.submission-id }}.jpg (as many as needed)
└── chair-{{ page.submission-id }}.blend or .mb

```

### <a name="level-2"></a>Level 2:

1. Duplicate your project folder from the previous exercise and rename it to **_{{ page.submission-id }}-L2_**.
2. For each of the three objects you modeled in the last exercise:
  a. Unwrap the object’s UVs
  b. Export a UV snapshot
  c. Create a color texture in Photoshop (1024px by 1024px).
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
6. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L2.zip._**
7. Upload the .zip file to the [submission dropbox]({{ page.assignment-dropbox }})
8. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 2_ folder structure**

```

{{ page.submission-id }}-L2.zip
|
├── uv1-{{ page.submission-id }}.jpg
├── uv2-{{ page.submission-id }}.jpg
├── uv3-{{ page.submission-id }}.jpg
├── color1-{{ page.submission-id }}.jpg
├── color2-{{ page.submission-id }}.jpg
├── color3-{{ page.submission-id }}.jpg
├── obj1-{{ page.submission-id }}.blend OR .mb
├── obj2-{{ page.submission-id }}.blend OR .mb
└── obj3-{{ page.submission-id }}.blend or .mb

```

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