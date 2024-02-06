---
title: "Calculator Art: How to create art on a TI-84"
date: 2024-02-04
---

# Calculator Art: How to create art on a TI-84

![Woah!](../../../assets/img/Capture1.png)

The first time I saw a calculator, it was one of the top 10 worst experiences of my life. I was a snot-nosed, fat kid in middle school, staring at a block of plastic with a dull gray-green screen in front of me. My teacher started off her introduction to the calculator with how to reset it:

> \> 2nd+712

> \> You'll be using this alot, as your calculator can be broken in so many ways

But that rocky introduction did not stop me from fostering an ever-growing love for my calcualtor. Nerd that I am, I went through thick and thin with this little guy. From Statistics, to Calculus, to Linear Algebra, matrices, derivatives, and Chi-Squared tests, I've enjoyed a long, prosperous journey with what I consider to be my true soulmate.

Now, you might be questioning my sanity when I say that this thing can create art. But what some of you may not know is that TI-84s can be programmed, and has drawing functionality. The image above was created with just _ lines of code

```
:0→X
:8→A
:.1→B
:While B<10
:0→X
:While X<2pi
:Line(Bcos(X+B),Bsin(X+B),Bcos(X+4pi/A+B),Bsin(X+4pi/A+B))
:X+2pi/A→X
:End
:B+.1→B
:End
```

__"Goodness gracious"__ you might say. You might *gasp* at the horrible variable names, and cringe at the use of ```while``` loops instead of ```for``` loops. But you have to understand the limited capacity of this device. I guarantee nobody at Texas Instruments was thinking about the lonely, bored kid in AP Chemistry, who really only uses his calculator for dimensional analyses, sitting there after an assignment or test, chugging away at his calculator, making __ART__.

To get back to the point, the program uses some easy-peasy while loops, and the basics of trigonometry: that sine and cosine are part of the unit circle. By using these basic principles, and some creativity, you can create things like this!

![A circle with some flair to it](../../../assets/img/Capture2.png) ![What some might call a hexagonal tesselation. Am I using that right?](../../../assets/img/Capture3.png) ![I don't even know what this is...](../../../assets/img/Capture4.png)

If any of y'all want the code for these, feel free to ask. But if you want to explore the wonderful world of programming art, let me know how it goes!

***

EDIT: In case you would like to replicate these images on YOUR TI-84, I now have all the .8xp program files [here](https://github.com/green60ninja/green60ninja.github.io/tree/main/assets/calcProg). Here's essentially how I made them.

I started out with a typical, run-of-the-mill, circle. Each program almost always goes from 0 to 2pi, drawing lines from one location to the location on the circle. If you fiddle around for enough time, and with enough patience, you can create interlocking, mesmerizing patterns. For example, if you want to draw a hexagon, you step every pi/3 (that is, 2pi divided into six subintervals) to have your six-pointed polygon. Or you can skip every other point to get a six-pointed star. Have fun with it!