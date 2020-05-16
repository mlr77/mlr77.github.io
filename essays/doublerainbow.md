---
layout: essay
type: essay
title: Double Rainbow
# All dates must be YYYY-MM-DD format!
date: 2020-05-14
labels:
  - Software Engineering
  - Learning
summary: Adventures in discovering Software Engineering.
---

## [What does this mean?](https://www.youtube.com/embed/OQSNhk5ICTI?start=75&end=79)

To be honest, only recently did I begin to discover the differences between Computer Science, IT, Software Engineering, Computer Engineering, Programmer, Software Developer, etc. Let me rephrase that, I, like many others, never gave it much thought. Yes, I included IT in the mix. Sadly, I was working in a different career and to me the titles were perfectly synonymous with one another. In fact, they do all overlap to some extent and in any of those professions you probably will never be too far from a computer.

So where does Software Engineering fit in to the puzzle? Are they the ones glued to the keyboard hacking away at code all day to push out an app? Do they do more than just write code? What is it that makes them any different from someone developing web apps as a hobby? How is it that Software Developers can even call themselves Engineers in the first place? I am no expert in the matter, but I believe the answer lies in all the extras. Nowadays, anyone can build an app. There are many people without so much as a high school education that can put together a solid web application, or possibly write code better than many people calling themselves Software Engineers.

It's important to note that in many states it is illegal to use the title Engineer without being a licenced Engineer, but let's ignore that for now. In order to provide a better sense of the term, here is a list of some (not even close to all) of the topics taught during the entry level Software Engineering course at UH Manoa:

- Open Source Software Development
- Configuration Management
- Functional Programming
- Development Environments
- Coding Standards
- User Interface Frameworks
- Agile Project Management
- Design Patterns
- Ethics in Software Engineering

A few keywords, such as standards, ethics, project management, stand out in my mind, and I feel it is those terms that begin to distinguish what it means to be a Software Engineer.

## Whoa-ho-ho

When I signed up for Software Engineering I thought it would be mostly centered on writing code. I was aware there would be some technical essay writing required, but after seeing previous students' work, I did not think it would be too much work. The student profiles consisted of a few highlighted projects, and a handful of essays, and I mistakenly believed that was the end product for the entire course. [Whoa](https://www.youtube.com/embed/OQSNhk5ICTI?start=31&end=40) ... was I wrong. It turned out to be just the tip of the Iceberg. Learning JavaScript and functional programming was just a small component of the course, and the essay requirements more than doubled what was displayed at the end. Fortunately, it is all designed in a step-by-step process to build each student from the ground up, similar to building an application. This is, after all, an engineering course, and software engineering goes way beyond simply programming.

## That's too much

