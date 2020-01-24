---
layout: project
type: project
image: images/tetris_img.png
title: Tetris Clone
permalink: projects/tetrisclone
# All dates must be YYYY-MM-DD format!
date: 2019-04-30
labels:
  - Java
  - Eclipse
  - EZGraphics
  - GitHub
summary: A Tetris clone developed for ICS 111, Intro to Java.
---

[![Tetris Clone ICS 111](https://github.com/mlr77/mlr77.github.io/blob/master/images/tetris2_img.png)](https://www.youtube.com/watch?v=m7jz075N9hU&feature=youtu.be "Video Title")

# Intro to Java - Final Project

This was our team's final project, a Tetris Clone written in Java using EZ Graphics(@Dylan Kobayashi) using 1-3D arrays, arrayLists, etc. The classes included are Config.class, Tetris.class, and Main.class. We worked together mostly on debugging in one file and then separated the classes. We experimented with public and private settings, and used the ICS 111 Bubble example to help remove EZ elements so the Tetris pieces could move freely without hogging too many resources. 

Keyboard keys are, Enter to play, ESC to pause, left/right arrow to move, Q and E to rotate and SPACEBAR to drop the piece down faster. Also, we implemented a "Hold" function using boolean to hold a piece for future use by pressing the Shift Key. Lastly, there is a preview window which displays 5 next pieces, a simple clock to let you know how long the game has been played, as well as a scoreboard which resets if the game is lost. 

The speeds increase commensurate the levels and background music/pictures change when the levels change. The game speed and how many lines it takes to switch levels can be configured int he Config.class.
