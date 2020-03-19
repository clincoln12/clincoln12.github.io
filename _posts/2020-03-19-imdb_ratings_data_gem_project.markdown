---
layout: post
title:      "IMDB Ratings Data Gem Project"
date:       2020-03-19 17:54:21 +0000
permalink:  imdb_ratings_data_gem_project
---


This was the 1st time during the course where the training wheels are (almost) completely off and it's up to you to go and build something cool. While I was excited to have a crack at it - I knew this would be a somewhat daunting task. 

Here was the task: **Build a gem that showcases your acquired knowledge of Ruby. **

# Gem Description
As a movie nerd I wanted to build something that I would use moving forward. That's where the IMDB Ratings gem comes in. It starts by scraping all movie genres off of IMDB and allows the user to select which genre they're interested in watching. Upon selection - that specific genre's popular movie page is scraped, sorted and displayed to the user. The overall purpose is to display a list of the most popular AND best rated movies within that genre.

# What I Learned
1) **Collaborating Objects:** One of the most challenging parts of this project was collaborating classes/objects. At times it felt like a complicated web of code that constantly had me tracing my code back. Don't be afraid to do something a little different to make sure it all makes sense. Illustrate your code on a piece of paper to get a visual on how everything links up.
2) **Scraping:** When I read the scraping labs I was a bit lost and I think it had to do with still being a bit shaky when it comes to knowing what I was looking at in HTML. After gaining familiarity it didn't confuse me nearly as much - however, it was tricky to figure out what to do with the scraped 'href' links from each genre. This resulted in scraping the URL path in each genre (anchor) and storing it within each Genre upon instantiation. Later when I scrape the movies page the path is added in through interpolation for the full URL. 
Example: `imdb_url = "https://www.imdb.com#{genre.path}"`

# Wrapping Up
The 2 points above aren't the only things i learned/built on. They're just the 2 that I struggled with most during the project. This was a great way to touch on all of the Ruby elements taught in previous labs and bring it into 1 cummulative process. I feel quite a bit more confident in my coding abilities after conquering this. Still a lot of room to grow - but I'm excited for the journey.



