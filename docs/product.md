# Product decisions

[한국어](product.ko.md) · [← README](../README.md)

The decisions that shape Wyldbyte, and why. Each one was made as the product owner, almost always after trying the first version and changing something.

## Who it's for

People with an idea for an app, a game or a tool who are not software engineers: solo founders, hobbyists, people who want to try something before spending money on it. They know what they want the product to do. They don't want to learn a code editor, and they don't have a product team to ask the right questions.

## Not "a coding tool made easier"

**Decision:** Wyldbyte doesn't show an IDE, code, terminals or ports. The person thinks about the product they're making; the engineering happens underneath and appears only when a choice is really theirs to make.

**Why:** tools that put a friendly face on a code editor still make the person think like an engineer. The questions a non-engineer can answer well are product questions: who is it for, what does it let them do, how will you know it works.

The journey follows how products are made in real practice, roughly **Discover → Imagine → Plan → Build → Accept → Grow**, broken into steps an AI guide can walk a person through one at a time. Some steps are never skipped, because only real people can answer them: research, the brief, testing the prototype, and learning from use.

## Byte asks; the person decides

**Decision:** the person acts like the CEO, and Byte acts like the team. Byte asks the questions needed to get the right input, and writes the best-practice document (the canvas, the research, the brief) on the right side of the screen.

- **One question at a time.** No "question 3 of 10" forms.
- **Several answers, one option at a time.** A question with several possible answers shows one option as a card: O to keep it, X to drop it, or own words. Options that exclude each other settle together.
- **Byte's pick is marked as a recommendation**, never chosen for the person.
- **Edits by hand count.** If the person changes the page themselves, Byte is told what changed before their next message.
- **Going back undoes Byte's work too.** Editing or retrying a message restores the page to how it was, but keeps what the person changed by hand.

## Said, guessed and found are kept apart

**Decision:** on every page, what the person said, what Byte inferred and what research supports are shown differently. A guess stays a guess until the person keeps it.

**A decision changed on the founder's own experience:** the first version asked the person what evidence they already had for each belief. I removed it the same day. Solo founders usually have none; research should find evidence for and against, not ask for it.

## Research that is real, or says it isn't

- **Beliefs are checked with sources.** Each belief the idea depends on ("learners would pay") gets a verdict (holds, doubtful, still unknown) and the sources that support it. A source is kept only if a search really returned it.
- **The most used competitors come from the stores.** The first version found only the closest products, one of them with a thousand downloads. Web search doesn't rank by popularity, so Wyldbyte now asks Google Play and the App Store directly for the most used apps in the category and shows their ratings and downloads, most popular first.
- **What people say is attached to what it is about.** Reviews sit under the product or belief they concern, summed up as likes and complaints with counts. If none are found, it says "No reviews found".
- **Try it yourself.** A competitor's page opens inside the app, beside the conversation, where the person can select or capture parts of it for Byte and mark the product Yes / Partly / No. Phone-only apps get a QR code.
- **Careful links.** Links to sites that haven't been checked are marked "Not verified" and asked about before opening.

## A one-page brief, then a feasibility check

**The brief** is one page: the problem, who it's for first, how it beats the closest competitor, the first version, and how you'll know it works. Byte proposes candidate features; whether each is in the first version is the person's call alone.

**The check came from a real mistake.** I once planned a website with an embedded browser and AI guidance hovering over other sites, and only learned late that a web page can't do that. So right after the brief there is now a check: for each thing the product needs, is it possible as a web page, a web page with a server, a phone app, a desktop app or a browser extension, with sources. Byte recommends a form and offers ways out; the person chooses. Whether *Wyldbyte* can build that form today is never the model's guess. It is read from the builder, and when the answer is no, the app says so instead of starting a build that can't succeed.

## Imagine before building

- **Ways.** Byte sketches a few genuinely different ways to make the idea, side by side. The person keeps one.
- **Imagine.** The chosen way is drawn screen by screen on a sketching canvas: draw, add shapes, connect a button to the screen it opens, test, refine, colour. A rough sketch is refined by AI into real, editable objects, never a flat generated picture.
- **Prototype.** The refined screens become one small playable web page. The person tries it, saves the file and gives it to testers; what testers did is noted before deciding to make it, change the prototype or change the idea.

The founder's feedback on the first Imagine layout ("too much like a property editor") led to a rebuild from the founder's own mockup: the canvas as the main focus, conceptual instead of low-level.

## Plan and build in the person's words

- **The plan is a list of what the product lets people do**, with where it runs, what it keeps, who uses it and what it's for. No engineering tasks.
- **Each piece is built and tested on its own** by contained AI coding workers, and the person gets a plain-language test for it.
- **When the plan can't keep a promise, it asks.** If something agreed in the brief can't be done as planned, Byte says so and offers the alternative; the person keeps the original or accepts the change.

## Design rules

- **No explanatory text in the interface.** No hints, how-to lines or captions explaining controls: labels, actions, counts and states only.
- **Never look more complete than it is.** Every number is real, an honest empty state, or says the feature doesn't exist yet. An early audit found 22 made-up values across six panels of an older interface; that is why this rule exists.
- **Results appear as they arrive.** Research findings one at a time, a drawing that draws itself line by line, reviews loading behind each product.
- **One-press delete, with a 30-day bin.** No double confirmations; a deleted project can be put back.

## Things I decided *not* to build (yet)

- Building phone apps, desktop apps or browser extensions from an idea: today Wyldbyte builds web pages and says so for the rest.
- Launch and "Grow" (measuring and learning from real use): named in the journey, not yet specified.
- A cheaper image model as a fallback: images use the best available model only, or none.
