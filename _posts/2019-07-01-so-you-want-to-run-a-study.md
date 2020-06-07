---
layout: post
title: "So you want to run a study?"
---
We ran a study to measure if using the <a href='https://talkhiring.com'>Talk Hiring</a> mock interviewing tool improves interviewing skills, and we have proven that it does!  Here’s a <a href='https://docs.google.com/document/u/1/d/1sqLllYxWRr9UV6WQd86SKwz5zGVY26utCNLHx2mSqaI/edit?usp=sharing'>link to our study setup and results</a>.  Running this study was much harder than I thought it would be.  Here are my learnings for others who might want to run their own study!  
![image](https://images.bloggi.co/35a4d682.png)
**Why did we run a study?**  
Our product helps job seekers become better at interviewing.  To make a claim like that, we wanted to back it up with data.  First we thought, why not measure hiring outcomes?  There are too many confounding variables to measure hiring outcomes from people who use or do not use our tool; plus, it would take much longer to prove or disprove.  Then we thought, can we use our existing interview data to measure interviewing improvement?  Users practice with over 100 different interview questions across different industries.  It’s hard to compare interview quality across different questions, let alone across different industries.  We decided to run a study so that we could control variables and prove the worth of our mock interviewing product. 
![image](https://images.bloggi.co/4fb4adff.png)
**Recruiting Participants:**  
As the operator of a self-funded startup, I initially tried to run the study without paying participants.  <a href='https://talkhiring.com'>Talk Hiring</a> works with workforce development organizations mostly in NYC, and I tried to recruit participants through those organizations.  We were able to recruit a few people through those channels, but the study would have dragged on for months if we had continued down that path.  I tried running free mock interviews with people, and using those interviews as data points in the study, but that was taking up so much of my time with lots of people canceling/rescheduling.  I finally decided to recruit for the study via a $10 Craigslist posting and through my existing Talk Hiring user base.

**A Note about Craigslist:**  
If your participants can complete the task remotely, always set the location of your Craigslist task to a major metropolitan location.  We had people from all over America completing our study because they were searching for paid studies in Manhattan.  
![image](https://images.bloggi.co/608c0cd1.png)
**Money:** 
I paid every study participant $5 via PayPal.  Even for that relatively small sum of money, people really needed the money.  I tried to pay everyone at the end of each day, but I got pushback.  A few people told me that they were planning on using my $5 for lunch that day.  Others would email me in all caps right after they completed the study, asking when they would get paid.  Some told me that they never received the money, and I had to screenshot my PayPal receipt to show them that they had been paid.  Interacting with so many people who needed my meager $5 was disheartening.
![image](https://images.bloggi.co/325c4280.png)
**Choosing the Right Significance Test:** 
There are lots of statistical tests of significance, and it has been 10 years since my high school stats class.  I did more than my fair share of Googling to figure out how to structure our study and which significance test to use.  Initially, my plan was to use a one-sided z-test to measure if a participant’s interviewing scores improved by using the tool.  Once the study was underway, I realized that it was not possible to accurately score interviews on a 1-5 scale.  Instead, I decided to measure simply if a participant’s 3rd try at an interview question was an improvement over their 1st try, defaulting to “no improvement” if it wasn’t clear.  I ended up using a single proportion t-test to measure statistical significance.
![image](https://images.bloggi.co/3b30c370.png)
**Unexpected benefits:**  24 people participated in our study.  Out of the 24 participants, 2 people sent me their resumes for employment opportunities, and 4 people told me that they would spread the word about our mock interviewing tool!  

A special shoutout to <a href='https://www.linkedin.com/in/joycecahoon/'>Joyce Cahoon</a> and <a href='https://www.linkedin.com/in/sam-waters-644a5a28/'>Sam Waters</a> for sanity checking all of my statistics in this study!  