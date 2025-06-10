# Linters for Thought

Joshua Levy\
*v0.1.0 (June 2025) – Draft!*

## Purpose

This is a rough draft I'm using to articulate a few ideas for research on the idea of
"linters for thought".
What that means, why it's important, and how we might make progress on it.

I'd love your feedback!
Fastest way is DMs: [x.com/ojoshe](https://x.com/ojoshe)

## Why We Should Talk about IA as Much as AI

In 1950, after reflecting for months on what mattered most, Doug Engelbart famously came
to three conclusions:

1. He would focus his career on making the world a better place

2. Serious efforts to make the world better would require harnessing collective human
   intellect to contribute to effective solutions

3. If you could dramatically improve how we do that, you'd be boosting every effort on
   the planet to solve important problems

75 years later, and more than 50 years after he invented the computer mouse and gave
[the Mother of All Demos](https://en.wikipedia.org/wiki/The_Mother_of_All_Demos), I
think his conclusions are still correct.

A key inspiration in my own career was meeting Doug in the 2000s, when I was a young
researcher at SRI. Another old mentor of mine, Adam Cheyer (also at SRI then, before he
started Siri) used to say: if you want to see the future of technology, you should look
to the past.

Today, billions are spent on the valuable and exciting work of training more powerful
models, including reasoning models.
But it is equally vital we spend more resources on helping *humans* think and act more
effectively—**intelligence augmentation (IA)** as Doug would call it.

In terms of software, the challenges for human reasoning may seem different today than
they were before the rise of LLMs.
But just as always, possibly the hardest part of being human is *working effectively
with other humans to solve human problems*.

I see so much focus today on the rising capabilities of AI systems—but vastly less on
*how* we can use LLMs and other tools to augment human thinking and collaboration.

Doug's vision is unchanged.
It's time we apply the tools of today with his vision in mind.

## Why We Need More Flexible Primitive Operations

> "Civilization advances by extending the number of important operations which we can
> perform without thinking about them."
> —Alfred North Whitehead

This is one of my favorite quotes.

If we wish for LLMs to improve human rationality and our ability to work together, we
need more tools that make complex tasks feel like easy steps.

That's why it makes sense to build tools that make individual steps more powerful, so
larger, human processes accelerate over time.

In software, big ideas often must be realized from practical, concrete pieces.

Typically there are two opposite pitfalls when building software:

- *Underengineering (inadequate up-front design)*: This is when you don't plan ahead and
  just building a tool, realizing it doesn't work as hoped, but then getting stuck
  because the complexity of the software is too high to change it.
  This too little design and too much technical debt.

- *Overengineering (too much up-front design)*: This is the opposite, which is that
  you're so afraid of inadquate design that you design a much more complex
  architecture—but then it ships too slow and it too might not work as hoped.
  This is too much design without testing and learning.
  This is common among engineers of moderate experience and was called by Fred Brooks
  [the second-system effect](https://en.wikipedia.org/wiki/Second-system_effect).

Unfortunately, for products like knowledge tools, the use cases are complex and not
obvious. So both of these are real risks.

So what do you do?

My answer is you should work "bottom up"—that is, you should build small pieces that
combine in many ways, including in ways you can't plan for right now.

If you can build small pieces that combine in many ways, the right combinations and
workflows become easier to discover.

A good analogy for this is the old story about planning paths on a college campus: you
can try to design them up front, or you can put down grass, wait for students to create
paths in the grass, then pave them.

## Why Linting is a Powerful Idea

### A Brief History of Linting

The power of incremental improvements is powerfully illustrated by the history of
software engineering.

Although historically, programming was seen as an arcane skill, over the history of
programming we've seen over and over that the challenges faced by software engineers are
really challenges we face in general in the knowledge economy—they are just happening
sooner, and more obviously for programmers.

The original *lint* was created in 1978 by Stephen C. Johnson at Bell Labs to flag bugs
and portability issues in C programs.
Modern linters parse code into abstract syntax trees and check it against predefined
rules. The idea was to catch bugs early before they manifest at runtime.

Now as it turned out, the validation of code is one of the hardest problems in software.
The past 40 years, this idea has slowly but consistently grown in maturity and in
importance for software development.

*Type systems* were another layer of validation for software.
The degree to which programmers should declare and enforce types has been a longstanding
source of debate.
Modern languages like TypeScript and Python offer type annotations that
reflect invariants about variables in code.
Type checkers catch whole classes of errors.

The development of tools like this let programmers build more complex things with fewer
errors.

It would be quite difficult to imagine building software of the complexity we have today
without the tooling like linters, type checkers, auto-formatters, and IDEs, that were
developed in the 1990s, 2000s, and 2010s.

### The Lesson of Linting

The key insight is this: *Remove the necessity to sort out trivial errors inessential to
the core problems at hand.*

This is partly an issue of catching typos or obvious bugs.
But the impact is more profound than that.

For complex and difficult problems, the scarcest resource is attention.
Linters (broadly speaking) make small and common errors not something you waste
attention on.

### The Value of Linting to LLMs

Today the rise of LLMs has made it possible to write code significantly more complex
applications. People who have never coded now realize they can build software.
And experienced engineers (myself included) are finding they can build certain things
much faster.

This has great benefits and some risks.
We don't need to get into them here.

But suddenly, prompts, tools, UIs, and frameworks to help LLMs get more reliable at
coding have become extremely valuable.

A key part of this is LLMs have been greatly enhanced in their ability to write better
code by the maturity of linters and type checkers.

In fact, perennial debates in Python and JavaScript ecosystem about the advisability of
using types have largely gone away suddenly, as people using Cursor and other AI tools
to code have realized types make LLMs far more reliable and better at coding accurately.

What was good for humans was great for LLMs.

## Can We Build Linters for Thought?

Now we are in the era of LLMs, it is an ideal time to revisit the idea of *linters for
thought*—that is, what are the tools that can help people iteratively improve the
quality of written ideas and consequently, of their ideas, both individually and when
collaborating?

I don't mean it quite literally, like finding grammar errors in whitepapers.

What I mean with this idea is that are there things that make small steps that do
powerful things easier, more rational, more effective at collaboration or at finding the
truth.

## How Do We Approach Building Better LLM Tools?

For certain hard problems, the devil is in the details.
Often we can have exactly the right idea but not work on it at the right time.
Or we might be at the right time but not be in an organization or with a team of the
right structure and incentives to have the outcome we want.

I'm fortunate to have worked at the intersection of knowledge tools, publishing,
reasoning systems, and engineering extensively.
Today, the rise of vibe coders, more powerful reasoning tools (like o3 and Gemini 2.5
Deep Research), and the return of classical formal reasoning tools for use with LLMs
(like [DeepSeek-Prover-V2](https://github.com/deepseek-ai/DeepSeek-Prover-V2)'s use of
Lean 4), makes it the perfect time for revisiting creative efforts in this area.

Of course, many large companies are working on related problems and making fast
progress, on their models and products, including OpenAI and Anthropic and various
startups.

But the approach I think makes sense is a bit different than what most startups are
doing right now. The three key differences:

1. Prioritize tools that *augment human ability* rather than just maximizing model
   performance

2. *Bottom-up development* of small, individually useful tools that are open source and
   composable so they can be combined in varied, unexpected ways

3. The tricky part: Innovate and experiment at all three layers:

   - the content layer (text editing and annotation workflows that encourage
     transparency, quality, and rigor)

   - the UX layer (going beyond chat and doc UIs to more flexible hybrids that are
     easier for unplanned workflows and cases, especially GUI/Terminal hybrid design)

   - the engineering layer (restructuring and repackaging typical messy full-stack web
     development in simpler ways so that simple apps are simple and for both humans and
     LLM coders)

This may sound ambitious but I want to be ruthlessly practical about it too.
See below for some concrete examples of what I've begun building.

## Experiments So Far

In software, big ideas often must be realized from practical, concrete pieces.
So often I like to work "bottom up".

Over the past couple months, I've found that because I can build more myself with LLM
coding tools, I have been able to prototype a few of these bottom-up tools.
These are just a start but they are pieces that build on each other:

All of these are rough and I haven't promoted any of them yet, but I'd like early
feedback if you're willing to share it.

- **Textpress:** A new platform for simple publishing of complex documents.
  You can publish or republish research reports for Gemini or OpenAI, PDFs or DOCX
  files, or other documents in a way that's easier to share and read, with good
  typography, mobile accessibility, clean footnotes, table of contents, annotations,
  etc. (This is in collaboration with another engineer, former YC founder and OpenAI
  engineer Kevin Lin.)

  Website: [textpress.md](https://textpress.md) (new!)

- **Leximetry:** An LLM-powered tool to measure *qualitative dimensions* of writing
  quality. Given a writing sample (or transcript) it summarizes metrics on 12 dimensions
  like clarity, coherence, sincerity, factuality, rigor, warmth, etc.

  Repo: [leximetry](https://github.com/jlevy/leximetry) (alpha!)

- **Deep Transcribe:** A tool for high-quality transcription of audio or video (such as
  YouTube videos) and then automatic editing, organization, analysis, and
  formatting/publishing.
  The output can be assessed with Leximetry, text can be fact checked with Kash Actions,
  and the result can be published on Textpress.

  Repo: [deep-transcribe](https://github.com/jlevy/deep-transcribe) (alpha!)

- **Kash:** The knowledge agent shell.
  This is a library and tool for experimentation.
  Think of it as a "command line for knowledge tasks".

  It lets you iterate and experiment with "Actions" like transcribing audio, converting
  documents, fact checking, annotating, and pretty much any other task possible with
  Python and LLM APIs, but interactively and each in a single command.
  Current actions that already work are conversion of PDFs to text, transcription of
  videos, captioning and annotating text, organizing and structuring transcripts, etc.

  It's currently terminal based (think like Claude Code).
  It also lets you chain together commands and assemble the outputs in topical
  workspaces (think a bit like Obsidian).
  The goal is this framework would be open source and let more people experiment and
  discover more powerful AI workflows.
  (It's also compatible with MCP.)

  Repo: [kash](https://github.com/jlevy/kash)
