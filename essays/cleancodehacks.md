---
layout: essay
type: essay
title: Clean Up Your Code!
# All dates must be YYYY-MM-DD format!
date: 2020-02-13
labels:
  - Software Engineering
  - ESLint
  - IntelliJ
  - JavaScript
  - Underscore.js
---

If you have ever taken a typing test, you will quickly realize a mistyped character decreases the typing "speed" dramatically. For example, if you do not correct your mistake, the program usually will dock time, and if you take the time to hit backspace and correct your mistake, or worse, use the mouse to fix a mistake, it will cost you loads of time. With only one minute on the clock in most cases, you may see your score drop from 60 words per minute (wpm) to 40 wpm. I once had to take a typing test for a job and I recall practicing over and over to type perfectly, rather than fixating on the actual speed of my typing. What is actually happening here? Are you getting faster at typing? Not necessarily, but avoiding uncessary mistakes will certainly save time and in the end will produce not only a better score, but correct results. The point of a typing test is not to see how quickly your fingers move, afterall. 

Implementing coding standards with ESLint in IntelliJ is similar. Enforcing coding standards with these tools is a great way to practice getting things right the first time. Reducing workflow costs through coding standards and keyboard shortcuts saves time and allows for more efficient programming. 

<h4>Within seconds, using a few of IntelliJ's shortcut keys (option-Return, then choose fix file), code can go from looking like this: </h4>

<img class="ui small right floated rounded image" src="../images/messyroom.png">

```js
function countOccurrences1(str)
{
  var counts = {};
  for (var i=0;i<str.length;i++)
  {
    var char=str.charAt(i)
    if(counts[char])
    {
      counts[char]++
    }else{counts[char] = 1}
  }return counts;
}
```

<h4>...to this (accepted by ESLint but one bracket still appears off):</h4>

```js
function countOccurrences1(str) {
  const counts = {};
  for (let i = 0; i < str.length; i++) {
    const char = str.charAt(i);
    if (counts[char]) {
      counts[char]++;
    } else { counts[char] = 1; }
  } return counts;
}
```

<h4>...and finally one manual touch-up: </h4>

```js
function countOccurrences1(str) {
  const counts = {};
  for (let i = 0; i < str.length; i++) {
    const char = str.charAt(i);
    if (counts[char]) {
      counts[char]++;
    } else {
      counts[char] = 1;
    }
  } return counts;
}
```

<h4>Even better, write the code using the underscore.js library and it begins like this:</h4>

```js
function countOccurrences2(str) {
  return _.countBy(str);
}
```
<h4>And since there are no problems, ESLint is happy.</h4>

<h4>Both functions produce identical output!</h4>

My coding style was riddled with spacing issues, misplaced brackets, and missing semi-colons. Although the functions ran the same, they were difficult to read, especially if you are used to a certain style. I found that after writing just a few simple functions, I began to prefer the new style and immediately adjusted accordingly. Without some type of standard, the code becomes messy and unreadable, and worse yet, prone to errors. Therefore, I fully support using linters such as ESLint, Integrated Development Environments (IDEs) such as IntelliJ, and for better, more concise and readable code, Underscore.js. Most importantly, these tools can and will help improve coding speed. Unfortunately, they cannot help with writing. Happy coding...