Have you ever come across a task that is so large it is difficult to know where to begin? Or once you do get started it is hard to manage and easy to lose track of where you're at. Finally, once finished, it may be all wrong, and you have to start over. It's just [too much](https://www.youtube.com/embed/OQSNhk5ICTI?start=176&end=184). That's where Agile Project Management (APM) comes in. Instead of focusing on one huge task, such as building an application from start to finish, APM allows us to break down large projects into smaller, more manageable chucks. This allows software developers to quickly, and continuously turn around completed sections of the application which can be vetted and any flaws can be promptly fixed. It allows the client or end-user to be a part of the process and can lead to a better overall product, often saving time and money. I previously worked as an instructional designer and occasionally worked on a project from start to finish with little or no input from the end-user. Once completed, it would either be incorporated into the existing curriculum or scrapped entirely. If I had incorporated some APM strategies it certainly would have saved a ton of time. Imagine building a bridge and not continuously testing it throughout the build process?

## Oh my god

Many years ago I began dabbling in PHP and worked with a small team building a Content Management System for the DoD. None of the dev team had any credentials and mostly it was an ever-changing sidebar project that wound up getting deployed at several DoD schools. If any true software engineer saw the code they probably would cry in disbelief, shouting "[Oh my god!](https://www.youtube.com/embed/OQSNhk5ICTI?start=159&end=162)" Not because it was pristine code, quite the opposite in fact. Since each of us was learning to write code as we went, there was no such thing as coding standards, except for one aspect. 

The original author decided to use variables that were all somehow related to Harry Potter books. If you did not read the Harry Potter books then it would have been pretty difficult to make sense of anything. For example, the admin test account username was something like "Professor Dumbledore." I cannot remember most of the rest, but I do recall running across one line of code that appeared on every page. It was named, "sentinel." I asked what that was about, and it turned out to be the author's way to assign protected paths. Basically, sentinel would just check the user's role and if it did not line up then you are rerouted to another page. It worked, but security through obfuscation is not the best practice. More importantly, it made it very difficult for anyone else to work on the project. That was not the only problem however, coding styles varied from page to page. 

Since everyone just searched the internet to find snippets of code that seemed to work, many pages did not even have the same format. I don't think anyone on the team had ever heard of linters before. In Software Engineering class we gained hands on experience using ESLint and in my C programming class we used a linter written in Python to scan our code before turning it in. A linter basically scans code for all sorts of possible errors, from poor formatting to flat out improper use of syntax. There are so many great reasons to use a linter. For starters, when everything is consistent it is much easier to spot inconsistencies. When writing code, the most frustrating thing is to spend hours rewriting the code over and over, only to realize a comma or semicolon was missing. Nowadays, IDEs handle most of the work checking for syntax errors, but even inconsistent coding styles can lead to unnecessary frustration.

Standards, seems like the hallmark of an engineer to me.

## It's so intense

Software engineering can feel pretty [intense](https://www.youtube.com/embed/OQSNhk5ICTI?start=192&end=194) at times. It may involve many long hours of scrambling to hammer out the next task or meet the Milestone deadline, but it is amazing what one can accomplish if given the right set of tools. In our class we used the IntelliJ IDEA Integrated Development Environment (IDE) and Semantic UI framework. Despite my initial reservations, I discovered Semantic UI with React (a JavaScript library) to be fairly reliable after getting past the learning curve. Ironically, after learning the specific terminology and methods to customize components, it became fairly easy to incorporate new ideas into our existing application. Learning a new framework might feel overwhelming at first, but it is well worth the trouble because it just adds to your set of tools going forward, and it's almost like picking up a new language. The more you learn, the easier it is to learn the next. 

Every engineer has a handbag of tools in his or her arsenal and is able to choose the right tool for the right job.

## Ethics...

I attended boarding school as a child and during the process of choosing the right school, there was one feature I always examined more closely, rules. Most schools had a relatively normal set of rules, but occasionally there were really oddball rules. For example, a boarding school in Arizona had a line in their rulebook that said, "Must not pass objects through the windows." Another school's dress code stated, "No kilts allowed." The military dress code even specifies what types of undergarments airmen must wear. While I do not live by the motto "rules are meant to be broken," I do think it is interesting why they exist in the first place. They often appear as the result of some problem that occurred enough times to need a rule to fix it. Engineers adhere to many rules, but also have their own set of [principles](https://ethics.acm.org/code-of-ethics/software-engineering-code/). Principles differ in that they are not brought about by some external mandate, but actually come from within. I am not a huge fan of rules, but having principles is admirable. Software Engineers, like traditional engineers have a tremendous responsibility to ensure every aspect of the program is flawless and free from causing harm. 

Ultimately, being able to write code or develop an app does necessarily warrant the title Software Engineer, just as being a person does not inherently qualify you as a good person. Practicing standards, upholding key principles, managing projects effectively, taking responsibility, and ensuring software [integrity](http://physics.princeton.edu/~steinh/CargoCult.pdf) are a few of the key elements of true software engineers.

~RIP [Paul Vasquez](https://www.nytimes.com/2020/05/12/style/double-rainbow-paul-vasquez-dead.html) - Shame on you Coronavirus.