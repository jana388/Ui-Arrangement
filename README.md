# Ui-Setup
## Tutorial for putting an UI in a game
This is a beginners guide to setup a UI in your game.
By the end of this tutorial you will know have to set up a score count on the top of the screen!
This tutorial can be applicable on both 2D and a 3D project.

## Prerequisites

For this tutorial, I will be using a 3D project in Unity 2022.3.46f1. However, this can be applicable on 2D and any newer versions of Unity.
Since there will not be any programming in this tutorial, we will not need Microsoft Visual Studio.


## Setting up the User Interface

A **UI** is a simple tool that helps the player interact with games' features and mechanics. By the help of a few clicks, your game can have a camera view based visual which will guide a player throughout the game.

The first thing we need to do is open a project *(does not matter if it is 2D or 3D)* an then go to the Hierarchy. 

Right click on the area and a **drop menu** should appear.

![Screenshot (366)](https://github.com/user-attachments/assets/62f2943b-fec3-404d-9fb1-e9538fbc8466)

You will see an **UI icon** shown on that list. Press it and you will get another drop menu. There are various options we can choose from like *Image, Text, ScrollBar* and so on.
We will go to Panel and left click it.

After doing these steps correctly, a scene will change. You should notice a Panel in your scene. In the Hierarchy, we can see that Panel is a child of a canvas.

![Capture2](https://github.com/user-attachments/assets/125e3d43-8683-42b5-9bab-c5b1558f2c25)


> - Why can't the Panel be by itself, and why does it have to be a child of the Canvas?
> - The Canvas is a root to every UI element, hence each one is a child to it
> - This ensures we render the UI element correctly within the scene
> - When adding a UI not only do we automatically get a canvas but also an **Event System object**.
> - Event system facilitates the interaction between the input *(mouse, keyboard, joystick)* and the visual output
> - It will map various inputs to appropraite function
> - It is used to process the input and map it to its corresponding UI or Game object and invoke its appropriate function
> - Note that we do not have to alter it since it is automatic!

## Resizing the panel


Now if the panel is too big on your screen, there is an option to zoom out and see it from the *front perspective*:
- We can go to a 2D view (if you are in a 3D game)
- Select the canvas and put your mouse cursor on the scene
- Now hit the key **F** for frame and it will zoom out on the whole canvas
- If you enter the *Game mode*, you will see that the panel is covering the whole screen
- You can click and drag the panel to resize it manually by placing the mouse cursor to the edge of the panel until an *up and down arrow* appears
- There is an easier way to do this, and the results end up more organised and the size of the panel will be fixated no matter what the size of the screen is

## Navigating the Inspector

**We can resize the panel automatically by going to the inspector!**

As an example, let's make a **Score count** for left and right goal in a game.
As for now, if we enter **Game Mode**, the panel would cover the whole screen. Ofcourse, we would only like our UI to be on the *top centre screen* .

> UI should not a be in focus of the game, but rather a **tool** for the player to follow some important data in the game!

We can use a tool in the inspector by left clicking on the *frame* in the square. 

![Capture3](https://github.com/user-attachments/assets/849b1d3d-bbd1-4f10-8669-8850764ea1b7)

Then a drop menu will appear with the following:

![Screenshot (369)](https://github.com/user-attachments/assets/c763d723-127e-4f85-8654-f1cc92459ec8)

Those are automatic presets that allow us to correctly resize our panel.
By clicking on the box, we can change our **pivot, position and strech settings**
For even more options, you can hold *Shift* and *Alt* to access even more options
Now if we would go to the inspector and access the presets

I will choose *Top stretch*

![Screenshot (370)](https://github.com/user-attachments/assets/a6b1f840-6e9e-4458-b1d4-6c5b64a5ac28)
> To find this option, hold Shift and Alt and left click on the box on the top right corner.

Now that we got the position right, we can change the height.

Go back to Inspector and go to height.
We will change it to 110 so it will only cover the upper part of the screen

![Screenshot (3722)](https://github.com/user-attachments/assets/e7d66cf7-1d0f-449e-9a20-d7a295d0cc82)

This is what it should look like:

![Screenshot (3723)](https://github.com/user-attachments/assets/da55ef66-8836-4a92-9ae7-61069cffce80)

If we go down to image, we can change the fill and the colour of the panel, or we can deactivate it.
All of these options are useful for visualisation of the wished UI

![Capture6](https://github.com/user-attachments/assets/b20d13f4-39fe-4af4-9292-66439052c533)

We are going to deactivate it, since we do not want to cover the whole area, we just want to put the numbers for the score.

To deactivate it, untick the box next to the **Image**
If you have done these steps right, you can proceed to add the text to the UI.

## Adding the text
**Now we will add some text to the panel.**
We are going to go to the Hierarchy and right click on the panel and select UI and text.
Now we have a little text box.
we will not worry about the position of the box.
 we will not bother editing the text too much, for now we will just set a text to bold and type 0 to text
 We choose font size to 100 and bold text
 we align it  to centre horizontally and vertically.
 and we change the colour of the text to white.
 Now we will select the panel and add a component that will take care of the layer force. It's the component is under layout and is called horizontal layout group. For this game, we will set child alignment to middle centre, then we will uncheck child force expand for the width, and we will let this panel control the height of the  elements. And there you go, if you resize the panel, the text will adapt automatically. We are now all set for the coding part.

 

this we will add text
change the colours
rearrange the position



 



