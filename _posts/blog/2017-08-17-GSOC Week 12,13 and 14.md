---
layout: post
title: "GSoC 2017 - Week 12, 13 and 14"
categories: foss
excerpt:
tags: [Wikimedia, GSOC]
image:
  feature:
date: 2017-08-17 17:03:00 +05:30
share: true
---

### What I did

It's been a long time, since I have posted about the projects. I got busy with development, preparing for my placement interviews and submitting Camera ready paper submissions. With all of these tasks to take care about, I kept procrastinating the post :(

Finally, I got placed at Adobe System, India and submitted camera ready submission of my accepted research papers at International Conference on Pattern Recognition and Machine Intelligence 2017.

i18n know as internationalization, is the process of developing products in such a way that they can be localized for languages and cultures easily. i18n is an integral part of developing for MediaWiki extensions. So finally a stage came where my backend business logic required its own output label to the user. i18n requires the application to have message/label in all supported languages. So I began adding all the labels into en.json of i18n. Thank god, it was not my task to add translations of the message in all other supported languages. Fortunately, there are other people and automated bots that take care of this work. 

During this period there were several revisions of my patches due to multiple code review cycles. Some of the changes include renaming functions and variables, splitting the patches according to the functionality they serve, trying to serve corner cases. After rigorous testing and code review changes,  the code for drilldown feature got merged.

After this I to take some break due to all the work I just mentioned above. Phew. Thanks to my mentors.

After a one week break, I started working on adding support for creating hierarchy fields in CreateClass and CreateTemplate.
Using CreateClass page, I could not proceed further due to the false validation error. Validation did not work properly, even after providing Cargo Table name in the form, 'blank field' error was raised. I realized that it's a bug and thus submitted a patch.

I had named the core class of my contribution as CargoHierarchyTree at the beginning but later during the discussion, Yaron convinced me for a more abstract name CargoHierarchy. Now this week, after I inherited the class for another purpose, Yaron felt that it should be renamed backed to CargoHierarchyTree.


### What I learnt

Names are important! Correctly name things in code can save hours of debugging and can make understanding control flow easier.


### Tips to future myself (and anyone else reading this post)

![naming-important-hai-bhai](http://i.imgur.com/ksIVsui.jpg){:class="img-responsive"}

Yes, this is true. You need to spend some time naming important variables.
Never worry that changing something is too tough. It could be in some cases but it's not impossible either. Don't worry. Strive for a well readable and maintainable code.