---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of _Puerto Rico_ by _Axel Arellano_

## Describe your program

 The country I designed for is Puerto Rico, the grade I think I deserve is a 3. The reason I would give myself that grade is because I put in a lot of work 

## Current output

* * *
![Final-Flag](/images/Final-flag.png)
* * *

## Describe your process.

 Making this flag was a lot of hard work because making the rectangles the same distance from each other was hard. Making the flag equal proportion based on the ratio was hard. I had a lot of questions like, how do I make the proprtions correctly? How can I add fractions to my old flag to make the sides equal?. My teacher helped me write the fractions, he also helped me with the white rectangles.  


## Explain your code.

Below there is a part of code from my flag, the first part will function as a image placer. The name of the code is stripes, the name helps because we can later use the name instead of the whole code, the program knows that when you type stripes you are reffering to the code that went along with it. The function itself is both of the place-image line's, the basic function of what they do is they place the white rectangles onto the base rectangle(the red rectangle), it place's both of the white rectangles on top of the red base. Alone the code can not function, it needs the entire program to give the name's, WR(whiterectangle), and RR(redrectangle) value. As a whole, with the entire flag code, the place-image function will place the image of a red rectangle with two white rectangles onto it. The second part, both overlay lines, add a rotated triangle and a star onto stripes(the first part)
* * *

```
stripes = 
  place-image(WR, width / 2, 0.3 * height, 
    place-image(WR, width / 2, 0.7  * height, RR))
    

BTS = overlay-xy(BTR, 0, 0, stripes)
WSBT = overlay-xy(WS, -30, -65, BTS)
```

* * *

-   Explain the code you posted by telling us about each argument.
-   Then tell us how your code section fits into the whole.
 
<!--- Delete this comment and add your writing -->


## Program code

```
include image

size = 100
width = size * 3
height = size * 2

stripe-height = 1/5 * height


RR = rectangle(width, height, "solid", "red")

WR = rectangle(width, height / 5, "solid", "white")

RRWR = place-image(WR, width / 5, height / 5, RR)

BT = triangle(height, "solid", "blue")

BTR = rotate(30, BT)
WS = star(width / 8, "solid", "white")

stripes = 
  place-image(WR, width / 2, 0.3 * height, 
    place-image(WR, width / 2, 0.7  * height, RR))
    

BTS = overlay-xy(BTR, 0, 0, stripes)
WSBT = overlay-xy(WS, -30, -65, BTS)
```
