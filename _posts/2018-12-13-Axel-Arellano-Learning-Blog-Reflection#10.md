---
layout: post
title: Axel Arellano Learning Blog Reflection #10
date: 2018-12-13
---
  This week we were working on our new flag project. I am not done with my flag, but I am pretty close. I found a lot of things challenging, but one of the most challenging things I had to do was make both the white rectangles equal distance, also I kept  making one rectangle appear, but than my other rectangle would disappear. 
  This is my code:
  
```
include image
size = 200
width = size * 3
height = size * 2

RR = rectangle(width, height, "solid", "red")
WR = rectangle(width * 5, height / 5, "solid", "white")
RRWR = place-image(WR, width / 5, height / 5, RR)
BT = triangle(width / 1.55, "solid", "blue")
BTR = rotate(150, BT)
place-image(BTR, 175, 200,place-image(WR, 500, 300, place-image(WR, 500, 100, RR)))
```
The outcome is part of the puerto rican flag, except the triangle is not yet rotated and I haven't placed a star yet, this is the outcome of the code:

![Flag.image](/images/Flag.png)
