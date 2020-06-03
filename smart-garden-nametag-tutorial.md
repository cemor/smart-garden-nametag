# Smart Garden Nametag

# Getting started
 
## Introduction @unplugged
Welcome! This tutorial will teach you how to use the micro:bit and this website, Makecode.
 
 
## Step 2 @unplugged
Take a look at the three columns on this screen. There's a simulator on the left, code blocks in the middle, and a workspace to do your coding on the right.

 
## Step 3 
We will start by using the basic blocks to program the LED lights on the front of your micro:bit. Together, these lights act kind of like a screen that you can display information and images on.

 
## Step 4
You have two blocks on your screen already, an``||basic:on start||`` block and a ``||basic:forever||`` block.
Let's explore how the ``||basic:on start||`` block works.
 
## Step 5: Give Your Garden a Name
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
Now let's try out the ``||basic:forever||`` block and add some pictures to the garden nametag . Select 2 or 3 icons from the basic category and place them in the forever block. Clicking on the arrow next to the icon will allow you to pick a different icon.

 
## Step 8
You can also make your own icon by adding the ``||basic:showLeds||`` block to your code. Give it a try!
 

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
 
## Step 9
These images are changing pretty fast. You can slow them down by adding a ``||basic.pause||`` block to your program in between each image block.



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
Now you're ready to download your code! Press the ``|Download|`` button to save the code to your computer.
Watch this youtube video to learn how to move the code from your computer to your micro:bit (Mike's youtube link or other helpful resource here)

