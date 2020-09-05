---
layout: post
title:      "What a wild, wild ride!"
date:       2020-09-05 17:09:16 -0400
permalink:  what_a_wild_wild_ride
---


[Deep breath.] 

Today, I finished coding my first Flatiron School project - the CLI Data Gem. It's a little program called Wildflower Events, and its job is to accept a search term, scrape the www.wildflower.org events page, and present details about related events. As my first foray into writing code that I imagined into being, it has definitely been a journey of discovery.

### Discovery of Self

Getting started with this project was pretty rough. Being a novice, I decided to start things off with a switch to a local environment. Due to some issues with the in-browser IDE, I lost close to two hours of code recently (even with my addiction to ctrl+S), and I wanted to prevent that from happening again. However, making the switch to the local environment was much more complicated than I expected. I am fortunate to have AMAZING tech support in my family, and that helped me to keep moving forward. Nonetheless, the change was destabilizing and made for a steeper learning curve. Motivation was low, but fortunately, tenacity filled in the gap.

I began to watch the [CLI Live Project Build videos](http://www.youtube.com/watch?v=KwBMwZ89Hj8&list=PLc6AmvC5Zybybc-NjUUwQwTtUEXH4iB2s&index=1), and I am so, so glad that I did. Even though my project has some different functionality, I learned a lot, including little details like the colorize gem. The recommended scraper tool is invaluable. Overall, just watching other people work through the creation process was quite reassuring.

As it turned out, I would watch a bit of the video and then try to reproduce the parts I needed by myself. The first challenge was really finding a good scraping candidate. It took quite a while (more than a couple hours) to find an idea that I was excited about and a correlated website that I could successfully scrape. I looked at the US patent site, govenment spending, local events, a newspaper website, CDC data on Lyme disease, housing websites... I felt like finding a good scraping candidate was half the battle. The good news is that I have a TON of ideas that I'm excited to pursue in the future.

These "just getting started" steps felt like they were taking an eternity, which surprised and unnerved me. Ultimately, I realized that I was going to need to adjust my expectations by giving myself permission to take it one step at a time. This is all still pretty new to me - six months ago, I had never written a program. Basically all of the concepts I used for this program were foreign to me up until pretty recently. So I intentionally began to celebrate small victories and new functionality, and as a result, I can sincerely say that I enjoyed the process of building this program.

### Discovery of Skills

Once I got the basic functionality of my program established, testing my code and addressing issues was pretty fun. For example, when I entered a search term but the website returned no results, I ended up with an argument error. I was able to track down where the issue was and develop some conditional logic that would present a message explaining the situation and wait for a new search term. Once that happened, the program was accepting a new search term but pausing and requiring an extra keypress of enter in order to proceed. That one took some consideration and a few fruitless internet searches. On a lark, I found that the addition of a conditional statement checking to see if the search results array was populated eliminated the need for a second keypress, and oh, there was much rejoicing.

Figuring out how to offer users an option to repeat a search felt like a win, too. I imagine that there are more elegant and concise ways to accomplish this, but I am feeling pretty good about the functionality.
```
puts "\nWould you like to search again? y/n"
repeat = gets.strip
if repeat == "y"
	WildflowerEvents::Event.all.clear
	call
else 
	exit
end		
```

I'm looking forward to the code review, because I expect that a more experienced set of eyes will have constructive criticism for me. I can definitely say that I am feeling more confident about getting classes to cooperate, calling methods from within other methods, and namespacing. All in all, it was a great opportunity to piece together so many different bits of what I have learned so far. It also helped me prove to myself that I can, in fact, create code that DOES things. One might say that there's evidence that my skills are ... blossoming. 
	


