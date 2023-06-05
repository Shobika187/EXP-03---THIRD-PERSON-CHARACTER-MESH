# EXP-03---THIRD-PERSON-CHARACTER-MESH
```
Developed by : Shobika P
Register No:212221230096
```
## AIM:
To Change the third person character mesh using animations.

## PROCEDURE:

1.Import the animation assets: Obtain the animation files for jump, walk, and idle in a compatible format such as FBX or BVH. To import the animations, go to the Content Browser panel in Unreal Engine, right-click in the desired folder, and select Import

2.Create a Separate folder and Import the Animations to avoid any chaos

3.Create an animation blueprint: In Unreal Engine, animation blueprints are used to control character animations. To create a new animation blueprint, follow these steps: a. Right-click in the folder where you imported the mesh and select Create > Animation > Animation Blueprint.

a. In the Animation Blueprint Editor, click on the Event Graph tab.

b. Drag the new character mesh from the Content Browser and drop it onto the graph.

c. Connect the Output Pose pin of the mesh node to the Final Animation Pose pin of the Final Animation Pose node.

d. Save the animation blueprint.

4.Open the animation blueprint: Open the animation blueprint you created for your character in the Animation Blueprint Editor.

5.Create animation slots: Animation slots help organize different animations and control their blending. To create animation slots, follow these steps: a. In the AnimGraph tab of the Animation Blueprint Editor, right-click in the graph and select Add State Machine > Animation Layer.

a. Double-click the newly created animation layer to open it.

b. Right-click in the graph of the animation layer and select Add State Machine. d. Double-click the newly created state machine to open it.

c. Right-click in the graph of the state machine and select Add State.

e. Rename the state to "Jump" and repeat steps e and f to create states for "Walk" and "Idle".

6.Add animation assets to states: In each state, you will assign the corresponding animation assets. To add animation assets to the states, follow these steps: a. Double-click the "Jump" state to open it.

a. Right-click in the graph and select Add State Result.

b. Drag and drop the jump animation asset onto the graph.

c. Connect the Result node to the jump animation asset.

d. Repeat steps a to d for the "Walk" and "Idle" states, assigning the appropriate animation assets.

7.Create required Variables for the state’s like “ISJUMP”, “SPEED”.

8.Set up transition rules: Transition rules determine when the character transitions between different animations. To set up transition rules, follow these steps: a. Double-click the "Jump" state to open it.

a. Right-click in the graph and select Add Transition Rule.

b. Drag the transition rule from the "Jump" state to the "Idle" state.

c. Repeat steps a to c for the "Walk" state, creating transitions from "Idle" to "Walk" and from "Walk" to "Idle".

d. Configure the transition rules based on your desired conditions. For example, you might want to trigger the transition from "Idle" to "Jump" when the character jumps, and from "Jump" to "Idle" when the jump animation is finished.

9.Create a Anim Montage in Animation Folder To Manage the montages of the animations.

10.Connect the animation blueprint to the character blueprint: To connect the animation blueprint to the character blueprint and enable the animations in the game, follow these steps: a. Open the character blueprint associated with the third person character.

a. In the Viewport tab of the Blueprint Editor, select the mesh component of the character.

b. In the Details panel, under the Animation category, find the Animation Blueprint property.

c. Click on the dropdown menu and select the animation blueprint you created.

11.Test the character: Compile and save all the changes in the blueprints and animations. Now, you can test the character's jump, walk, and idle animations by clicking the Play button in the Unreal Editor.
## OUTPUT:
### STATE MACHINES:
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/2e1b1c68-0dd9-440c-a86e-0172d15c7fc4)
### STATE DIAGRAM:
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/9f9c8a84-baed-46ae-afa0-793cd5616715)
### VARIABLES:

![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/eb522780-45de-41b9-b34b-c72082ebded3)
### IDLE TO WALK:

![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/ccd5c90d-10dd-40a2-affe-a77305f73b03)
### WALK TO IDLE:
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/7a0545d2-cedc-4dae-a0dc-7063fd14a791)
### WALK TO JUMP:
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/05d18e19-2e91-42a1-86dd-4a4da51497a4)
### JUMP TO WALK:
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/74f32c62-c59e-4654-912d-ca8fff5b5e13)
### JUMP TO IDLE:
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/390d9dfd-fded-4ae1-9077-5a1a38853d7e)
### IDLE TO JUMP:
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/aa0a8a81-2215-4006-9093-1cd82ea3ea5a)
### ANIMATION BLUEPRINT:
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/215c467f-dd69-4971-9467-dcfee588235c)
### ANIMATION MONTAGE:
![P33](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/34fa2f55-f527-4b85-84eb-0bfc84286896)
![p21](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/1f85fe02-6df2-4d22-b07c-e3907352deff)
### THIRD PERSON BLUEPRINT:
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/fb48e4cb-5cd6-4b25-89b2-6ad8360f2298)
## RESULT:
The third person character mesh has been successfully changed using animations.






