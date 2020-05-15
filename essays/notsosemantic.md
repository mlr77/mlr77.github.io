---
layout: essay
type: essay
title: The Not So Semantic Truth Behind Semantic UI
# All dates must be YYYY-MM-DD format!
date: 2020-02-27
labels:
  - Semantic UI
  - HTML
  - CSS
---


Often times we use the term "it's just semantics" when arguing a point both parties agree on, but the words used are just not quite the same. In this manner of speaking, I feel the concept of Semantic UI is a little misleading. The idea behind using Semantic UI is that one no longer needs to cope with the learning curve that comes with difficult syntax to build websites. I somewhat disagree. 

While Semantic UI offers a unique way to build a fairly nice looking website, relatively quickly, with very little css, but there is still plenty of overhead to building a really nice website. In order to better illustrate my frustrations with using Semantic UI, I will highlight a few roadblocks I ran into while cloning a landing page off the [Roblox](corp.roblox.com) website this week.

***
### Navigation Bar Formatting

The nav bar is generally very easy to build. I began by copying the Roblox logo (actually, I cheated and just hotlinked it). Then using Semantic UI, I built the following menu:
```html
<!-- Fixed navbar at the top with ROBLOX logo -->
<nav class='ui menu fixed borderless inverted'>
  <a class='item' href='#'>
    <img class='ui image tiny' src='url/logo.png'>
  </a>
  <a class='item' href='#'>Careers</a>
  <a class='item' href='#'>Technology</a>
  <a class='item' href='#'>Our People</a>
  <a class='item' href='#'>News</a>
</nav>
```

It seemed easy enough, especially since this is such a simple navigation menu; however, the orginal website had a nice feature that changed the text color on mouseover. The only solution to get the clone working similarly seemed to be to manually edit the css properties, but it was difficult to know what was controlling the css in this case. It took me hours to figure out how to remove the highlighting from the menu despite knowing the right words to use. I attempted, a:hover, .item:hover, .ui.item:hover, etc. I scoured the internet and finally found I was missing a space between .ui and .menu... This may seem like it's a css problem but since I was forced to use css regardless, I consider it a problem with Semantic UI.

Ultimately, I added the following css to get the nav bar looking proper:

```css
body {
  background-color: black;
  color: #fff;
}

/* adjust left margin of logo */
.ui.image.tiny {
  margin: 0 0 0 25px;
}

/* Force the black background menu */
.ui.menu {
  background-color: #000 !important;
}

/* Fix highlight for item and font hover */
.ui .item:hover {
  background: transparent !important;
  transition: cubic-bezier(0.1, 0.7, 1.0, 0.1);
  transition: color .5s;
  color: #009dff !important;
}
```
***
### Video Stream and Picture with Text Overlay

There really was not any great thing about using Semantic UI in terms of formatting, but it is not too bad to add a YouTube or Vimeo video. You can simply call the "ui embed" class and type in the source of the video along with a placeholder image. The problem is there is no easy way to stream the video. The folks who build Semantic UI assumed people do not want to land on a page and suddenly have a video streamed, so rather than just muting the sound, they opted to disallow streaming altogether. This works for some cases, but it made it impossible to clone the Roblox website. 

Later, I came up with a pretty decent alternative to the video stream. Instead of fighting with Semantic UI to get it to do what I wanted, I found a snippet provided by Jonathan Harrell on [Codepen.io](https://codepen.io/jonathanharrell/pen/vVEerg) that allowed for a text overlay to pop-up when hovering over the image. It offered extra effects such as dimming and changing the saturation of the background image to make the text stand out even more. When I tested it with the Roblox site I changed the colors to better fit the style of the website but it was a lot more fun to play around with the css than fiddle with Semantic UI. 

***
### GRIDLOCK!

I eventually managed to muddle through the steps of building an accordian dropdown text similar to what is seen on the Roblox website, and also embedded a couple videos (that would not preload), but I finally met my match when it came time to building the footer. That should be the easiest part of any website! It's just a couple columns of text. Truthfully, it could have been easy if I attempted a static web page, but I decided to try and make the website responsive and adjust the grid boxes as the screen size changed. After all, most people use a mobile device to play Roblox, or at least that's what my daughter uses. 

I looked up all the different ways to mess around with grids on the [Semantic UI](https://semantic-ui.com/collections/grid.html) website and tried for hours to get it working. I failed. One of the major drawbacks was I kept having to open the documentation to see what the "simple language" was supposed to be. For example, to resize something, you can use small, tiny, large, big, huge, whatever...but it's never easy to remember where you can use those and there is nothing to let you know if it's working correctly until you reload the page. I tried to make my padding massive, but apparently padding can only be "very padded." I tried to align my grids but sometimes I was supposed to use the word middle, and other times I needed the word center, or centered. It actually turned out to be a nightmare for me most of the time.

Between all the time spent figuring out the grid structure and which words to use where, I finally gave up on getting the columns looking just right. Maybe I will try again someday when I have more time.

This is a quote from the Semantic UI website:
>Concise HTML
Semantic UI treats words and classes as exchangeable concepts.
<br/>
<br/>
Classes use syntax from natural languages like noun/modifier relationships, word order, and plurality to link concepts intuitively.
<br/>
<br/>
>Get the same benefits as BEM or SMACSS, but without the tedium. 
 
Some of the discouragement may have been caused by fatigue, but I have used Twitter Bootstrap in the past, long before I had a clue (not that I am much better now), and I did not have many issues building sites with Bootstrap, or plain old HTML/CSS for that matter. Plus, what's with all the DIVs!? Seriously, the HTML5 [documentation](https://html.spec.whatwg.org/multipage/grouping-content.html#the-div-element) points out that we should use DIVs as a last resort. Maybe I just have a bad memory, or maybe my English is not up to par for Semantic UI, but in the end, I think there must be better solutions out there. 

The concept of using natural language to write code and build websites is great. I think a better approach might be tying documentation to codepen.io or a similar online tool. In a round-a-bout way, that was sort of what I ended up doing anyway. 

Maybe we can build an AI to assist in coming up with solutions rather than searching all over the internet. For example, I want to have two columns that remain fixed width on on the left and one column on the right, but when the screen size shrinks, the two columns on the left should jump to the middle, centered, and the right column should drop below them, also centered on the page. I should be able to search that entire sentence and the search tool can take me directly to codepen.io and provide the code needed to implement. While I am there, I can make some other adjustments and get exactly what I'm after, and then just port the snippet into my code with no issues. Ha, it sounds so lazy. But, isn't that why humans have come so far? We are so lazy that we work very hard to become even lazier.

Better yet, the computer should just read my mind and build the site based on what it thinks I want. We could train a neural network to scan website screen shots and figure out most of the code, and it can help draft the next couple posts for me as well. Do artificial intellectual property rights exist? I suppose some might argue that website designers would be upset, but we use AI to create art all the time and artists are still doing what they do...I think I've gone off topic so I will end this now.

