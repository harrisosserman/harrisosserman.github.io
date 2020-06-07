---
layout: post
title: "My First Business Ever: KoalaCab"
---
During the summer after my freshman year at Duke, my friend and I started our first business.  I built my first website.  It was a taxi sharing and taxi booking website called KoalaCab (I know Uber now does this, but it was pre-Uber).  We ended up booking 450 cabs during our first year of operation.
![image](https://images.bloggi.co/84a0dc84.png)

Colleges are great places for taxi sharing because:
1. Students are price sensitive and want to spend as little as possible
2. Students are generally coming from/going to the same places (especially the airport before and after school breaks)
3. Students want to meet new people

This was our slogan and may have been the best part of the business:
![image](https://images.bloggi.co/0c6627cc.png)

**Building the Website**
At the end of freshman year, I had written very little code before, and had no idea how websites worked.  I saw a tutorial on Joomla called Website Essential Training, and it taught me the basics of how to build a website with PHP and MySQL.  Here is version 1 of the website:
![image](https://images.bloggi.co/a734da94.png)
I ended up using CodeIgniter, a PHP MVC framework, which helped with security (specifically SQL attacks) and code cleanliness.  I used JQuery Mobile for the KoalaCab mobile website.  In hindsight, building an app instead of a mobile website would have been the right decision, but I didn’t have the time to learn iOS/Android development.  

Final version before I killed off KoalaCab:
![image](https://images.bloggi.co/04fb0d05.png)

**Building the Business**
For KoalaCab to work, we would need to partner with a taxi company in the Duke area.  Riders would book rides through our system, the taxi company would drive the passenger, and we would take a cut.  We met with all the taxi companies in the Duke area to see what they would offer us.  All the taxi companies were willing to partner, some on better terms than others.  One company was willing to give my friend and me free rides for life (in hindsight, maybe we should have done that deal).  We vetted taxi companies on their tech capabilities, their management style, promptness, and reputation among Duke students.  We ultimately chose Charlene’s Safe Ride because they allowed students to pay with their FLEX school dollars.

**Learnings**
College students are very last minute, which is terrible for a web-based taxi sharing service.  It’s very hard to convince students to book a cab in advance.  The later the cab is requested, the harder it is for people to find out about the ride and join in.  When users came to our site, they were forced to first search for a cab with a similar itinerary before booking a cab.  If a cab was already doing a similar route, the user could join in.  If not, the user could create a new ride.  If everyone is searching/booking last minute, it is harder for people to truly cab share, and KoalaCab becomes more of a cab booking website for solo rides.    

And please don’t be in “stealth mode” while building your company.  Nobody wants to steal your idea.  Tell people about it, and have potential customers test it constantly.  