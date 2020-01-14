---
title: Maya Dynamics
subtitle: 
layout: exercise
asset-path: /assets/exercise-images
---

**Exercise Details**

    

In this exercise, you will create a 2 second (48 frame) animation of dynamic nCloth objects, the associated batch render passes, and an exported final composite of the render passes from After Effects in H.264 format.

* * *


**Learning Resources**

Animation/Dynamics

            Digital Tutors: [Turntable](http://www.digitaltutors.com/11/training.php?vid=12361&autoplay=1)

            Lynda (Lesson 4): [Working with nParticles](http://www.lynda.com/Maya-2009-tutorials/new-features/707-2.html) 

            Digital Tutors: [nCloth Sphere](http://www.digitaltutors.com/11/training.php?vid=1048&autoplay=1)

            Digital Tutors: [nCloth Cache](http://www.digitaltutors.com/11/training.php?vid=6036&autoplay=1) (Required to batch render)

Lynda (Lesson 4 → Building an nCache):  [Creating Particle and Fire Effects in Maya](http://www.google.com/url?q=http%3A%2F%2Fwww.lynda.com%2FMaya-2012-tutorials%2FCreating-Particle-and-Fire-Effects-with-Maya%2F83837-2.html&sa=D&sntz=1&usg=AFQjCNGLaeCEnL66B9vPihX9jDmnYLM7mQ)

Render Passes

Lynda (Lesson 1 - 4): [Maya Rendering for After Effects Composites](http://www.lynda.com/After-Effects-tutorials/Maya-Rendering-After-Effects-Composites/97402-2.html)

        Digital Tutors:[ Setting up render passes](http://www.digitaltutors.com/11/training.php?pid=3575)

    Digital Tutors:[ Luminance Depth](http://www.digitaltutors.com/11/training.php?vid=10044&autoplay=1)

Digital Tutors:[ Creating an Ambient Occlusion Render Pass](http://www.digitaltutors.com/11/training.php?vid=13589&autoplay=1)

    

        Batch Rendering

Lynda (Lesson 5):[ Maya Essentials 6: Lights and Rendering](http://www.lynda.com/Maya-tutorials/Maya-Essentials-6-Lights-Rendering/96718-2.html)

    Digital Tutors:[ Introduction to Rendering in Maya](http://www.digitaltutors.com/11/training.php?vid=21419&autoplay=1)      

        Import/Export After Effects

            Tutorial:[ Exercise 9: After Effects Image Sequence to H.264](https://docs.google.com/document/d/1R5G3bvXoe0_Bto59_dV4c4_iLZIA1--sHRQ8fhkBnvc/edit) 

        More information on Render Passes:

Digital Tutors: [Set up basic render passes and layers](http://www.digitaltutors.com/11/training.php?vid=21945&autoplay=1)

Digital Tutors: [3D Compositing in After Effects](http://www.digitaltutors.com/11/training.php?vid=10899&autoplay=1)

* * *


**Steps to Completion**

1) Watch the tutorials from Lynda and Digital Tutors.

2) Save a new scene called **_ex_10_yourstudentID.mb_**, set your scene to the project folder, and create the sub folders by choosing **_File_** → **_Project Window_*** → ***_Accept_***.*

3) Create a 48 frame dynamic nCloth animation of objects impacting each other. If you cannot decide what to create, follow the [sphere tutorial](http://www.digitaltutors.com/11/training.php?vid=1048&autoplay=1). Experiment with keyframing nCloth settings changes. Ensure you create an "nCache" after you achieve the desired animation for each object. 

4) Create the following render passes:

            - Diffuse

- Diffuse Material Color

- Indirect

- Reflection

- Specular

- Ambient Occlusion ([tutorial](http://www.digitaltutors.com/11/training.php?vid=13589&autoplay=1))

- Depth ([tutorial](http://www.digitaltutors.com/11/training.php?vid=10044&autoplay=1))

- Shadow

- matte

5) Batch Render your animation with these Render Settings

        a) **Render Using:** Mental Ray

        b) **Common Tab:**

**          **File Name Prefix: **<Scene>/<RenderLayer>/<RenderPassType>**

            Image Format:** Maya IFF**

            Frame/Animation ext: **name.#.ext ****(NOT name.ext.#)**

            Frame padding: **2**

            Start Frame: **1**

            End Frame: **48**

            By Frame: **1**

            Alpha channel (Mask): **Checked**

            Presets: **HD 540**

        C) **Features Tab:**

            Raytracing: **Checked**

            Global Illumination: **Not Checked**

            Final Gathering: **Checked**

d) **Quality Tab:**

            Quality: **1**

            Motion Blur: **Full Deformation**

             Framebuffer → Premultiply:** Unchecked**

        e) **Indirect lighting:**

            Click this button:** Create Physical Sun and Sky**

            In Physical Sun and Sky Attributes → Use Background: **Checked**

6) Import your render pass sequences to After Effects

7) Create the following layers with their respective blending mode:

            - Specular / Screen

- Reflection / Screen

- Indir ect / Screen

- Ambient Occlusion / Multiply

- Shadow / Multiply or use as an alpha mask on a black solid layer

- Diffuse / Normal ← (Apply the "Matte Pass as mask if Alpha doesn’t work)

- Diffuse Material Color / Normal

- Luminance Depth / Normal (use this pass with the lens blur effect)

8) Export an H.264 MP4 movie file. To do this,[ follow this tutorial](https://docs.google.com/document/d/1R5G3bvXoe0_Bto59_dV4c4_iLZIA1--sHRQ8fhkBnvc/edit). (It should be about 1MB in total file size)

9) Put your H.264 video into the project folder in movies folder.

10) Compress the project folder once you’ve completed the tutorial and rename it **_ex_10_yourstudentID.zip._**

11) Upload the .zip file to Lore → Calendar → Exercise 10.

12) Download and unzip the file that you uploaded to ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded as a late submission, or a 50% reduction in your grade.

* * *


## Grading

Your grade will be assessed according to the [Exercise Grading Criteria](https://docs.google.com/document/d/16KERm1NWgcl8CH-fPwGSSW0RJYlXDCOCwVM8WrRVuKw/edit?usp=sharing). 

