---
layout: post
title: Alarm Clock iOS App
---
I share my bathroom with a roommate.  Nobody likes to wake up and find your roommate in the shower.  To solve this problem, I built an Alarm Clock app that shares my wake up time with my roommate.  That way, I can know when my roommate is planning on waking up, and I can set my wake up time accordingly. 

I use UILocalNotifications to do the wake up.  These notifications work great because an internet connection is not required for the notification to fire and I don’t need to manage running a background job.  To do authentication, I used Twitter’s Digits SDK, which works seamlessly for doing phone number based authentication.  Having an email address and password are not required to create an account on my app.  For all my database storage, I used Parse.  I did not want to manage a server for this small application.  

All of the source code is here: <a href='https://github.com/harrisosserman/AlarmClock'>https://github.com/harrisosserman/AlarmClock</a>.