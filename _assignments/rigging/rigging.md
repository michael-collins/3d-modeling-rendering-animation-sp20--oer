---
title: Character Rigging in Blender
subtitle: 
layout: exercise
submission-id: rigging-YOURNAME
assignment-dropbox: 
exercise: exercise-6
asset-path: /assets/exercise-images
download-path: /assets/exercise-downloads
---
![Rig in Blender]({{ site.baseurl }}{{ page.asset-path }}/blender-rigging.png)

In this exercise, you will practice creating a rig for a polygon mesh. You will create a simple biped rig starting with the [base mesh FBX file]({{site.baseurl}}{{page.download-path}}/biped-base-mesh.fbx).

## Learning Resources:

***

**Level 1: Novice Students**

* Lynda.com: [Character Rigging](https://www.linkedin.com/learning-login/share?forceAccount=false&redirect=https%3A%2F%2Fwww.linkedin.com%2Flearning%2Frigging-a-humanoid-character-with-blender%3Ftrk%3Dshare_ent_url&account=76811570)
* [Weight Painting](https://www.youtube.com/watch?v=Tl4qTgwQwYw)
* [Rigging People](https://www.youtube.com/watch?v=cp1YRaTZBfw)
* [Rigging a character in blender 2.80](https://www.youtube.com/watch?v=gMnH9vvMLYg)
* Lynda Tutorials: [12 Principles of Animation](https://www.lynda.com/3ds-Max-tutorials/12-Principles-Animation-CG-Animators/474685-2.html?org=psu.edu)

***

**Level 2: Intermediate Students**

* [Modeling a Low Ploy Animal](https://www.youtube.com/watch?v=6mT4XFJYq-4)
* [Rigging Animals with Rigify in BLENDER 2.80](https://www.youtube.com/watch?v=MZg97cmTcIs)
* [Quadruped Rigging in Blender Part 1: Inverse Kinematics Rig](https://www.youtube.com/watch?v=mnFRyVZd8TI)
* [Quadruped Rigging in Blender Part 2: Inverse Kinematics Rig](https://www.youtube.com/watch?v=DlHqrdcpjUI)

***

**Level 3: Experienced Students**

* [Blender 2.8 - Rigging For Animation 6 \| Introduction To IK Part 1](https://www.youtube.com/watch?v=LYqsEEgan7s)
* [Blender 2.8 - Rigging For Animation 11 \| How To Rig A Piston Part 1](https://www.youtube.com/watch?v=QEUVgS3Ag-g)
* [Blender 2.8 - Rigging For Animation 11 \| How To Rig A Piston Part 2](https://www.youtube.com/watch?v=F6eBF76heYg)

***

## Steps to Completion

Choose a either level 1, level 2, or level 3 to complete based on your prior experience with 3D tools. If you are a novice, choose Level 1. If you have some experience, choose Level 2. If you are very experienced with 3D tools, choose Level 3.

[Level 1 Steps](#level-1) | [Level 2 Steps](#level-2) | [Level 3 Steps](#level-3)

### <a name="level-1"></a>Level 1:

1. Watch the rigging character rigging tutorials.
2. Download the base [base mesh FBX file]({{site.baseurl}}{{page.download-path}}/biped-base-mesh.fbx).
3. File → Import the FBX mesh into a new Blender scene.
4. Scale up the model.
5. Add subdivisions (edge loops) to the polygonal mesh to minimize unwanted distortion when posing the mesh. Add geometry to articulate the head, torso, legs, and arms.
6. Object → **Apply** all transforms including scale, rotation, and location.
7. Create joints for the torso, hips, knees, legs, feet, shoulders, arms, neck, and head. Name and number them for your reference. You must put a ".L" or ".R" at the end of your bones for them to symmetrize properly.
8. Attach the armature to the polygonal mesh. Do this by selecting the mesh first, select the armature, and then press 'CTRL-P,' and choose "with automatic weights." If you do not see this option, you have selected in the reverse order.
9. Adjust the influence weight where needed to create a posable character.
10. Pose the biped to be in a sitting pose. (You can add a chair if you like)
11. Do not model the character into a sitting pose, it must be modeled in a T pose, and posed in a seated position via the rig.
12. Save as **_{{ page.submission-id }}.blend_** and upload to the submission dropbox.
13. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

### <a name="level-2"></a>Level 2:

1. Watch the level 2 rigging tutorials.
2. Create a quadruped (four-footed animal). It must include the following:
   - Named bones
   - IK/FK rig and controllers
   - Properly painted weights
3. Save as **_{{ page.submission-id }}-L2.blend_** and upload to the submission dropbox.
4. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.


### <a name="level-3"></a>Level 3:

1. Watch the level 3 rigging tutorials.
2. Design a unique robot arm made of at least 4 main parts, including a gripper, a forearm, an upper arm, and a piston. You may add additional elements as you see fit.
   - Create a rig for hard objects (do not download an existing rig)
   - include at least one rigged piston.
   - Include and IK system to control and animate the arm.
3. Create a short animation that shows off the capability of your robot arm design and rig. The animation does not have to be rendered.
3. Save as **_{{ page.submission-id }}-L3.blend_** and upload to the submission dropbox.
7. Ensure you’ve included everything properly. Failure to ensure that you’ve uploaded the file will result in your exercise being graded according the grading criteria.

* * *

## Grading
Your grade will be assessed according to the [Exercise Grading Criteria]({{ site.baseurl }}/grading). 