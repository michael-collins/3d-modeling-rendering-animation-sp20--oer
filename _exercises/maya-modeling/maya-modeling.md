---
title: Maya Modeling
subtitle: 
layout: exercise
submission-id: modeling-YOURSTUDENTID
asset-path: /assets/exercise-images
---

In this exercise, you will gain basic understanding of modeling fundamentals. There are different tutorials and exercise submission requirements for three experience levels. Choose the experience level that matches your own.

## Learning Resources

### Tutorials:

**Level 1: Novice Students**

Watch Lesson 4, 5, and 6: [Lynda.com - Modeling with Polygons](https://www.lynda.com/Maya-tutorials/Maya-2017-Essential-Training/432363-2.html?srchtrk=index%3a1%0alinktypeid%3a2%0aq%3amaya+2017+modeling%0apage%3a1%0as%3arelevance%0asa%3atrue%0aproducttypeid%3a2)

**Level 2: Intermediate Students**

[Lynda.com - Advanced Modeling](https://www.lynda.com/Maya-tutorials/Maya-Advanced-Modeling/622047-2.html?org=psu.edu)

**Level 3: Experienced Students**

[Lynda.com - ZBrush Essential Training](https://www.lynda.com/ZBrush-4-tutorials/Essential-Training/76980-2.html?org=psu.edu) (Lessons 1- 7)  
[Lynda.com - Sculpting a Creature with ZBrush](https://www.lynda.com/Photoshop-tutorials/Welcome/366834/386733-4.html?org=psu.edu) (Lessons 1 - 3)  

**Reference Websites**

[Youtube: Good Edge Flow](https://www.youtube.com/watch?v=Lip59doQQRk)

[Random Objects Generator](http://www.randomlists.com/things)

## Steps to Completion

Choose a either level 1, level 2, or level 3 to complete based on your prior experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.

[Level 1 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Watch tutorials from Lynda on introduction to modeling.
2. Download [these project files](https://drive.google.com/file/d/194-L3lZRCvcHYssHXoXKl36aOBtGydNn/view?usp=sharing) and use the scene file as the starting point and rename the project folder to : **_{{ page.submission-id }}_**.
3. Set your project to the downloaded folder by choosing **File** → **Set Project**.
4. Model the airplane from the reference images with your newly learned modeling skills with polygons. (Be careful not to accidentally create nurbs primitives when modeling)
  - Skills to practice include:
     - ploygonal edge flow
     - extruding polygon faces
     - inserting edge loops
     - moveing, rotating, and scaling vertecies, edges, and faces
     - mirroring and duplicating geometry
5. Clean up your [edge flow](https://www.youtube.com/watch?v=Lip59doQQRk).
5. Save your scene as **_{{ page.submission-id }}_** in the scenes folder.
6. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L1.zip._**
7. Upload the .zip file to the [submission dropbox]({{ site.assignments.exercise-2.dropbox-url }})
8. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 1_ folder structure**

```

{{ page.submission-id }}-L1.zip
|
└── {{ page.submission-id }}-L1
    |
    ├── sourceimages/
    |   |
    |   └── reference images/
    |       |
    |       ├── front.jpg
    |       ├── side.jpg
    |       └── top.jpg
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

1. Watch Lynda tutorials for advanced modeling.
2. Obtain three randomly generated objects from [this website](http://www.randomlists.com/things). Include a screenshot of the website objects in your **_sourceimages_** folder called **_objects-{{page.submission-id}}}.jpg (or .png)_**
3. Create a new project folder with associated sub-folders (**File** → **Project Window** → **_Accept_**). Create a new scene for each object and save in the **_scenes_** folder.  
  *Naming:*  
  **_obj1-{{ page.submission-id }}_**  
  **_obj2-{{ page.submission-id }}_**  
  **_obj3-{{ page.submission-id }}_**  

4. Create 3 reference image planes for each object with pencil and paper or in Photoshop. Set up the image reference planes in their respective scenes files. Ensure they are square. Place them in the **_sourceimages_** → **_referenceimages_** folder. [Instructions for aligning reference images in Photoshop:](https://app.pluralsight.com/player?course=beginners-guide-image-planes-maya-70&author=kyle-green&name=beginners-guide-image-planes-maya-70-m2&clip=0&mode=live)
  *Naming:*  
  **_obj1-side-{{ page.submission-id }}.jpg_**  
  **_obj1-front-{{ page.submission-id }}.jpg_**  
  **_obj1-top-{{ page.submission-id }}.jpg_**  
  **_obj2-side-{{ page.submission-id }}.jpg_**  
  **_obj2-front-{{ page.submission-id }}.jpg_**  
  **_obj2-top-{{ page.submission-id }}.jpg_**  
  **_obj3-side-{{ page.submission-id }}.jpg_**  
  **_obj3-front-{{ page.submission-id }}.jpg_**  
  **_obj3-top-{{ page.submission-id }}.jpg_**  

5. Create one polygonal model for each scene file from your set of randomly generated objects in Step 2. (You should be making three objects since you’ve created three scenes.)
6. Capture the gesture of the objects with as little detail as needed to describe the shape.
  - Do not "smooth" the objects.
  - Focus on maintaining quads and good [edgeflow](https://www.youtube.com/watch?v=Lip59doQQRk).
    **See example image of a crowbar below:**  
    ![image alt text]({{ site.baseurl }}{{ page.asset-path }}/maya-modeling-1.jpg)  

7. Compress the project folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L2.zip._**
8. Upload the .zip file to the [submission dropbox]({{ site.assignments.exercise-2.dropbox-url }})
9. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 2_ folder structure**

```

{{ page.submission-id }}-L2.zip
|
└── {{ page.submission-id }}-L2
    |
    ├── sourceimages/
    |   |
    |   ├── objects-{{ page.submission-id }}.jpg
    |   |
    |   └── referenceimages/
    |       |
    |       ├── obj1-front-{{ page.submission-id }}.jpg
    |       ├── obj1-side-{{ page.submission-id }}.jpg
    |       ├── obj1-top-{{ page.submission-id }}.jpg
    |       ├── obj2-front-{{ page.submission-id }}.jpg
    |       ├── obj2-side-{{ page.submission-id }}.jpg
    |       ├── obj2-top-{{ page.submission-id }}.jpg
    |       ├── obj3-front-{{ page.submission-id }}.jpg
    |       ├── obj3-side-{{ page.submission-id }}.jpg
    |       └── obj3-top-{{ page.submission-id }}.jpg
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

1. Watch the tutorials from Lynda on modeling with ZBrush.
2. Using the techniques learned in the Digital Creature Creation tutorials, create a **Clothed creature with quite large ears**.
3. Your ZBrush model should be of similar refinement to the model in Sculpting a Creature with ZBrush, by the end of Lesson 3.
4. Take a screenshot of your model and rename the image as **_{{ page.submission-id }}.png_**.
5. Save your image in a project folder **_{{ page.submission-id }}-L3_**.
6. Compress the folder once you’ve completed the tutorial and rename it **_{{ page.submission-id }}-L3.zip._**
7. Upload the .zip file to the [submission dropbox]({{ site.assignments.exercise-2.dropbox-url }})
8. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

**Example _Level 3_ folder structure**

```

{{ page.submission-id }}-L3.zip
|
└── {{ page.submission-id }}-L3
    |
    └──{{ page.submission-id }}.png

```

* * *

## Grading
Your grade will be assessed according to the [Exercise Grading Criteria]({{ site.baseurl }}/grading). 



