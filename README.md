# Ui-Arrangement
## Tutorial for putting an UI in a game
So you wolud like to have some UI in your game: a score number popping on your screen or maybe a timer?

This is the tutorial for you!
it can be used in a both 2D and a 3D project.

## Prerequisites

For this tutorial, I will be using a 3D project in Unity 2022.3.46f1. However, this can be applicable on 2D and any newer versions of Unity.
Since there will not be any programming in this tutorial, we will not need Microsoft Visual Studio.


## Setting up the User Interface

A UI is a very simple tool that helps the player interact with games' features and mechanics. By the help of a few clicks, your game can have a camera view based visual which will guide a player throughout the game.

The first thing we need to do is open a project (does not matter if it is 2D or 3D) an then go to the Hierarchy. Right click on the area and a drop menu should appear.
You will see an UI icon shown on that list. Press it and you will get another drop menu. There are various options we can choose from like Image, Text, ScrollBar and so on.
We will go to Panel and left click it.

After doingt these steps correctly, a scene will change. You should notice a Panel in your scene. In the Hierarchy, we can see that Panel is a child of a canvas.
Why can't Panel be by itself, and why does it have to be a child of the Canvas?
This is because it is makes it easier to place it in the scene without having to go to Game mode from time to time.


