---
layout: post
title:      "Cook's Assistant - Sinatra Project"
date:       2020-07-19 18:14:05 +0000
permalink:  cooks_assistant_-_sinatra_project
---


Hitting my 2nd project in this curriculum hit me with a couple of emotions. The excitement of getting to build a more "full stack" application was met by the feeling of "oh crap - am I ready for this?"

Needless to say I was fully aware of the week of grinding that was ahead of me. But ready to take on the challenge I was.

## What I Learned

1) **Return Values Matter:** Okay - this is totally something I should have paid more attention to earlier in the course. Because if I did I could have easily saved an hour or 2 of my life. However, sometimes this is how you learn the most important lessons. So why am I talking about this?

Multiple times throughout my Controllers it was important to be able to find a User or a Recipe by an ID. What I didn't realize is that if a Recipe ID or User ID didn't exist - there would be different return values depending on the method. Example:

```Recipe.find(params[:id]) => returns the Recipe if it exists BUT raises an exception if it doesn't
Recipe.find_by_id(params[:id]) => returns the Recipe if it exists BUT returns nil if it doesn't```

This allowed me to redirect Users to an 'OOPS' page if the Recipe ever returned nil. No more broken pages!

2) **HTML/ERB/CSS Debugging:** This was possibly the most tedious part of the project. Waiting to add CSS until after everything was functional helped - but AFTER I added it things became a bit harder to read for me. Possibly because VSCode does not support ERB from a formatting standpoint. So the color coding is awful and causes some easy errors. For anybody who uses VSCode might want to take the time to download an ERB Beautifier so you can avoid that. 

But other than that there would be some issues that arised from trying to write my own HTML/CSS while using the Corneal gem (which is fantastic by the way). If you're going to use it - take a minute to understand how it works (I didn't take the time until I was getting random overflow issues haha). That way if you have an "unexplainable" issue regarding your HTML - you will know to debug the Corneal files as well.

## Final Thoughts

This was a great project to not only recap the previous lessons but to give you a taste of what it's like to build a more complete application. My biggest take away is to be a bit smarter with debugging. If something is an issue - I need to do a little bit less sitting around and thinking what it could be & more DOING. Onto the next!




