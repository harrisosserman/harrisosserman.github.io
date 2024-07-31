---
layout: post
title: "Building Virtuous Product Loops: The Hire Rewards Journey"
---
All great consumer products need positive feedback loops, where events that happen via the product reinforce further usage of the product. Here’s how we built this kind of a virtuous, positive feedback loop within Hire Rewards.

## The Challenge

Hire Rewards was struggling. We had a promise that users loved: earn cash back while you job search. However, skepticism was high. Many people feared it was a scam, a fear heightened by the fact that our users were mostly low/moderate-income Americans who are often targeted by scams. Many users shared vivid stories of being scammed, reinforcing their wariness.

To succeed, we had to perfect the core dynamic: earning rewards as you applied for jobs. There was no room for doubt.

## The Core Dynamic

It was easy to explain to users that applying to a job would earn them money. However, the key was ensuring they received their rewards immediately upon application. Instant gratification was essential for a product like this.

### Initial Attempts

Initially, we validated job applications via a Gmail integration. The problem was timing. We couldn’t predict how quickly after hitting submit the potential employer would send the automated “thank you for your application” email. Our educated guesses weren’t enough; telling users when they might get paid would lead to failure.

Next, we tried using webhooks—requests that our server would receive when someone applied for a job. These worked well but weren’t universally supported by all employers, leaving us with only a partial solution.

## The Breakthrough

Our breakthrough came from an unexpected source: Ibotta, a popular grocery cash-back app. Ibotta requires users to take pictures of their receipts to ensure they bought the products they expect to earn cash back for. This receipt mechanism is used when Ibotta lacks a direct relationship with the grocery store’s cash registers.

With advancements in optical character recognition and text parsing from images, we realized we could employ a similar process. After users applied for a job, they could take a screenshot of the “thank you for applying” webpage, return to Hire Rewards, and upload the screenshot. We used a combination of automation and anti-fraud systems to verify that the screenshot was a legitimate job submission*.

## The Positive Feedback Loop

This new screenshot process solved our core problem and created a virtuous loop. The user would go from our app to the employer’s job application webpage, fill it out, and then return to our app to earn their cash back. Once they uploaded a successful screenshot, the money was added to their account immediately.

After uploading a successful screenshot, the user was back in our app, with extra cash back in their balance, validated that the app was legitimate, and ready to jump into another job application. The average user applied to 9.45 jobs, far above the job board industry average of about 1 job submission per user.

## Conclusion

By creating a seamless and immediate reward system, we built a positive feedback loop that not only reinforced the legitimacy of Hire Rewards but also encouraged repeated usage. This approach turned skeptical users into active participants, significantly boosting our engagement, job search outcomes, and profitability.

---

*If you’re interested in learning more about how we built our automation and anti-fraud systems, feel free to reach out!*