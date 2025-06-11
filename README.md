# Linters for Thought

Joshua Levy\
*v0.1.2 (June 2025) – Draft!*

## Purpose

This is an incomplete and rough draft I'm using to articulate a few ideas for research
on the idea of "linters for thought."
It revisits some long-standing ideas of Engelbart and some thoughts of my own on how to
think about tools for augmenting human collective intelligence.

I walk through some underlying concepts on what augmentation is and why it's important,
the history and future of software engineering and its relation to human knowledge work,
and discuss we might design, discover, and build tools for augmenting our collective
ability to explore solutions to complex problems.

I'd love your feedback!
The fastest way is DMs: [x.com/ojoshe](https://x.com/ojoshe)

## Intelligence Augmentation

### Learning from History

In 1950, Doug Engelbart was 25, newly engaged, and realized he had no career plans.
After months of reflection, he famously came to three conclusions:[^engelbart]

1. He would focus his career on making the world a better place

2. Serious efforts to make the world better would require harnessing collective human
   intellect to contribute to effective solutions

3. If you could dramatically improve how we do that, you'd be boosting every effort on
   the planet to solve important problems

A key inspiration in my own career was meeting Doug in the 2000s, when I was a young
researcher at SRI.

75 years later, over 50 years after he invented the computer mouse and gave [the Mother
of All Demos](https://en.wikipedia.org/wiki/The_Mother_of_All_Demos), I think his
conclusions are still relevant.

### Why We Should Talk about IA (Not Just AI)

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

Another old mentor of mine, Adam Cheyer (who was also at SRI, before he built Siri),
used to tell me: if you want to see the future of technology, you should look to the
past.[^futurehistory]

Doug's vision never wavered, but in spite of the immense impact of his work on the
Internet, the GUI, the mouse, and almost every piece of software we use, he always
considered his dream unrealized.
It's time we apply the vastly more powerful tools of today with his insights in mind.

### Why Technological Shifts Happen First for Programmers

I want to take a significant detour in the next section through some core insights about
the challenges of building software.

This is for two reasons.
Firstly, if you look at the history of the Internet, you'll see many of the things that
most influenced online products and culture were first observed by programmers.
Although historically, programming was at first seen as an arcane skill, over the
history of programming, we have seen over and over that the challenges and insights of
programmers are usually challenges or insights we face in general with knowledge work.
If you want to see the future of the knowledge economy, look at what programmers are
excited about today.

Secondly, the rise of LLMs are making it possible for non-programmers to become
programmers, programmers to become designers, and roles to increasingly blur.
Along with this, the dichotomy between human language and code is blurring.

LLMs don't change the fundamentals of how humans interact with information.
But they are accelerating changes that have long been happening to an even more rapid
pace. These insights are increasingly relevant to writing, communication, and clear
thinking in a post-LLM world.

## Reflections on Software

### What Doesn't Change in Software?

Today, as AI is transforming software and the knowledge economy, famous technologists
are confidently making extreme predictions almost every day.

Does AI make work obsolete and eliminate all jobs?
Does it accelerate us toward multi-planetary techno-Utopia?
Or is your P(doom) so high you should liquidate your retirement portfolio?

In a world where software is more intelligent, what creates value and makes the world a
better place—and what averts possible disaster?

Predictions about large technology-driven changes are rarely reliable, even if they are
made by experts.

In technology, some things change fast—and some don't change at all.
The hard part is in knowing which parts are which.
However, as Jeff Bezos pointed out, you often can have more confidence in things that
don't change.

So let's look first at what *doesn't* change.

### What is Technology?

> “Technology is the solution to human problems, and we won’t run out of work till we
> run out of problems.”
> –Tim O'Reilly[^oreilly]

Many people today fear AI eliminates jobs.
And it's true many roles are changing or being eliminated.

As Tim O'Reilly explains, human problems are complex and evolving because human desires
are insatiable. And technology is the ever-evolving ways we find solutions to those
problems.

So even if many things are changing, we have one concept that doesn't change.

<div class="boxed-text">

***Technology** is the solution to human problems.*

</div>

### What is Software Engineering?

Another surprising thing today is how many programmers and tech leaders make quite
confused statements about programming and engineering.

Many seem to confuse software engineering with coding.
This is a bit like confusing writing with typing.
One currently involves the other, but it's a woeful misunderstanding to think the value
of a writer is their typing ability.

At the most essential level, software engineering is not writing code.

It is critical to realize, programming is not just implementing a specification—or
commanding an AI tool to build a solution.
It is an exploration of solutions.
Because not all human desires are logically or practically feasible.

Just for fun, let’s take a hypothetical example.

Imagine you had a near-magical piece of software, even better than current AI tools,
that instantly converts any user’s request to code with high fidelity and never
misunderstands them.

Say you give it to a bunch of users.
You know what you’d discover?
At first, they'll be delighted by simple things.
But once they start to do anything really complex, your *users* will begin to have
misunderstandings *with themselves* about what they want the software to do.

They’ll realize they asked it to do A and B but actually that implies C. And now they
look more closely, C is definitely not what they wanted.

So what would happen next?
The more clever or determined users would start *exploring* what they really wanted.
Changing B to D or adding a special case E, and so on.

You know what you’d call those determined, unusually analytical users who were good at
figuring out what they really wanted?

You guessed it: engineers.

So this brings us to a second definition that doesn't change:

<div class="boxed-text">

***Software engineering** is the precise exploration (by humans) of solutions (in
software) to human problems.*

</div>

### Why is Software Engineering Hard?

Another fundamental question is, why does it seem like software engineering is quite
hard, both for humans and now for LLMs?

I'd like to say the answer is simple, but it's not: the answer is *complexity*.

For better or worse, it's a fact that humans have varied and insatiable desires.
And our desires arise not just from our own needs or imagination, but out of what we see
others want.

And as a consequence, human problems are *complex* and *constantly evolving*.

So more often than not, the solutions are complex and constantly evolving.

That means *good* software engineering is the art of rapidly and effectively exploring
and building software solutions to human (or specifically customer) problems that are
complex and evolving.

<div class="boxed-text">

***Good engineering** is engineering that allows **sustained velocity** in exploring
solutions to human problems.*

</div>

You need to do it quickly but at the same time without getting bogged down by details
that aren't really relevant to the problem.

As one of the best engineers I know describes it, "good engineering is moving fast but
not painting yourself into a corner."

Another important way to frame this statement, originally due to Fred Brooks: good
engineering involves exploring the *essential* complexity of a problem and possible
solutions without adding too much *accidental*
complexity.[^nosilverbullet][^naturalcomplexity] Having too much accidental complexity
is a common way engineering becomes ineffective.[^techdebt]

<div class="boxed-text">

*The **hard part of engineering** is understanding and exploring **essential
complexity** while managing **accidental complexity**.*

</div>

This is true whether you're a human developer or an LLM. And it's one more thing that
*doesn't* change with progress in AI.

### Why Don't Apps Have the Features We Want?

So we now know one reason it's hard to be a good software engineer: because it's hard to
explore the essential complexity of problems.

It can be hard to understand what problems your user (or even you yourself) are really
solving, and it's hard to identify the essential parts of that problem.
And especially over time, it's hard to build and evolve solutions that aren't
constrained by accidental complexity.

We all know numerous situations where we want a software program to solve a problem we
have. But we know ChatGPT, Anthropic, Notion, Google Docs, Slack, Excel, and Zapier, and
dozens of other products don't quite solve it directly.

But often, we know what the solution is.
Why don't companies build the solution to your problem?

There are several reasons for this.
And they depend on the size of the team and some apply *even if people know the solution
and know how to build it*. It's worth being aware of the key ones:

1. *Lack of awareness*: They don't know your problem exists

2. *Lack of understanding*: They are aware of the problem but don't understand it
   properly (because they haven't talked to users or because they can't as a team
   describe or articulate it in a way that can be built)

3. *Lack of resources*: They understand the problem, but don't have the resources to
   properly design and build it

4. *Innovator's Dilemma*: They understand and have the resources, believe it is
   relatively less profitable than working on other products and features

5. *Conway's Law*: They understand the problem and resources and incentives to solve the
   problem, but still don't solve it (or solve it poorly or do something else).
   Many don't realize how common this is.
   The biggest reason many large, successful companies don't add specific features you
   want, even if they are obviously a good idea, is
   [Conway's Law](https://en.wikipedia.org/wiki/Conway%27s_law), the underrated but
   well-established rule that teams are constrained to produce products that mirror
   their organizational structure.

Looking at these reasons, we can see that for the most part, none of these fundamentally
go away with AI tools.

So while AI tools are changing software and even radically changing the jobs of people
building software, we will still always want things faster than developers, product
managers, designers, entrepreneurs, and companies design and ship solutions.

<div class="boxed-text">

*Even with perfect engineering, software and features are constrained by **human
communication**, **profit incentives**, and **organizational structure**.*

</div>

This too won't change.

## The Future of Software Development

Now we've talked about the essential facts that seem inherent to how and why humans
build software, it's time to ask what *is* changing?

### Is English the New Programming Language?

One of the most remarkable shifts in the last year or two is that more people are able
to code more complex things by using Cursor, GitHub Copilot, and other LLM coding tools.

It has become popular to say English[^english] is the new programming language.

This may be partly true, but of course applications are still actually committed to
GitHub and then deployed based on Python, TypeScript, Rust, SQL, and the other standard
programming languages.

So is English code? How should we even define code now?

### What is Code?

Before we talk about natural language coding and specifications, let's talk about code.
Oddly enough, just like there are common confusions about the true purpose of
engineering, there are also common confusions about the true purpose of code.

When learning to program, people tend to think of programming as communicating with the
computer. It can even be a fun challenge to do this in as direct a way as possible, such
as in C or assembly language.
Over time, engineers and programmers invariably move to to “higher-level” languages and
frameworks that are easier to write in.

But there is a key point even some experienced programmers forget: As systems evolve,
more time is spent reading, debugging, and changing the code than writing it.
In software engineering, the true goal of writing code is not to give the computer (or
more generally, the distributed system) commands, but to communicate to yourself and to
other engineers what the whole system should do.

As a side effect, you produce code that works (and, if you're good at it, also runs
efficiently). Compilers can be built for any language.
The history of the development of "better" programming languages is the history of
improving the languages to support communication *with people*.

The point is still that code is actually about communication between humans.

Now the ways we code are changing a lot with LLMs.
Much code is written or explained by LLMs to a human (vibe) coder.
So LLMs are like co-pilots for writing, sharing, and modifying code.

But with only a small addition we have a clear definition.

<div class="boxed-text">

***Code** is the communication format for humans (and LLMs) to express with **near-exact
precision** the behavior of software in a way humans (and LLMs) can understand.*

</div>

Aside from this broadening, this definition is the same as it would have been 20 years
ago.

Code is the medium to allow humans to perform the process of exploring solutions in a
completely precise (and ideally, practical) way.
That's why *effective workflows* around code, such as tests, commits, pull requests, and
code reviews, are so important.
They are what structure and manage the complexity of expressing and updating the current
description of the software's behavior.

### What is a Specification?

Traditionally, people thought of a specification as a natural language document (like a
product requirements doc or an API spec) that described what software should do *before*
code was written. The idea was that business analysts or architects would specify
behavior precisely enough that programmers could implement it correctly.

Famously, the waterfall approach to software development rarely worked in practice.
(At this point this should come as no surprise since we know it fundamentally hinders
the true process of engineering.)
Specifications were too vague, didn't reflect a correct solution, or were too detailed
to maintain as requirements evolved.

Documents are "dead" unless they are part of routine engineering workflows.
So over time, the "real" specification was often just the code itself.

Now vibe coders working with LLMs are rediscovering specifications, because of this
crucial difference. While imperfect, it's effortless to convert English to and from
programming languages.

The history of programming languages perfectly illustrates this convergence.
Assembly required developers to think like machines.
C abstracted away memory addresses.
Python reads more like pseudocode.
Each generation of languages moved closer to how humans think with precision about the
essential complexity of problems.

<div class="boxed-text">

***Specifications** are a communication format for humans (and LLMs) to express with
**acceptable precision** the behavior of software in a way humans (and LLMs) can
understand (more easily than code).*

</div>

Specifications and code have always both been different ways to express software
behavior in a way that helps human engineers communicate about it.

### Are LLMs the New Compilers?

Engineers are now writing more and software by using just English and natural-language
specifications and docs.
Developers of Claude Code now say most (perhaps even 90%) of Claude Code's own codebase
is now written in Claude Code.
This is a remarkable fact.

It's now tempting to say English is the new programming language, and LLMs are the new
compilers. (On Twitter, and you'll see similar statements almost every day.)

But this simply isn't the most insightful way to frame what is happening.

As we've seen, you can't get away from the fact that we have always needed rigor and
precision in expressing solutions to the essential parts of our problems.

Specs in English and code in Python are closely related.
They're both documents to help describe and explore software behavior.

But English specs and programming languages with formal semantics are not the same.
Precision of such descriptions in corner cases is of fundamental and unavoidable
importance for many of the use cases that matter most.[^nines] English in the form we
normally use it is far too ambiguous and imprecise to express the behavior of software
with full precision.
We can use English in *many* ways with LLMs, from writing poetry to brainstorming
software architecture.
Only some of these forms directly support engineering.

It's more accurate to say we are seeing three related but different changes:

1. We are using English with LLMs and LLM-powered agents to read, write, and test code
   more quickly than ever before

2. We are seeing the emergence of English documents as specifications that are critical
   parts of workflows, used by both humans and LLM agents

3. Because a single person can build and test software more quickly, they can rapidly
   make experiments and test and see if the software works or solves their problem

We're moving from a world where we had occasional, poorly used English specifications to
one where clear and precise English is essential to working efficiently with our tools
and teammates. And we'll work with this *and* traditional programming language code with
formal semantics.

LLMs are pushing us toward precise and structured ways of expressing software that are
more human friendly.
It's quite likely we'll see emergence of languages at new points between English and
current programming languages, or of rigorous, constrained formats for English
(themselves enforced by LLMs and grammar specifications).

### The Future of Knowledge Work

Does the history of software engineering really have relevance for us today for people
who are not engineers or builders of software?

I think it does. The most difficult problems we face, where our collective intelligence

A decade ago, the practice of writing software was so different from writing emails or
having meetings that it seemed like they were entirely different disciplines.

But if what we care about is working effectively together to explore solutions to human
problems with software, the approaches that work are *the same processes that work for
software*.

And now AI tools transform the nature of our work so code and language, writing and
spoken word, are increasingly interchangeable, the distinctions of the past are becoming
flimsy.

In short, if you believe all the points I've made so far, it's hard not to come to a
possibly surprising conclusion:

<div class="boxed-text">

***Effective knowledge work** and **effective software engineering** are increasingly
the same thing.*

</div>

This may be a bold statement, but I think it's worth entertaining and exploring its
implications.

## The Metaphor of Linting

> "When you make it harder to do the basic parts of an activity, the more advanced parts
> become almost impossible... Tools don't only make things easier: they allow us to
> augment ourselves to do things that were previously impossible..." —Doug
> Engelbart[^aug]

### A Brief History of Linting

The power of incremental improvements is powerfully illustrated by the history of
linting and type checking in software.

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

## Can We Build Tools for Collective Augmentation of Thought?

What are the tools that can help people iteratively improve the quality of written work
and consequently, of their ideas, both individually and when collaborating?

While linting is good metaphor, I don't mean it literally, like simply finding grammar
errors in whitepapers.

What I mean is we need to look for more reliable, small steps that makes meaningful
adjustments and improvements to content so it is better in different dimensions—clarity,
rationality, rigor, and so on.
By improving content along the right dimensions, and using these tools collaboratively,
so the judgement of many people is combined, it seems we can significantly improve the
quality, rigor, and real-world effectiveness of many ideas.

### What Will Improve Our Tools?

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

### Build More Flexible Primitive Operations

> “*Civilization advances by extending the number of important operations which we can
> perform without thinking about them.*” —Alfred North Whitehead[^whitehead]

This is one of my favorite quotes.

If we wish for LLMs to improve human rationality and our ability to work together, we
need more tools that make complex tasks feel like easy steps.

That's why it makes sense to build tools that make individual steps more powerful, so
larger, human processes accelerate over time.

In software, big ideas often must be realized from practical, concrete pieces.

Typically there are two opposite pitfalls when building software:

- *Under-engineering (inadequate up-front design)*: This is when you don't plan ahead
  and just building a tool, realizing it doesn't work as hoped, but then getting stuck
  because the complexity of the software is too high to change it.
  This too little design and too much technical debt.

- *Over-engineering (too much up-front design)*: This is the opposite, which is that
  you're so afraid of inadequate design that you design a much more complex
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

## A Few Tool Experiments (So Far)

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

* * *

## Notes
[^engelbart]: https://en.wikipedia.org/wiki/Douglas_Engelbart

[^futurehistory]: In fact, this is true for many fields.

    I think the reason is that in newer but rapidly growing domains—such as physics or
    math in the early 20th century, or computer science and software engineering over
    the past 60 years—when a field is young, it is small enough for a few early
    visionaries to deeply understand the whole field.

    This lets them see further ahead than even brilliant people decades later, because
    the field has become so large that no human can truly grasp it all deeply.

[^oreilly]: https://www.oreilly.com/tim/wtf-book.html

[^nosilverbullet]: Frederick P. Brooks, [*No Silver Bullet—Essence and Accident in
    Software
    Engineering*](https://worrydream.com/refs/Brooks_1986_-_No_Silver_Bullet.pdf), 1986.

[^naturalcomplexity]: It's worth noting essential complexity comes in two forms.

    If you are building an airplane, you need a good understanding of aerodynamics and
    materials science, which are governed by quite complex interactions of the laws of
    physics. This is *natural complexity*.

    On the other hand, if you are building a messaging platform, you will discover your
    users (and competitors) like features such as emoji reactions and generative-AI
    stickers. These make your product significantly more complex in response to human
    desires. This is *feature complexity*.

    Both are distinct from *accidental complexity*, which arises not from nature or from
    human desires but from the engineering process.

[^techdebt]: Some call this technical debt.

[^english]: Please forgive me: for brevity, I sometimes say “English” to mean *natural
    language*, but of course people use many natural languages with LLMs.
    Since English is used for much of the training data and documentation, it often
    makes the most sense to use English when communicating with LLMs about code.

[^nines]: Experienced designers and engineers will tell you to count nines.

    We tend to forget, when seeing prototypes and demos, a fundamental fact: the design
    and success of products is fundamentally different depending on whether they need to
    work 90 %, 99 %, or 99.999 % of the time.

    To take a healthcare example, compare the software involved for (1) Googling and
    reading WebMD, (2) messaging your physician, and (3) the tools and process your
    pharmacist uses to make sure the right pill is in your prescription bottle.
    If you want to add machine learning to each of those use cases, the approach needs
    to be very different in each.

[^aug]: *Augmenting Human Intellect: A Conceptual Framework* —\
    https://www.dougengelbart.org/pubs/augment-3906.html

[^whitehead]: “It is a profoundly erroneous truism … that we should cultivate the habit
    of thinking of what we are doing.
    The precise opposite is the case.
    Civilization advances by extending the number of important operations which we can
    perform without thinking about them.”
    —Alfred N. Whitehead, *An Introduction to Mathematics* (1911), p. 61

* * *

## License

© 2024-2025 by Joshua Levy

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International
License](http://creativecommons.org/licenses/by-sa/4.0/).

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)
