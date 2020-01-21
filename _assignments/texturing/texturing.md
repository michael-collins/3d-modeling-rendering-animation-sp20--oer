---
title: Texturing
subtitle: 
layout: exercise
submission-id: texture-YOURNAME
asset-path: /assets/exercise-images
exercise: exercise-2
project-file: /assets/exercise-downloads/airline-chair-2-8.blend
---

![Chair render]({{ site.baseurl }}{{ page.asset-path }}/chair-render-compressed.jpg)

In this exercise, you will continue 3D modeling and begin texturing. There are different tutorials and exercise submission requirements for three experience levels. Choose the experience level that matches your own.

## Learning Resources

***

**Level 1: Novice Students**

- Blender Foundation - Videos 16-20: [Blender Fundamentals 2.8](https://www.youtube.com/playlist?list=PLa1F2ddGya_-UvuAqHAksYnB0qL9yWDO6)
- LinkedIn Learning - Chapter 4: 
[Textures and shading](https://www.linkedin.com/learning/blender-2-8-essential-training-2/introducing-blender-2-8-for-beginners)
- **Chair Modeling Reference:**
  - Airline Chair: [Download]({{ site.baseurl }}{{page.project-file}})
  - Modeling reference: [Speed modeling a chair](https://www.youtube.com/watch?v=xvpcchM9AfA)

***

**Level 2: Intermediate Students**

- Blender Foundation - Videos 16-20: [Blender Fundamentals 2.8](https://www.youtube.com/playlist?list=PLa1F2ddGya_-UvuAqHAksYnB0qL9yWDO6)
- Lynda - Chapter 4: 
[Textures and shading](https://www.linkedin.com/learning/blender-2-8-essential-training-2/introducing-blender-2-8-for-beginners)
- Jayanam - [Blender 2.8 PBR Texturing for Beginners](https://www.youtube.com/watch?v=XI-pZshRp8g)
- [How To Setup PBR and Displacement in EEVEE AND Cycles Blender 2.8](https://www.youtube.com/watch?v=UkU0-QeWUcU)

***

**Level 3: Experienced Students**

- Flipped Normals - [Introduction to Sculpting in Blender 2.8 - Sculpting Essentials](https://www.youtube.com/watch?v=A-Wq8K8icpQ&list=PLBX-X8mPyxIqV8Uto03OdvfnGUHCu9Hxz&index=2)
- [Blender 2.8 - How to bake textures - Tutorial](https://www.youtube.com/watch?v=2ClzsuExtCo)
- [Retopology for Beginners in Blender 2.8 - Retopo the Correct Way](https://www.youtube.com/watch?v=CuQzPDs99yM&list=PLBX-X8mPyxIqV8Uto03OdvfnGUHCu9Hxz&index=1)
- [How To Setup PBR and Displacement in EEVEE AND Cycles Blender 2.8](https://www.youtube.com/watch?v=UkU0-QeWUcU)

***

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
7. Save the textures as _**arm_color.jpg**_, _**cushion1_color.jpg**_, etc. in the project folder. Name the files in an organized in a logical way.
8. In Blender, set up the chair's textures so they are visible on the model.
9. Save the 3D scene file as **_{{ page.submission-id }}_** in the project folder.
10. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L1.zip._**
11. Upload the .zip file to the assignment dropbox.
12. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 1_ folder structure**

```

{{ page.submission-id }}-L1.zip
|
├── [chair part]_uv-{{ page.submission-id }}.jpg (as many as needed)
├── [chair part]_color-{{ page.submission-id }}.jpg (as many as needed)
└── chair-{{ page.submission-id }}.blend

```

### <a name="level-2"></a>Level 2:

1. Duplicate your project folder from the previous exercise and rename it to **_{{ page.submission-id }}-L2_**.
2. For each of the three objects you modeled in the last exercise:
  a. Unwrap the object’s UVs
  b. Export a UV snapshot (UV wireframes)
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
7. Upload the .zip file to the assignment dropbox.
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
├── obj1-{{ page.submission-id }}.blend
├── obj2-{{ page.submission-id }}.blend
└── obj3-{{ page.submission-id }}.blend 

```

### <a name="level-3"></a>Level 3:

1. Watch the level 3 tutorials.
2. Continue working on your model from the previous exercise.
3. Retopologize the mesh.
4. Create two maps: A **diffuse map** and a **normal map**.
5. Follow the **Normal Maps and Nodes** tutorial to connect the textures to the creature’s shader.
6. Save your file as **_{{ page.submission-id }}_.blend**
7. Save your diffuse map in the project folder as **_diffuse-{{ page.submission-id }}.png_**.
7. Save your normal map in the project folder as **_normal-{{ page.submission-id }}.png_**.
7. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L3.zip._**
8. Upload the .zip file to the assignment dropbox.
9. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 3_ folder structure**

```

{{ page.submission-id }}-L3.zip
|
├── diffuse-{{ page.submission-id }}.png
├── normal-{{ page.submission-id }}.png
└── {{ page.submission-id }}.blend

```