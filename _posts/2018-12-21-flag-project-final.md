---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of _insert your country_ by _insert your name_

## Describe your program

-  I designed the United Kingdom flag
-   Honestly i expect a pretty high grade because i used alot of defining and your able to make my flag by simply writing a word

## Current output

-   Insert an image that your program currently produces. _then delete this instruction_

* * *
![Flag](/images/final-flag.png)
* * *

## Describe your process.

-  Honestly define really help me without define i wouldnt have been able to make the flag but my biggiest struglle was probably when i made a vertical line on top of all of the base and the diagonal lines but i did know what to do after that and then i thought of something what if i put a define over this (overlay vertical-cross left-cross-right-cross-base)) add then i overlay and with the horizontal line and it actually worked (define flag-without-horizontal-line(overlay vertical-cross left-cross-right-cross-base)) Coding really invovles alot of thinking i've been realizing that little by little it is really advanded but it may take time but its worth it because theres so much you could do with it.


## Explain your code.

define width 300)
(define height 200)
(define width-white-on-red 400)
(define stripe-width (* 1/5 height))
(define red-stripe-width (* 2/6 stripe-width))
(define stripe
  (rectangle width-white-on-red stripe-width "solid" "white"))
(define red-stripe (rectangle width-white-on-red red-stripe-width "solid" "red"))



* * *

```First i had to make a define for the base of the flag the background so i did the height and the the width but the reason i did that was because i'd be able to use it over if i ever needed to and since my flag goes down to the ends in with and height it proved pretty useful but then Me and Mr. Alatta were thinking after that i tried making the diagonal line but instead of doing the red line and white lines separate and making it harder we just thought that we should put them together and we put the white stipe 1/5 of the hieght and the red stripe 2/6 of the white stripe but there are 2 ways we could of done that we could of did overlay as well  then once i defined them i put them together to put the lines together.

* * *





* * *


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

 
