---
layout: post
title: "Book Club for One Side Project"
---
I love to read, but I am a terrible reader. What I mean by that is my reading comprehension is frustratingly mediocre. I’ll zone out mid-sentence, wonder “wait, who is this character again?” and months later, struggle to recall even the basic plot. Back in high school, I used to force myself to add a sticky note to every page or two with brief summaries of what I'd just read, ensuring I was paying attention and retaining the story. It worked surprisingly well, but the downside was that it made reading painstakingly slow and significantly less enjoyable.

My dad once explained studying to me like this: your brain fills with information like a bathtub fills with water. After the test, the stopper gets pulled, and you’re left with just droplets clinging to the sides. Those droplets are the bits of knowledge that stay with you long-term. It’s a vivid analogy—and painfully accurate.

If I’m investing many hours into a book, I certainly don't want to end up with just a little bathtub ring of knowledge clinging to the edges.  I want to learn deeply, be genuinely moved, inspired to introspect, or pushed to see the world differently. This is exactly why people join book clubs—they crave that deeper connection to what they've read.

But what if you could have your own “personal trainer” for reading—a book club designed just for you? Imagine an automated, asynchronous buddy, invisibly guiding you to comprehend, reflect deeply, remember clearly, and suggest your next read. I spent the last couple of months hacking away at this idea purely for fun, without any pressure about the business side. That made this project uniquely joyful.

I began by exploring OpenAI’s capabilities to build a GPT model that would take the name of the book and, for a given reading session, the pages you started and finished at as input. The model would then provide a concise summary, highlight deeper themes, and suggest potential follow-up questions for further inquiry—questions you could ask the model or explore on your own. This works because many books we read are fully available online, whether legally or not. The results were impressive! Check it out yourself [here](https://chatgpt.com/g/g-67f311b4406c819180ed13bc48ebf9fc-book-smart).

I knew this would not be a final product solution, but more of an experiment of OpenAI's capabilities.  GPT or text-based interactions are awkward solutions. Interrupting your reading to open a phone or computer and manually input pages or chapters breaks immersion and inevitably leads to users forgetting to log their progress.

Now that the backend was working well enough to prove that it could work, I started a multi-week design sprint, trying to figure out the right way to capture the start and end page of a reading session without it feeling clunky or annoying. I spent weeks prototyping and playing with ideas. Could it be a watch app that lets you scroll quickly to log your spot? A voice command? A smart bookmark with just enough tech in it, like [Mark](https://mark.engineering/)? A tiny camera that clips onto the book or your shirt or glasses? Maybe something that senses page turns and just knows? I kept cycling through form factors, searching for something that felt seamless and subtle—like having a quiet little helper who always remembered where you stopped reading.

The brilliance of [Granola](https://www.granola.ai/), the invisible note-taking app that's exploded in popularity, inspired me—it’s effortlessly unobtrusive, silently providing searchable notes and perfect recall of meetings without participant input. That ["set-it-and-forget-it"](https://www.youtube.com/watch?v=v-8G_yT4UGc) elegance was exactly what I was chasing.

Eventually, cameras emerged as the most compelling solution.
But if cameras were the answer, where should they be mounted? On a clippable book light? Attached via fish-eye lenses poking out from the book edges? Embedded in smart glasses or a wearable device clipped onto clothing?

After many brainstorming sessions with ChatGPT on form factor, I bought some Raspberry Pi gear to practically test different camera setups.
Once everything arrived, it quickly became clear: glasses were undeniably the superior form factor.
For a camera to accurately read an entire page, it must be a good distance away (about a foot).  Placing cameras at the page edge wouldn’t cut it, requiring cumbersome setups with dual cameras awkwardly jutting out—and even then, they wouldn’t consistently capture the full baseline or header needed to reliably identify the page number.

This week’s Google IO introduced the [Project Moohan smart glasses](https://www.theverge.com/hands-on/671077/project-moohan-android-xr-google-io-2025-smart-glasses-wearables), Google's answer to Meta's Ray Bans. These seem exactly what my idea needs. Though their release is uncertain, likely around 2026, I’ll eagerly track their SDK developments. This whole idea really hinges on a product like smart glasses with a powerful SDK—something that lets you build tightly integrated, low-friction tools on top of always-on hardware.

In the meantime, Amazon, could you please integrate this feature into Kindle? You already have the perfect dataset on reading start/stop points, making this product effortlessly seamless. I'd gladly build it if you released an API...

Until the next rabbit hole.