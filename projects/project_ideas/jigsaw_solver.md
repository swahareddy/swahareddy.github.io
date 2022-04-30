---
layout: project
title: Jigsaw puzzle assist
---

![](https://miro.medium.com/max/2000/1*fdeD2ntePx5R_aStXakYww.jpeg){: width="98%" }*

> An (mobile) app to help you solve a jigsaw puzzle. IN the larger 10000 piece type puzzles it is often frustrating to solve it half way and run out of enthusiasm or worse trying to determine how the 40 pieces representing the clear blue sky are supposed to correctly align.

## User experience:
1. You provide a photo of the image the puzzle's actual image.
2. You provide the *resolution* of the puzzle. i.e. Number of pieces (Eg - 50x30)
3. You provide a photo of a piece from that puzzle and the app will tell you where it should go (or top possible choices in case it's ambiguous).

## How we can accomplish this (technologically):
This has been tried before:
* Similar to what I thought of - [Cornell Tech](https://medium.com/cornell-tech/jigsolved-computer-vision-to-solve-jigsaw-puzzles-70b8ad8099e5)

> These guys have created a software to solve the puzzle [simply by looking at the pieces](https://www.abtosoftware.com/blog/computer-vision-powers-automatic-jigsaw-puzzle-solver) !! They do not need to know how the end state even looks like.
> ![](https://www.abtosoftware.com/assets/ezgif.com-optimize.gif){: width="20%"}*

* Handling the pieces themselves - 
  * [Towards Data Science](https://towardsdatascience.com/solving-jigsaw-puzzles-with-python-and-opencv-d775ba730660)
  * [CMU](https://www.andrew.cmu.edu/user/estherw/final/writeup.pdf)

## Challenges
1. An important part of this will be to have good quality images of the puzzle. (Similar brightness, glare, angle etc on both the puzzle picture and the piece you are looking to place). These are very practical concerns if you want a layperson to actually use your solution.
2. While we might be [matching](https://www.wikiwand.com/en/Scale-invariant_feature_transform) the piece based on the rectangular *resolution*, in reality the puzzle piece is *jigsawed*(i.e. has convex and concave parts) and hence can lead to false positives.
3. Browsing through large puzzles on Amazon, I just see *10000 pieces* printed on the boxes. Not *500x200 pieces*. In that case the user will need to tell me the dimensions (length and width) of the full puzzle (available on the box) and dimension of a single piece (will need to measure).


![](https://miro.medium.com/max/1150/1*nQZxgvOBWs-D8Ako17EI1Q.png){: width="15%"}*

*Images have been taken from the blogs referenced in this post.