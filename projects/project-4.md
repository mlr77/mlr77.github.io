---
layout: project
type: project
image: images/landing-intro-featured.png
title: Dorm Room Cook Meteor App
permalink: projects/dormroomcook
# All dates must be YYYY-MM-DD format!
date: 2020-05-14
labels:
  - Javascript
  - IntelliJ IDEA
  - Meteor
  - Semantic UI React
  - GitHub
summary: A Food-based app designed to connect UH Manoa students and local markets through food. 
---

<img class="ui image medium rectangle" src="../images/landing-intro-featured.png" alt="">

# Dorm Room Cooks
- [View Documentation](https://dorm-room-cook.github.io/)

Dorm Room Cooks can be used by University of Hawaii students to find recipes to simple but delicious meals that can be cooked in a dorm room microwave or a small apartment with few tools.

### Team Building

Our team did not quite make it past the first stage of [Tuckman's](https://en.wikipedia.org/wiki/Tuckman%27s_stages_of_group_development) Stage's of Group Development, but we still managed to knock out a pretty powerful web application in a short amount of time. Due to the COVID-19 pandemic, several members of the team may have been isolated and without internet access. Despite the setbacks, we tried our best to adhere to the Issue driven project management (IDPM) guidelines by building tasks in Github, having each member assigned to a task at all times with one in reserve, and by using branches to keep each issue isolated until it was ready for prime time. This proved to be quite effective as it helped prevent problems with merging. 

### Application Concept

During our team's first (and only) "live" virtual meeting, each person provided thoughts on what the app should do and gave suggestions for addon-on features. The initial concept included user/vendor/admin access and associated management, a method for storing and retrieving recipes, a few design ideas such as what approach to take when allowing user access, and we also assigned some roles to each team member. The major goal seemed to be, "keep it simple and add features later." I agreed with this idea for the most part but also felt it can be difficult to backtrack, so it might be a good idea to at least build with the mindset we may add something later.

### Template Choice

Unfortunately, in a rush to get the site started, I chose to start building off the "My-Meteor-Template." This was a bad choice for two reasons. The template was outdated which led to wasting some time trying to update dependencies, and the template did not include profiles to get us started. If I could do it all over, I would have started with the Bowfolios template as it was the most robust template and would have led to a more successful starting point.

### Database Structure

To some extent, this is a silly topic since MongoDB is a NoSQL database and uses key-value stores, meaning, it does not really need to be structured. It is not a relational database in that sense so you can throw in whatever data you may have, and as long as you give it a name you are able to retrieve the info later. In fact, you do not even have to give it a name since each item will be associated with some type of id key. Regardless, designing the structure of the recipes and which fields should be mandatory or optional took a healthy amount of time. 

### Default Data Choice

Ultimately, our database included much more information than ever used, but it was a good idea to include the extra info because if we decided to add a feature or display information we did not have, it definitely would be a pain to individually add again. I think we made a huge mistake by trying to hunt down recipes on the internet. Also, I did not provide clear instructions one the types of recipes from which to choose. After creating nearly 60 recipes, I quickly realized most did not adhere to the objective of the app. Many recipes took more than an hour to make or needed an oven. This should have been a relatively simple task, but it did not work out well. In the future, I recommend just pulling up a dataset from Google's dataset [search](https://datasetsearch.research.google.com/) and downloading a .json file that already contains default data. That said, it was a great learning opportunity to see what can go wrong. 

### Application Design and Layout

There was quite a bit of confusion in regard to the design of the application. I suspect the primary reason behind this was in large part due to the breakdown in communication. It is difficult to come to a consensus on the designs or issues that needed to be carried out if people are not unreachable. In an ideal situation, members can ping ideas off one another during meetings and develop a solid strategy. Instead, I ended up testing out various designs and ideas with poor results. 

Later, I began to reach outside of the team to get reviews on various themes and ended up redesigning the theme and layout several times based on their feedback. A common complaint was my use of a gradient background on the landing page. I still prefer it, but the application is not just for me. Another decision I made was to keep the design responsive in order to reach a broader user base. Outside of the Computer Science department, many students may not have daily access to a computer, but most students have a smartphone nowadays. I used two browser windows at all times when designing, one to test the "mobile" version and one with a wider viewing area to test the browser version. After merging the changes, I then redeployed the app on Galaxy Meteor to run a live test on my phone.

After testing on my phone, there were several design flaws that did not initially appear in the shrunk down browser window. I made a note of those issues and quickly fixed them locally. One aspect I had not considered was the page that displayed "All Recipes" included all 50+ recipe cards, and on the phone it quickly became obnoxious to scroll back to the top. I ended up adding a small arrow button fixed to the lower right-hand-corner. That way the user can tap the button and be auto-scrolled to the top of the page.

One thing I learned about the design is it can, and should, wait until the end, but similarly to the database, some foresight is necessary to ensure the final changes do not take too much time or prevent the site from functioning properly. One useful trick is to assign a class to each item's className field and setup documentation in the css file for this. Later, if you want to change the style for any component it is easy to modify at one time. Another thing I've learned is to keep things simple. Having too many font types, or different colors can be distracting.

Lastly, we did not do enough research early on. As I began designing the recipe cards, I searched other websites for ideas. There are many great recipe sites out there filled with useful ideas on how to display the info, including which information to display, and it is a great opportunity to have first-hand experience testing user interface without building the interface first. Obviously, some websites are more user-friendly than others. We can certainly learn from others' mistakes and should not reinvent the wheel. A mass of advertisements was a common distraction amongst most online recipe apps. Thankfully, we did not have that problem. One student who tested the site suggested the "reviews" section was a great place to introduce [native advertising](https://www.wordstream.com/blog/ws/2014/07/07/native-advertising-examples) if that was ever needed.

### Testing

Continuous testing is a vital step in building an application. Any change made to the theme, especially via css had the potential to affect other areas of the site. One immediate benefit of running the Meteor application locally while updating the code is the changes appear in near real time. The only caveat is that sometimes you need to manually run through each page and nav-menu option to ensure they all still work properly. For example, there was one time when I changed the background and suddenly the titles were no longer visible. 

### Writing the Code

Documentation is key to every successful application. I had the React documentation opened in several browser windows at all times to quickly find code snippets or search for ways to implement a feature. Unfortunately, our team spent very little time adding documentation within the code, myself included. Failing to document changes can quickly lead to chaos down the road. This step is something seared into us as students but seems to be one of the most neglected tasks. We even discussed the need for better documentation but due to time constraints, and the fact we were mostly working individually we did not add much. Other than that, I felt writing the code was not too bad. There were a couple features that were difficult to implement using Semantic UI React such as the magic scroll or whatever it's called, but once I found out it is a Chrome built-in feature it was easy to incorporate. Also, the Search feature seemed tricky at first but another classmate led me to discover [fusejs](https://fusejs.io/examples.html#weighted-search) and implementing the Search quickly became a non-issue.

Please feel free to browse the "Dorm Room Cook" [documentation](https://dorm-room-cook.github.io/), and the [code](https://github.com/dorm-room-cook/dorm-room-cook) to your heart's content.