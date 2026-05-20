---
layout: post
title: "Save the Date"
---

Over the holidays, a close friend was telling me about her dating life. She'd gone on a string of dates over the last few months. A few she thought went really well, but the other person never asked her out again. She had spent months going out, getting her hopes up, and walking away with no clarity about what was actually happening.

It reminded me of my own dating years ago. The dates themselves weren't the hard part. The hard part was how long the whole process took. Months of guessing. Months of replaying conversations through your own biases.

I started thinking about how lopsided the dating industry is. Hinge, Bumble, Tinder, the League. Basically every dollar in this space goes to the top of the funnel. Profile optimization, photo selection, bio crafting, matching algorithms. But once you're actually sitting across from someone? You walk away with only what you happened to pick up on.

That gap was the idea. What if you could get an outside perspective on a date you actually went on, not a coach reading your texts, not your friends speculating, but feedback grounded in what actually happened?

I called it [Save the Date](https://getsavethedate.com). The pitch was a mutual reflection system: both people opt in, both get their own private AI insights afterward, and the raw recording gets deleted. Nobody is reviewing their date's review. The product wasn't trying to gamify dating or turn it into a sport. It was trying to give you the one thing you can't get anywhere else, an outsider perspective on every date.

The innovation I was most excited about was the feedback format itself. Instead of a clinical "here's a summary of your date" report card, the insights came back as a Reddit-style thread. After every date, twelve different AI personas, each with their own voice and lens, would weigh in on what they observed. One persona is a no-nonsense friend who tells it to you straight. Another is the over-analyzer who pulls on a specific quote and unpacks it. Another is the romantic who sees the spark you missed. Another is the cynic. You scroll a thread of reactions the way you'd scroll a r/datingoverthirty post, except every comment is about you. The framing made the feedback feel like a group chat of friends instead of a verdict from an algorithm, and almost everyone I showed it to lit up at it.

I built the thing with Claude Code over a few months. React Native app, Supabase for the backend, AWS Lambda for the audio processing, Claude on the AI side. The hardest design problem was the consent flow. Both parties have to agree, in the app, before recording starts. The audio recording and the transcript both get deleted after the insights are generated. I obsessed over the privacy story because I knew that would be the thing people pushed back on.

Then I started doing user interviews. About 30 of them. Some were friends and friends-of-friends. The rest I recruited on [Prolific](https://www.prolific.com), people who had actually been on multiple dates in the last year. I'd share my screen, walk them through [the marketing site](https://getsavethedate.com), the app, the consent flow, the post-date insights, and just let them talk.

What I expected was that people would have a privacy reaction. They did. But it wasn't the privacy concern that mattered. The thing that came up in nearly every conversation, almost word for word, was:

> "I like it. But how do you ask the other person?"

It came up from Joseph, a nurse in Boston who said his big worry was "getting the other person to be ok with it." It came up from Emily in Portland, who said proposing recording "just feels awkward." It came up from Evan in LA, who told me point-blank that he'd love to be the recipient but would never be the asker. It came up from Alyssa in Austin, who would happily use it but didn't want her date to know.

Person after person told me the same thing. The product was interesting. The insights were exciting. They wanted to see what an AI thought of their date. But the act of sending a stranger a link and asking them to consent to being recorded? That was a wall.

So we iterated. We rewrote the marketing site to lead with trust and privacy. We added a "deletion receipt" that showed the user when their audio was destroyed. We added scripts, actual sample text messages, for how to ask your date, in three different tones (warm, casual, playful). We added a section on the site for how other people had handled the consent ask. We softened the colors. We added an AI personas page so people understood the feedback wasn't coming from real strangers. We tried, in every way we could, to lower the awkwardness floor of asking.

The biggest unlock came from listening to the interviewees. The same people who flinched at the idea of asking a stranger to be recorded would tell me, almost as a throwaway, "I'd be happy to use it on a second date." Joseph in Boston pitched me the line basically verbatim: "I had a great time, let's do it again soon. By the way, I would love to try this app on our next date. No hard feelings if not." That reframing changed the product. The consent ask doesn't belong before a first date when you barely know each other. It belongs at the end of a date that went well, when the goodwill is highest and the next date is the natural conversation. We rewrote the scripts, the marketing site, and the in-app prompts around that timing. The awkwardness floor dropped noticeably.

But solving the consent ask still left a harder problem behind it, and it was the one I noticed late.

Even when someone downloaded the app, there was no natural moment to remind them to use it. Most people don't have a date scheduled the day they hear about an app. They might have one in two weeks, or three, or not for a month. By the time the date came around, they had completely forgotten that Save the Date existed. I could send emails, push notifications, "any dates this week?" nags, but none of it felt good, and none of it solved the problem. The product needed to insert itself at exactly the right moment, and I had no way to know when that moment was.

The honest answer is that this product belongs inside a dating app, not outside one. The match itself is the right trigger. When two people match, the app already knows they're talking. It can read the conversation and notice the moment they start discussing meeting up. It can offer Save the Date as a one-tap double opt-in, before either of them has to type a single awkward sentence to a stranger. The friction disappears. The reminder problem disappears. Both people opted in to a dating app, so they're already on board with the premise of putting effort into dating. The consent ask becomes a feature, not a hurdle.

I'm not a dating app. I don't have those matches. And building a dating app to get to this feature is the long way around.

[Save the Date](https://getsavethedate.com), the only STD you will want to tell your friends about.
