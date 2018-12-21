---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of _insert your country_ by _insert your name_

## Describe your program

-   What country did you design for? _then delete this instruction_
-   What grade do you expect? _then delete this instruction_

<!--- Delete this comment and add your writing -->

## Current output

-   Insert an image that your program currently produces. _then delete this instruction_

* * *
![Flag](/images/final-flag.png)
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
Insert entire program here _then delete this instruction_
```
(define width 300)
(define height 200)
(define width-white-on-red 400)
(define stripe-width (* 1/5 height))
(define red-stripe-width (* 2/6 stripe-width))
(define stripe
  (rectangle width-white-on-red stripe-width "solid" "white"))
(define red-stripe (rectangle width-white-on-red red-stripe-width "solid" "red"))

(define red-on-white (overlay red-stripe stripe))



(define base (rectangle width height "solid" "blue"))


(define stage1 (put-image(rotate 35 red-on-white) 160 110 base))   



(define vertical-cross(overlay (rectangle 40 200 "solid" "red")
         (rectangle 70 200 "solid" "white")))



(define left-cross-right-cross-base(put-image(rotate -30 red-on-white) 160 110 stage1))

(define flag-without-horizontal-line(overlay vertical-cross left-cross-right-cross-base))

(define horizontal-cross(overlay (rectangle 300 50 "solid" "red")
         (rectangle 300 80 "solid" "white")))

(overlay horizontal-cross flag-without-horizontal-line)

 
