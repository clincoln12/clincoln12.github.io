---
layout: post
title:      "MyMo. [A Subscription Tracking Rails Application]"
date:       2020-12-12 21:05:44 +0000
permalink:  mymo_a_subscription_tracking_rails_application
---


Well - that took me longer than expected.

2020 has brought a ton of challenge to many of us & I'm no exception to that. These past couple months have been a definite obstacle due to a variety of issues - but I'm proud to say that I've overcome everything that's been thrown my way.

Before I get into a basic breakdown of the application I just want to give a shoutout to Dustin for helping me solve my permissions errors that was plagueing the start of my project. TLDR: I couldn't edit/delete any files and in some cases start my rails server. After some mild confusion from both of us - he suggested moving my project directory to my labs directory. Problem solved - thank you Dustin!

## What I Learned...

**1) ActiveRecord Associations:** Although this was something that was covered thoroughly in the Rails curriculum - this wasn't something that I was strong with. 1 of the reasons that this project took me so long was that I originally wanted to do a Sports Betting application but there were far too many models & associations to make sense of so I ended up binning it and focusing on MyMo. Doing a project with only 4 models really gave me a clearer picture and allowed me to get past the initial planning phase.

Take your time to really think about your data structure/schema! You'll thank yourself later.

2) Rails Magic: The more you use the Rails - the more you love it. But with Rails magic comes great responsibility. I found myself looking up the 'What(s)' & the 'Why(s)' quite a bit because there's just so much that it does for you. I'm by no means a Rails expert after finishing this project - but getting stuck in a process like this with little to no help besides the internet really helps you grasp everything more than the labs. (Not a knock on the labs - I'm sure this is the intention of everything)

## The Application...

I wanted this to be a basic subscription tracking app where you could see how much $ is leaving your bank account every month (both /mo & /yr). Well upon reading project requirements I needed to include another model for nested resources - in comes payments. From a UX standpoint (and perhaps a securtity one) I don't think many people would want to include payments on their subscriptions but nonetheless - they're included!

Curious about what the app looks like? Here's the Repo:

https://github.com/clincoln12/MyMo/tree/master

## Final Thoughts...

While I'm a bit frustrated with how long it took me to finish this part of the curriculum - I'm satisfied with how much I've learned. But with that being said there's still a TON of room for improvement before I want to consider myself a capable Dev. Looking forward to the rest of the journey. Onto the next!

