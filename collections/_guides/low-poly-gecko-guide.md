---
layout: guide
title: How to Make Melee Run with Lower Poly Character Models
---

# How to Make Melee Run with Lower Poly Character Models

This is a code to make Melee run with lower poly player characters, thus slightly reducing the strain on your computer if you’re running a weak computer.

1\. Right click your vanilla iso

2\. Select Properties

3\. Click “Edit Config” in the bottom left corner of the properties window. This will open up GALE01.ini

4\. Make sure you copy and paste this text, so that your GALE01.ini looks like this:

![codes in the GALE01.ini file](/images/guides/perf-2.png)  

$Low-Poly v2 [UnclePunch,Yakult]  
C20748DC 0000000E  
3A26FA14 89D10007  
2C0E0009 41820010  
2C0E0017 4182001C  
48000014 89D10619  
2C0E0001 40820008  
48000008 38800000  
7C8F2378 7DDF782E  
39EF0004 7E1F782E  
7C0E8000 41820024  
7C8F2378 7DDF782E  
39EF000C 7DDF792E  
39EFFFF8 7DDF782E  
39EFFFFC 7DDF792E  
7C1F202E 00000000

5\. File > save.

6\. Close GALE01.ini

7\. Click on “Gecko Codes” in the top middle of the properties window.

![Gecko Codes tab](/images/guides/perf-3.png)

8\. Make sure it’s checked on.

9\. Press close.

10\. Start Melee, should be low poly now!
