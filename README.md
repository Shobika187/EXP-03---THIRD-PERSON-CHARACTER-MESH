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
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/eb9a8e7a-2014-4462-af1f-f6017597e819)
![image](https://github.com/Shobika187/EXP-03---THIRD-PERSON-CHARACTER-MESH/assets/94508142/65862955-797e-4b01-85e9-12f60ebafb56)
![Uploading image.png…]()
![Uploading image.png…]()
![Uploading image.png…]()
