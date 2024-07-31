---
layout: post
title: "Earned Secrets"
---
For the last six years, I have been building Talk Hiring. Our goal has always been to improve the efficiency of the job training program (a.k.a workforce development program), job seeker, and employer triangle.

We started with automated mock interviews to enhance the efficiency of workforce development programs. Initially, we didn’t set out to build an automated mock interviewing tool, but we pivoted to that, and customers liked it a lot (we conduct ~35k automated mock interviews per year).

In the summer of 2021, we decided to reset and try something new to solve this problem.

I connected with five large employers and 15 well-respected job training programs in NYC. Workforce development programs hire a role called a job developer, who builds relationships with local employers and helps place job seekers into relevant jobs. To understand the challenges within this triangle of actors, I worked as a free job developer for these employers and workforce development programs.

Every week, I followed up with our employer partners and job seekers who had applied for these employer partners' jobs to gather intel on how candidates were progressing in their hiring processes. All this information was relayed to the workforce development programs.

However, this process revealed several key challenges:
- **Lack of Incentive for Status Updates**: Giving status updates to a workforce development program is not the job of either the employer or the job seeker. While it would be helpful, there is very little incentive for them to consistently share status updates.
- **Discrepancies in Progress Reporting**: Employers and job applicants often (about 1 in 3 times) disagreed on where the applicant was in the hiring process. Employers were more often correct about the candidate’s status.
- **Inconsistent Response Rates**: Both employers and job seekers were inconsistent in their response rates to status update requests, making it tough to pin down either party for updates.
- **Communication Gaps**: Employers would email job seekers, but job seekers frequently missed these emails. This issue stemmed from ATS emails ending up in spam and job seekers being overloaded with emails.

Ultimately, having spotty job search status data for a workforce development program is like running a sales organization with spotty CRM sales data: it just won't work that well.

I kept searching for a better way to track this data and realized that the job seeker’s email inbox was an underutilized system-of-record for identifying job search status. Almost the entire job search process sits in the job seeker’s inbox, from applications to job offers and everything in between.  Sure, it's a beast to structure this very unstructured data, but if we could do it, it would be very valuable.

We built a unique system to integrate into the job seeker’s inbox via a Gmail API integration. We parsed about 700k emails a day (~20 million emails per month) to identify job application-related emails. From there, we extracted information about the employer, job title, location, job status, and threaded the email into the relevant opportunity. We trained our own ML models using transfer learning and also leveraged OpenAI to achieve this. At our peak, we were parsing about 70k job application processes a month.

Job seekers are understandably hesitant to share their inbox with just anyone, so we integrated cash-back rewards. Job seekers could earn money for sharing this data, and we profited from the spread between what employers paid us to send traffic to their jobs and the cash back we paid to job seekers.  We also shared hiring insights with job seekers who connected their inbox, sort of a "Glassdoor 2.0" where job seekers could see which jobs had the highest/lowest interview rates, how long it took to hear back about a job on average, and which jobs we thought were ghost jobs.