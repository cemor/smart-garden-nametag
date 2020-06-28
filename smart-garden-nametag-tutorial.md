# Name your Garden with micro:bit

# Getting started
 
## Introduction @unplugged
Welcome! This tutorial will teach you how to use the micro:bit and this website, Makecode.
 
 
## Step 2 @unplugged
Take a look at the three columns on this screen. There's a simulator on the left, code blocks in the middle, and a workspace to do your coding on the right.

 
## Step 3 
We will start by using the basic blocks to program the LED lights on the front of your micro:bit. Together, these lights act kind of like a screen that you can display information and images on.

 
## Step 4
You have two blocks on your screen already, an``||basic:on start||`` block and a ``||basic:forever||`` block.
Any code inside of the ``||basic:on start||`` block will run only one time, right when you turn on your micro:bit. 
Any code in the ``||basic:forever||`` block will run over and over again until you tell it, with code, to stop or until you unplug your micro:bit.
Let's explore how the ``||basic:on start||`` block works.


## Step 5
Click on the basic  category and then click on a  ``||basic:show string||`` block and drag it inside of the ``||basic:on start||`` block.
Let's change the text. Think of a fun name for your garden and type it in the ``||basic:show string||`` block.
Click on the lightbulb icon to the right for some helpful hints.

```blocks
basic.forever(function () {
    basic.showString("My Garden Name")
})
```


## Step 6
Take a look at the simulator on the left side of the screen. It should be showing your garden's name scrolling across the screen. The simulator lets you see what your code will do before you download it onto your micro:bit. Because you added this code to the ``||basic:on start||`` block, your garden's name will only scroll across the screen once when the micro:bit turns on.



## Step 7
Now let's try out the ``||basic:forever||`` block and add some pictures to the garden nametag . Click on the basic category, choose 2 or 3 of the ``||basic:showIcon||`` blocks and place them in the forever block. Clicking on the arrow next to the icon block will allow you to pick a different icon.

 
## Step 8
You can also make your own icon by adding the ``||basic:showLeds||`` block to your code. Give it a try! Make your own icon using the ``||basic:showLeds||`` block and place the icon in the ``||basic:forever||`` block.
 

```blocks
basic.forever(function () {
   basic.showIcon(IconNames.Heart)
   basic.showIcon(IconNames.Happy)
   basic.showIcon(IconNames.Ghost)
   basic.showLeds(`
       # . # . #
       . # # # .
       # # # # #
       . # # # .
       # . # . #
       `)
})
```
The dark blue squares in the ``||basic:showLeds||`` block each represent one of the LED lights on your micro:bit. Clicking on one of the squares will turn it white, which means that LED light will turn on. If the square is dark blue, it means that the LED light is off. 
 
## Step 9
These images are changing pretty fast. You can slow them down by adding a ``||basic.pause||`` block to your program in between each ``||basic:showLeds||`` or ``||basic:forever||`` block.



```blocks
basic.forever(function () {
   basic.showIcon(IconNames.Heart)
   basic.pause(100)
   basic.showIcon(IconNames.smallHeart)
   basic.pause(100)
   basic.showIcon(IconNames.Heart)
   basic.pause(100)
   basic.showIcon(IconNames.SmallHeart)
})
```
You can use icons to do cool things like create a heartbeat animation. Pretend this is your garden's heartbeat. What conditions might make your garden's heart beat faster because it's upset or excited? What might calm your garden down and lead to a slower heartbeat?


## Step 10
Now you're ready to download your code! Press the ``|Download|`` button to save the code to your micro:bit.
Visit this page to learn how to plug in your micro:bit and how to download your program to the micro:bit https://microbit.org/get-started/first-steps/set-up/ 

