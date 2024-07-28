---
layout: post
title: "How to Automate Your Customer Support"
---

If you run a business and want to automate most of your customer support for cheap/DIY, follow these steps:

#### 1. Organize Your FAQs
Take your frequently asked questions (FAQs) and put them in a simple, easily editable location. For us, this means using a Google Sheet.

#### 2. Create a Contact Us Form
Develop a straightforward web form for users to contact you.

#### 3. Integrate with an LLM
Every time a user submits the web form, pull all of the FAQs into the context window of a large language model (LLM) and ask it to answer the user's question. We use Anthropic’s Sonnet model and manage around 100 FAQs.

#### 4. Automate Response Emails
Send the user an email with their question and the LLM-generated answer, provided the LLM's confidence level meets or exceeds a set threshold (for us, it's at least 90%).

#### 5. Provide a Follow-Up Option
At the bottom of the email, inform the user that they can reply to this email if they need further assistance, and someone from the team will review their query.

#### 6. Monitor and Update
Regularly monitor the emails sent by the LLM to ensure the responses are accurate. If the LLM provides incorrect answers, step in to respond to the customer personally and update the Google Sheet to improve future responses.

### 🤖

By following this approach, we have automated more than 90% of our customer support, costing only a few cents per inquiry. This method requires no expensive customer support software and involves minimal setup time.