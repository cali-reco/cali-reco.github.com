---
title: Architecture
layout: default
---
The **CALI** library was developed to be platform independent. Actually there are two versions, one for Linux and another for MS Windows.

![Blocos](/images/blocos.jpg)

The figure above shows the main blocks of the recognizer as well as the blocks to develop on the application side. One of the blocks, on the application side, is responsible for collecting the individual points of the strokes, while the other is responsible for receive and manipulate the gestures returned by the recognizer. The code developed on the application side is machine dependent.

The first block of the recognizer receives the sketch from the application and computes the geometric features for it. The second identifies the correct gesture or gestures based on the values computed before. The recognized gestures are inserted in a list order by degree of certainty, and returned to the application.