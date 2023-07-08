---
layout: page
title: AutoMute
description: A smart home concept for disabled people
img: assets/img/AutoMute.png
importance: 3
category: fun
---

This project was a proof of concept type work done to demonstrate the feasibility of a smart home system for disabled people. Smart home systems have become very prevalent in the modern society. Almost everyone has some form of smart home systems at their homes nowadays, thanks to cheaper networking hardware and the abstractions that many smart home vendors like Nest have introduced which makes it easy for end users to set up and use. Another factor that makes it popular are smart speakers. They usually have some form of virtual assitants built-in whom you can beckon to do anything within it's powers. Main points of interactions with these systems are human inputs through smartphones and voice inputs taken by smart speakers.

This fact made me wonder, what if a mute person wants to turn on the lights at their home? This one thought was the motivation for this entire project. Here I'm proposing the use of deep learning vision models to identify some key features that maps to certain actions that can be performed in a smart home system. In this particular implementation I used numbers shown via fingers and mapped it to different actions.

# Implementation

### Counting Fingers

My first approach was to use VGG16 and take the count directly from a video feed. But I quickly realized how inefficent and ineffective that approach was. So I moved onto using Mediapipe instead. With mediapipe I kept track of different parts of the hand and then used these coordinates and write logic to find out which number was being represented based on these coordinates. Each number was mapped to an action, for instance showing 1 turned on the lights if it was off and vice-versa. 2 was wired to turn the fan on and off and so on. However, using finger gestures may not be the best approach in all instances, different approached may need to be explored based on diffrent use-cases.

### Circuit

The Mediapipe app was run on a computer with decent specs. An ESP-8266 was used at the other end connected to a relay to control the appliances

**Pictures and videos coming soon!**