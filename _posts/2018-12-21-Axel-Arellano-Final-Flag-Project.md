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
![Final-Flag](/images/final-flag.png)
* * *

## Describe your process.

-   What questions, strategies, help from peers or teacher, or thinking got you to this point? _then delete this instruction_

<!--- Delete this comment and add your writing -->


## Explain your code.

-   Choose a significant part of your program (15 lines max) and paste it below. Do not insert your entire program here. _then delete this instruction_
-   Explain each argument in the code section. _then delete this instruction_
-   Tell us how it functions independently and within the whole program _then delete this instruction_

* * *

```
Insert 10-15 line code section here _then delete this instruction_
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
