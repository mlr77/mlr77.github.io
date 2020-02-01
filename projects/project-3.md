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

<div class="ui embed" data-source="youtube" data-id="m7jz075N9hU" >
</div>

# Intro to Java - Final Project

I wrote the Tetris Clone in Java using @Dlyan Kobayashi's EZ Graphics library. This was part of a team project and we decided build Tetris because it applied most of the concept learned in the Introduction to Java course, including one, two, and three-dimensional arrays, ArrayLists, and a number of other elementary concepts. We experimented with public and private settings and used examples from the course to help remove EZ elements, so the Tetris pieces could move freely without hogging too many resources.  

We designed the gameplay to be similar to the original game, with the following keyboard inputs: Enter to play, ESC to pause, left/right arrow to move, Q and E to rotate and SPACEBAR to drop the piece down faster. Also, we implemented a "Hold" function using boolean to hold a piece for future use by pressing the Shift Key. Lastly, there is a preview window which displays 5 "next" pieces, a simple clock to let you know how long the game has been played, as well as a scoreboard which resets if the game is lost. 

Working as a team was actually quite easy since Java supports building all classes in one file and then separating them later. It was not ideal, but it made it simple for us to share updates since we did not all have GitHub accounts at the time. We built different components and added comments in the source file accordingly. After building the code, we designed some images and downloaded some shared images to add the final touches. Lastly, we embedded audio to have matching background music. The music and backdrop changes at each level. 

The most complicated component of the project was working with the EZ Graphics library. It is meant to be easy, but since it overrides many of Java's built in methods, sometimes it became quite challenging to incorporate. For example, when you add a graphic to the screen, it is stored in an EZArrayList by default, which meant the only way to remove each piece was to track them individually, remove the corresponding piece from the list, and then garbage collection could finally take place. It was quite cumbersome, but it gave us an opportunity to learn to write code from scratch while working with existing code. 

Overall, this project, along with the other projects in the Intro to Java course gave us each an opportunity to apply our new skills. I felt quite happy with the end product, but there is always room for improvement. 


