# Linters for Thought: Reflections on Software Engineering and Collective Intelligence

<div class="sans-text">

**Joshua Levy** ([GitHub](https://github.com/jlevy), [Twitter](https://x.com/ojoshe))\
*v0.1.12 (July 2025) – Draft!*

<div class="boxed-text">

This is a draft. I’d be grateful if you share your thoughts on any part, especially
skepticism or disagreement, as I revise it.
The easiest way is to tag or DM me: [x.com/ojoshe](https://x.com/ojoshe)

</div>

</div>

## Acknowledgments

I’m grateful to those who have discussed key ideas or who have given me feedback,
including Adam Cheyer, Amina Green, Sean Grove, Bekir Khan, Kevin Lin, Carlos E. Perez,
and Russell Power. I would like to include more references and credits where they are
due. If you know relevant work or if your own work is relevant, please let me know so I
can reference it.

* * *

## Introduction

> “*Civilization advances by extending the number of important operations which we can
> perform without thinking about them.*” —Alfred North Whitehead[^whitehead]

> “*Simple should be simple.
> Complex should be possible.*” —Alan Kay[^kay]

This work is a collection of reflections and research ideas on software engineering and
tools to augment our *collective intelligence*—that is, to improve our ability to find
solutions to complex human problems.

I’ve worked in software and knowledge tools for two decades, in research, in startups,
and in publishing. In terms of the ability of software to impact our lives, right now,
the mid-2020s, is possibly the most exciting time since the dawn of the Internet.

I’ve also used LLMs almost every day since 2022 and read *far* too many strong opinions
about AI on Twitter.
I find there are several ways my own views seem to differ significantly from what I see
in popular discussion.
This is my attempt to capture the insights I want to share when I talk to founders,
engineers, and others about how we can use AI and software for good.

There is quite a bit here, but it is all in support of four key points:

1. **IA (intelligence augmentation) deserves more attention.**

   Although popular debate today focuses on AGI and how AI can replicate human
   abilities, Doug Engelbart’s ideas on augmenting *human* intellect (*intelligence
   augmentation*, or IA) are as prescient and relevant as they were 50 years ago.

2. **Software engineering is essential to solving human problems.**

   LLMs writing code is a profound change in software.
   But it does not reduce the need for software engineering; rather, it increases it.
   The essential challenge of software engineering is *the exploration of software
   solutions to human problems*—and this need is as acute today as it was decades ago.

3. **Software engineering reveals the future of knowledge work.**

   The challenges of software engineering in fact give glimpses into the future of *all*
   human knowledge work.
   Instead of saying software engineers are being replaced by LLMs, it is more accurate
   to say *the patterns of how software engineers use LLMs will increasingly appear in
   all knowledge work and problem solving*.

4. **We should focus on better “infrastructure” for knowledge work.**

   In both software engineering and other knowledge work, the most difficult but
   high-leverage activities *improve tools to explore solutions more efficiently*. This
   is analogous to software engineering, where the most powerful systems rest on
   well-designed programming languages, flexible developer tools, and stable
   infrastructure.

If you find you agree with these arguments, you’ll see this suggests different areas of
emphasis than is currently in many research labs and AI startups.
It suggests areas where we could take inspiration from known patterns like linting to
build more powerful tools for thought and collective problem-solving.[^matuschak] At the
end, I give a few ideas for areas to focus on.

<div class="boxed-text">

*In case you’re in a hurry or skimming, key insights are in boxes like this.*

</div>

## The Unfinished Revolution

> “*When you make it harder to do the basic parts of an activity, the more advanced
> parts become almost impossible … Tools don’t only make things easier: they allow us to
> augment ourselves to do things that were previously impossible.*” —Doug
> Engelbart[^aug]

### The Problem of Solving Problems

In 1950, Doug Engelbart was 25, newly engaged, and realized he had no career plans.
After months of reflection influenced by Vannevar Bush’s 1945 essay “As We May Think,”
he famously came to three conclusions:[^bush][^engelbart]

1. He would focus his career on making the world a better place

2. Serious efforts to make the world better would require harnessing collective human
   intellect to contribute to effective solutions

3. If we could dramatically improve how we do that, we’d be boosting every effort on the
   planet to solve important problems

A key inspiration in my own career was meeting Doug in the 2000s, when I was a young
researcher at [SRI](https://en.wikipedia.org/wiki/SRI_International).

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

Doug’s vision never wavered, but in spite of the immense impact of his work on the
Internet, the GUI, the mouse, and almost every piece of software we use, he always
considered his dream unrealized.

However those who knew him tend to feel his most profound legacy wasn’t the mouse or
GUI, but rather his “[unfinished
revolution](https://dougengelbart.org/content/view/194)”—a vision for increasing our
collective capacity to address challenging problems.

It’s time we apply the vastly more powerful tools of today with this vision in mind.

### To Shape the Future, Study the Past

> “*The farther back you can look, the farther forward you are likely to see.*” —Winston
> Churchill

Another old mentor of mine, Adam Cheyer (who was also at SRI, before he built Siri),
used to tell me: if you want to see the future of technology, you should look to the
past.[^futurehistory]

Recently, famous technologists seem to make confident (and often extreme) predictions
about AI almost every day.
However, predictions about large technology-driven changes are highly unreliable, even
when made by experts.

In technology, some things change fast—and some don’t change at all.
The hard part is figuring out which parts are which.

<div class="boxed-text">

*The inherent challenges of building AI and software products have been with us for
decades. To **plan the future**, we must also **study the past**.*

</div>

### Programmers Live in the Future

In the next section I want to take a significant detour through some historical insights
about the challenges of building software.

When we look at the history of the Internet, one persistent fact is that many of the
things that most influenced online products and culture were first observed by
programmers. Although historically, programming was at first seen as an arcane skill,
over the history of programming, we have seen over and over that the challenges and
insights of programmers are usually challenges or insights we face in general with
knowledge work.

<div class="boxed-text">

*If you want to see the future of the knowledge work, look at what people who build
software are excited about today.*

</div>

The rise of LLMs are making it possible for non-programmers to become programmers,
programmers to become designers, and roles to increasingly blur.
Along with this, the dichotomy between human language and code is blurring.

LLMs don’t change the fundamentals of writing, communication, or clear thinking.
But they are accelerating many of the challenges that we have seen in software and
digital media for many years.

## Principles of Software Engineering

> “*Technology is the solution to human problems, and we won’t run out of work till we
> run out of problems.*” —Tim O’Reilly[^oreilly]

### What is Technology?

Many people today fear AI eliminates jobs.
It’s true many roles are changing or being eliminated, but as Tim O’Reilly explains,
human problems are complex and evolving because human desires are insatiable.
Technology is what gives us ever-evolving ways to find solutions to those problems.

<div class="boxed-text">

***Technology** is the solution to human problems.*

</div>

### What is Software Engineering?

People (even programmers and tech leaders) make confused statements about programming
and engineering[^progvseng] surprisingly often.

The thinking seems to be: *Programmers write code.
But now AI writes code—in fact, better than most programmers.
Therefore, programmers are no longer needed.*

In my view, this reasoning reflects a deep misunderstanding of what engineering is.
It is much like confusing writing with typing.
Writing certainly *involves* typing (at least, it usually does today), but it’s a woeful
misunderstanding to think the value of a writer is their typing
ability.[^combinedskills]

Software engineering is not writing code.
It is not simply implementing a specification—or even commanding an AI tool to build a
solution.

Not all human desires are logically or practically feasible.
Sometimes problems are ill-defined.
And even when the problem is clear, it will not be apparent what kind of software will
best solve the problem.
It takes time and effort to *explore* the problem and possible solutions.
Engineering is a practical exploration of solutions to a problem.

<div class="boxed-text">

***Software engineering** is the precise exploration of software solutions to human
problems.*

</div>

### Do We Still Need Software Engineers?

Not everyone would give this definition of engineering, but I hope I can convince you
this is the correct one,

Just for fun, let’s take a hypothetical example.

Imagine you had a near-magical piece of software, even better than current AI tools,
that instantly converts any user’s request to code with high fidelity and never
misunderstands them.

Say you give it to a bunch of users.
You know what you’d discover?
At first, they’ll be delighted by simple things.
But once they start to do anything really complex, your *users* will begin to have
misunderstandings *with themselves* about what they want the software to do.

They’ll realize they asked it to do A and B but actually that implies C. And now they
look more closely, C is definitely not what they wanted.

So what would happen next?
The more clever or determined users would start *exploring* what they really wanted.
Changing B to D or adding a special case E, and so on.

You know what you’d call those determined, unusually analytical users who were good at
figuring out what people really want?

You guessed it: engineers.

<div class="boxed-text">

*LLMs and agents alter engineering processes and the skills engineers need, but they
**do not eliminate the need for engineers**.*

</div>

### What is Good Engineering?

Another fundamental question is, why is software engineering so hard, both for humans
and now for LLMs?

The answer, of course, is *complexity*.

For better or worse, it’s a fact that humans have varied and insatiable desires.
And our desires arise not just from our own needs or imagination, but out of what we see
others want.

And as a consequence, human problems are *complex* and *constantly evolving*.

So more often than not, the solutions are complex and constantly evolving.

That means *good* software engineering is the art of rapidly and effectively exploring
and building software solutions to human (or specifically customer) problems that are
complex and evolving.[^whyfast]

<div class="boxed-text">

***Good engineering** is engineering that allows **sustained velocity** in exploring
solutions.*

</div>

You need to do it quickly but at the same time without getting bogged down by details
that aren’t really relevant to the problem.

As one of the best engineers I know puts it, “good engineering is moving fast but not
painting yourself into a corner.”

### Product vs. Infrastructure Engineering

Often, using a single word for distinct but related things can lead to a lot of
confusion.

While we’re talking about this, it’s worth distinguishing between two kinds of
engineering.

In comedy, there are “comedians’ comedians”—the comedians other comedians most respect.
But these are often *not* the people the general public finds most funny.

There is something similar with engineering.
For lack of better terminology, I’ll call them *product engineering* and *infrastructure
engineering*.

What is “infrastructure”?
For our discussion, it is *any* tooling that helps engineers, including programming
languages, frameworks, libraries, IDEs—and new AI-based tools (e.g. Cursor, Claude Code)
and agent frameworks.

<div class="boxed-text">

***Product engineers** explore solutions for users.*

***Infrastructure engineers** explore solutions for other engineers.*

</div>

This distinction can help resolve some confusions.

For example, you’ve probably seen heated arguments between engineers on things like what
database to use, which programming langauge is better, or if microservices are a
mistake.

Product-thinking people often find these arguments confusing or just a waste of time.
That’s because they are not about product engineering.
They are about *infrastructure engineering*: they are arguments about *what
infrastructure will lead to future sustained velocity* for other engineers.

Product-oriented people most respect people who give solutions to users.
Engineering-oriented people most respect engineers who help other engineers be more
productive.

These observations have applied for decades on software teams.
But this observation has new relevance today with LLMs.

LLMs are currently best implementing clear specifications.
Product engineers usually have clear specifications for a feature.
However, it’s much harder to give specifications for infrastructure engineering because
almost every hard decision is non-obvious and second order.
And it can takes time (often years!)
to see if it worked out as intended.

To a junior engineer, Java and Python may both seem perfectly fine for writing programs.
Similarly, Postgres and MongoDB might seem like just two different ways to store data.
To an experienced engineer, these are radically different technologies.
This is because they have years of experience with the non-obvious and painful ways each
of these tools caused them problems.

So how does this relate to LLM tools?
Well, LLMs help all engineers, but they can do more for product engineers than for
infrastructure engineers, because LLMs are best at pattern matching from training data.
Such pattern matching works better for features (which are typically written using
similar languages and syntax) than for infrastructure (which can change the way you
solve problems entirely).

There are two consequences of this.
First, this means human engineering effort is increasingly about infrastructure
engineering. What helps human engineers be more productive also helps LLMs be more
productive. And secondly, good infrastructure, once it is used in training data, also
helps LLMs.

<div class="boxed-text">

*LLMs are better at product engineering than at infrastructure engineering.*

</div>

<div class="boxed-text">

*LLMs make (human) product engineers more effective.
But (human) infrastructure engineers are what make LLMs more effective.*

</div>

Let’s give an example of the last point.

Almost all engineers readily acknowlege that CSS is overly complex and full of pitfalls.
Thankfully, many people now say, LLMs know CSS and can now handle the things that were
previously error-prone for humans.

This is true. But what is often overlooked is that another thing is also true: if it’s
hard for humans, it’s also hard for LLMs!
It is *relatively* far more productive to use an LLM with good infrastructure than it is
with bad infrastructure.[^infravsllm]

<div class="boxed-text">

*If you can minimize irrelevant complexity for an LLM while staying within the scope of
the training data, you can achieve more with an LLM.*

</div>

Minimizing accidental complexity for engineers and LLMs is (for a while at least) still
the job of human infrastructure engineers.

This brings us to another word that has a few distinct meanings in engineering:
complexity.

### Three Types of Complexity

> “*People will strive to experience an equal or increasing level of complexity in their
> lives no matter what is done to reduce it.*” —Bruce Tognazzini

An alternate and important way to frame the concept of good engineering is originally
due to Fred Brooks: good engineering involves exploring the *essential complexity* of a
problem and possible solutions without adding too much *accidental complexity* that
distracts and hinders your ability to find solutions to problems.[^nosilverbullet]

This is actually just a reframing of the same definition above of sustained velocity.
Having too much accidental complexity is a common way engineering slows down and becomes
ineffective.[^techdebt]

In fact, I think it’s best to think of *three* kinds of complexity that arise in
engineering:

- **Natural complexity:** If you are building an airplane, you need a good understanding
  of aerodynamics and materials science, which are governed by quite complex
  interactions of the laws of physics.
  This is natural complexity.
  It involves the inherent consequences logic, mathematics, physics, and the real world.
  It is ultimately consistent.

  *Engineers should always try to understand natural complexity.*

- **Feature complexity:** On the other hand, if you are building a messaging platform,
  you will discover your users (and competitors) like features such as emoji reactions
  and generative-AI stickers.
  These make your product significantly more complex as you try to make your users
  happy. I’ll call it *feature complexity* and it really is the complexity of human
  desires. It is not well defined and subjective but under your control.

  *Engineers should exercise careful judgement about when to explore feature
  complexity.*

- **Accidental complexity:** As you build something, it invariably becomes more and more
  complex. Most large, popular software is so complex few normal people can even hold all
  the details in their mind.
  But a lot of it is details that don’t really matter in the design process.
  Accidental complexity arises not from nature or from human desires but from the
  engineering process.

  *Engineers should avoid or reduce accidental complexity.*

Very simply:

- Natural complexity arises from logic or the world around us

- Feature complexity arises from human desires

- Accidental complexity arises from human stupidity

Note “essential complexity” is a slightly misleading term, because it sounds like if it
is “essential” it might be fixed or unchanging.
This isn’t true! In fact, feature complexity always grows due to human nature and
[**Tog’s paradox**](https://www.votito.com/methods/togs-paradox/): as soon as you solve
a problem for someone, they will think of a new problem.

<div class="boxed-text">

*The **hard part of engineering** is understanding and exploring **natural complexity**
and **feature complexity** while managing **accidental complexity**.*

</div>

Note this is true whether you’re a human developer or an LLM agent.
It’s one more thing that *doesn’t* change with progress in AI.

### Why Don’t Apps Have the Features We Want?

So we now know one reason it’s hard to be a good software engineer: because it’s hard to
explore the essential complexity of problems.

It can be hard to understand what problems your user (or even you yourself) are really
solving, and it’s hard to identify the essential parts of that problem.
And especially over time, it’s hard to build and evolve solutions that aren’t
constrained by accidental complexity.

We all know numerous situations where we want a software program to solve a problem we
have. But we know ChatGPT, Anthropic, Notion, Google Docs, Slack, Excel, and Zapier, and
dozens of other products don’t quite solve it directly.

But often, we know what the solution is.
Why don’t companies build the solution to your problem?

There are several reasons for this.
And they depend on the size of the team and some apply *even if people know the solution
and know how to build it*. It’s worth being aware of the key ones:

1. **Lack of awareness:** They don’t know the problem exists.

2. **Lack of understanding:** They are aware of the problem but don’t understand it
   properly (because they haven’t talked to users or because they can’t as a team
   articulate or communicate what is needed in a way that can be built).

3. **Lack of resources:** They understand the problem, but don’t have the resources
   (money, data, or people with the right skills) to design and build it.

4. **Innovator’s Dilemma:** They understand and have the resources, but to do so seems
   irrational because it is *relatively* less profitable than working on existing,
   successful products and features.[^christensen]

5. **Conway’s Law:** They understand the problem *and* have resources and incentives to
   solve the problem, but *still* don’t solve it (or solve it poorly or do something
   else). You might wonder if this is really possible, but it is very common for larger
   teams. The reason many companies don’t add specific features you want, even if they
   should and they are obviously a good idea, is
   [Conway’s Law](https://en.wikipedia.org/wiki/Conway%27s_law): teams are almost always
   constrained to ship products that mirror their organizational structure.

Looking at these reasons, we can see that for the most part, none of these fundamentally
go away with AI tools.

So while AI tools are changing software and even radically changing the jobs of people
building software, we will still always want things faster than developers, product
managers, designers, entrepreneurs, and companies design and ship solutions.

<div class="boxed-text">

*Even with perfect engineering and powerful AI, software and features are always
constrained by **human communication**, **profit incentives**, and **organizational
structure**.*

</div>

## The Future of Software Engineering

Now we’ve talked about the essential facts that seem inherent to how and why we build
software, it’s time to ask what *is* changing?

One of the most remarkable shifts in the last year or two is that more people are able
to code more complex things by using Cursor, GitHub Copilot, and other LLM coding tools.

It is now common to hear that English is the new programming language.[^english]

This clearly is partly true.
But of course applications are still actually committed to GitHub and then deployed
based on Python, TypeScript, Rust, SQL, and the other standard programming languages.

So is English now code?
Do we even agree on what code is?

### What is Code?

Just as there are common confusions about the essential nature of engineering, there are
also some common confusions about the essential nature of code.

When learning to program, people tend to think of programming as communicating with the
computer. It can be good for learning or a fun challenge to do this “the hard way” in C
or assembly language.
Over time, whenever they can, engineers and programmers invariably move to
“higher-level” languages and frameworks that are easier to write in.

But there is a key point even some experienced programmers forget: As systems evolve,
more time is spent reading, debugging, and changing the code than writing it.
In software engineering, the true goal of writing code is not to give the computer (or
more generally, the distributed system) commands, but to communicate to yourself and to
other engineers what the whole system should do.

As a side effect, you produce code that works (and, if you’re good at it, also runs
efficiently). Compilers can be built for any language.
The history of the development of “better” programming languages is the history of
improving the languages to support communication *with people*.

The point is still that code is actually about communication between humans.

Now the ways we code are changing a lot with LLMs.
Much code is written or explained by LLMs to a human (vibe) coder.
So LLMs are like co-pilots for writing, sharing, and modifying code.

But with only a small addition we have a clear definition.

<div class="boxed-text">

***Code** is any text format that describes the behavior of software with **exact
precision** in a way humans (and LLMs) can understand.*[^exact]

</div>

Aside from mentioning LLMs, this definition is the same as it would have been 20 years
ago.

Code is the medium to allow humans to perform the process of exploring solutions in a
completely precise (and ideally, practical) way.

That’s why *effective workflows* around code, such as tests, commits, pull requests, and
code reviews, are so important.
They are what structure and manage the complexity of expressing and updating the current
description of the software’s behavior.

### What is a Specification?

Traditionally, people thought of a specification as a natural language document (like a
product requirements doc or an API spec) that described what software should do *before*
code was written. The idea was that business analysts or architects would specify
behavior precisely enough that programmers could implement it correctly.

Famously, the waterfall approach to software development rarely worked in practice.
(At this point this should come as no surprise since we know it fundamentally hinders
the true process of engineering.)
Specifications were too vague, didn’t reflect a correct solution, or were too detailed
to maintain as requirements evolved.

Documents are “dead” unless they are part of routine engineering workflows.
So over time, the “real” specification was often just the code itself.

Now vibe coders working with LLMs are rediscovering specifications, because of this
crucial difference. While imperfect, it’s now far easier to convert English to and from
programming languages.

The history of programming languages perfectly illustrates this convergence.
Assembly required developers to think like machines.
C abstracted away memory addresses.
Python reads more like pseudocode.
Each generation of languages moved closer to how humans think with precision about the
essential complexity of problems.

<div class="boxed-text">

***Specifications** are text format that describes the behavior of software with
**inexact precision** in a way humans (and LLMs) can understand.*

</div>

<div class="boxed-text">

*Code and specifications are both **ways to express the desired behavior of software**.
The differences are a matter of **language** (programming language or natural language)
and **precision** (exact vs inexact).*

</div>

### Counting Nines

Experienced designers and engineers sometimes talk about counting nines.
This is because of a fundamental fact:

<div class="boxed-text">

*The design of products is fundamentally shaped by the **cost of errors**: whether they
need to work 90%, 99%, or 99.999% of the time.*[^uptimevscorrect]

</div>

Let’s illustrate this by imagining you have back pain.
Consider these three systems:

1. The search engine and websites that help you find articles about treating back pain

2. The online messaging system you use to write to your physician about it

3. The software and process the pharmacist uses to fill your prescription bottle with
   the correct pill

The first can tolerate a 1–10% error rate since you’re reading many things and will form
your own opinions. The second can tolerate perhaps a 1% error rate.
The third has very low tolerance for error, perhaps a 0.01% error rate or less.

It is certain that each of these systems could improve with machine learning and AI. But
if you want to add AI or machine learning to each of those use cases, the approach needs
to be very different.
You can’t get away from the fact that some systems need high reliability and precision.
In other cases, we can adapt to errors because the cost of errors is low.

### Exact and Inexact Processes

Most complex human endeavors can be viewed as a **socio-technical system**[^sociotech]
that involves people, tools, and written or unwritten processes.
Some activities in such a system are informal or ad-hoc, and some are more systemetized.

As systems and products mature, processes are codified and automated for efficiency and
consistency. And the decades since software began “eating the world,” many of the tools
and processes are implemented in software.

For example, in a mature software business, there is a process for how software is
deployed as well as processes for customer support.
In an accounting department, there is a process for calculating revenue as well a
process for auditing financial statements.

Let’s call standard processes like this **procedures**.

Procedures are not all the same.
Some procedures are exact.
When software is deployed, the program that users access should be *exactly* the same
program that the developers tested.
When an Excel spreadsheet calculates the revenue for the month, it should be *exactly*
the same calculation performed last month.

Other procedures are inexact.
Even the most codified customer support processes are not exact.
They require best-effort judgement in certain cases.
The same is true for auditing financial statements.
The decisions may often be clear-cut but there will inevitably be situational gray areas
that need ongoing resolution.

<div class="boxed-text">

*Socio-technical systems require a combination of both **exact procedures** and
**inexact procedures**. Exact and inexact procedures are qualitatively different,
regardless of how they are implemented.*

</div>

Imagine that you have code that performs a task, such as using an API to get your sales
data from your payment processor.
And you have certain pieces of code to calculate customized monthly sales metrics.
It’s easy to combine these into reporting software that does both reliably.

This is how software is built: by **composition**. A typical application is the
composition of dozens or hundreds of layers like this.

That is the power of software precisely encoding exact procedures.
However, inexact procedures are different.

Imagine you have an inexact procedure for a sales engineering team to configure your B2B
SaaS product to work for a new customer.
And you have an inexact procedure where an account manager emails the customer to be
sure they’re happy with the service.
Partly or even fully automating both these processes might be possible, but it’s not a
simple composition of two procedures.
To do this right requires creating *more* procedures, such as a dashboard for the CEO,
the sales lead, and the account manager to monitor the state of these automations and
deal with issues personally.

<div class="boxed-text">

***Exact procedures** are **easy to compose**: if you combine them, the result is an
exact procedure.*

***Inexact procedures** are **hard to compose**: if you combine them naively the result
is often useless or doesn’t work as you expect.*

</div>

I’m not saying you can never compose inexact procedures.
In fact, you often need to compose them a lot.

It’s just that because each one has its own corner cases and failures, you can’t
unthinkingly combine them and expect the resulting combination to work!

The design of systems of inexact processes is qualitatively different from pure software
engineering.
This is why many generic early “agent frameworks” were not as useful as they
at first may have seemed.
Agent frameworks often are trying to compose lots of inexact processes (e.g., check the
user’s calendar, navigate to the airline website, choose the flight, pay for it),
blindly hoping the composition would work.

### Is English the New Programming Language?

Engineers are now writing more software just by using English and natural-language
specifications and docs.
Developers of [Claude Code](https://claude.ai/code) now say most (perhaps even 90%) of
Claude Code’s own codebase is now written in Claude Code.
This is a remarkable fact.

It’s now tempting to say English is the new programming language, and LLMs are the new
compilers. (On Twitter, and you’ll see similar statements almost every day.)

I hope by now you’d agree with me that this isn’t the most insightful way to frame what
is happening.

Specifications in English and code in Python may have similar purpose but are not
interchangeable. English is too ambiguous and imprecise for exact procedures.

This is a fundamental issue, with both natural language and the development of LLMs.
Even if an LLM correctly interprets an instruction 99.9% of the time today, it’s a
significant challenge to have a process that ensures the updated LLM you will be using
next month will do the same thing 99.9% of the time.

<div class="boxed-text">

***Inexact procedures** are best expressed in **English**.*

***Exact procedures** are best expressed in **code**.*

</div>

There is an interesting nuance, however: Could we think of English as an “inexact
program” that we “compile” using an LLM to code, and then review and use that code?
Well, yes! That’s what we are already doing when we use LLMs to code.

But the key thing is, this process *is itself inexact*! There’s no free lunch.
Making a procedure exact is a process of exploring straggling, unresolved ambiguities.
This requires information about the problem, not just the current solution.
So to get exactness takes human effort.

One thing that *is* changing right now: traditionally, we tend to only save or version
control the code. Increasingly, we may wish to version control the spec that led to the
code, as well, so we can streamline the update process of “re-compiling,” reviewing, and
testing the code.

### Automation of Inexact Procedures

Traditionally, we have used code for exact procedures.
And we’ve used people and documents for inexact procedures.
But LLMs change all this.

<div class="boxed-text">

***LLMs** are now **as good as humans** for most inexact procedures.*

</div>

<div class="boxed-text">

***Inexact procedures** will increasingly become **automated** with **natural language
specifications** shared by both humans and LLMs tools.*

</div>

Because of this, engineering workflows engineers have devised over decades to manage the
complexity of code (like version control, code reviews, and so on) will begin to apply
to English specifications, just as they do now for code that defines exact procedures.

However, this doesn’t mean English is just like code.
LLMs can automate inexact procedures but without clarifications to the procedure,
automation does not make an inexact procedure exact.
To automate an inexact procedure you have two options:

- Automate but combine it with interactive human oversight on an ongoing basis

- Invest in human engineering (perhaps also with LLMs) to explore new ways to convert
  the inexact procedure to a more reliable exact procedure

Automated workflows for inexact procedures will lead to great efficiency gains.
But we have to remember:

<div class="boxed-text">

***Automation** is not the same as **exactness** of a procedure.*

</div>

Basically, we are seeing an explosion in the forth quadrant of this table:

|  | Exact procedures | Inexact procedures |
| --- | --- | --- |
| *Manual implementation* | **Traditional tedious paperwork**<br>(increasingly obsolete) | **Traditional company processes**<br>(most work at large companies today) |
| *Automated implementation* | **Typical software usage**<br>(defined in code, run on a computer, used by humans) | **New agent-human workflows**<br>(defined in English, interpreted by LLMs, interactive with humans) |

### Software Engineering with LLMs

Now let’s think about software engineering again.
If we accept that human engineers still need to work with code, what is changing?
I think of three key areas:

1. **Faster coding with LLM tools:** Engineers can code more quickly by using English
   with LLMs and LLM-powered agents to read, write, and test code more quickly than ever
   before (e.g., “vibe coding” prototypes)

2. **Broader capabilities of human workers:** Because a single person can build and test
   software more quickly, they can rapidly make experiments; in fact, they can
   effectively broaden their roles (e.g., a designer coding in HTML/CSS instead of
   waiting for a frontend engineer to convert Figma to code)

3. **Software processes described in natural language:** We are seeing the emergence of
   English documents as specifications that are critical parts of workflows, used by
   both humans and LLM agents (e.g., Claude agent rules, LLM-based validation workflows)

We’re moving from a world where we had occasional, poorly used English specifications to
one where clear and precise English is essential to working efficiently with our tools
and teammates. And we’ll work with this *and* traditional programming language code with
formal semantics.

LLMs are pushing us toward precise and structured ways of expressing software that are
more human friendly.
It’s quite likely we’ll see emergence of languages at new points between English and
current programming languages, or of rigorous, constrained formats for English
(themselves enforced by LLMs and grammar specifications).

### What is the Future of Knowledge Work?

Does the history of software engineering really have relevance for us today for people
who are not engineers or builders of software?

I think it does. The most difficult problems we face, where our collective intelligence
is most needed, are increasingly similar to the challenges of software engineering.

A decade ago, the practice of writing software was so different from writing emails or
having meetings that it seemed like they were entirely different disciplines.

But if what we care about is working effectively together to explore solutions to human
problems with software, the approaches that work are *the same processes that work for
software*.

And now AI tools transform the nature of our work so code and language, writing and
spoken word, are increasingly interchangeable, the distinctions of the past are becoming
flimsy.

In short, if you believe all the points I’ve made so far, you may see some possibly
surprising conclusions:

<div class="boxed-text">

*The consequence of AI coding tools is not that software engineering is going away:
instead, it means **more knowledge work involves engineering**.*

</div>

<div class="boxed-text">

*The distinction between **software engineering** and **knowledge work** is
disappearing.*

</div>

This may be a bold statement, but I think it’s worth exploring its implications.

## The Metaphor of Linting

### A Brief History of Linting and Type Checking

The power of incremental improvements is powerfully illustrated by the history of
linting and type checking in software.

The original *lint* was created in 1978 by Stephen C. Johnson at
[Bell Labs](https://en.wikipedia.org/wiki/Bell_Labs) to flag bugs and portability issues
in C programs. Modern linters parse code into abstract syntax trees and check it against
predefined rules. The idea was to catch bugs early before they manifest at runtime.

Now as it turned out, the validation of code is one of the hardest problems in software.
Over the past 40 years, this idea has slowly but consistently grown in maturity and in
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

### Type Checking and LLMs

Today the rise of LLMs means more and more code is written by LLMs, with some human
oversight and review.

But this doesn’t change the value of linting and type checking.
In fact, it seems to make it all the more important.

An interesting example: For decades, there have been debates among programmers about the
the advisability of using strongly typed languages (like Rust or Java) and to what
degree dynamically typed languages (like Python and JavaScript) should have types added.

These debates have suddenly largely been resolved.
Almost everyone using Cursor and other AI tools have quickly seen how types make LLMs
far better at coding accurately.

A similar thing is true for unit tests.
While people often knew that unit tests were a good practice, the fact that they are now
quick to write with LLMs *and* they then benefit LLMs in writing code with fewer bugs
has driven a rapid increase in their use.

<div class="boxed-text">

*When it comes to developer tooling, what is good for humans is great for LLMs.*

</div>

### What is Linting?

Historically, linting is mostly used to refer to highlighting fairly low level, specific
coding errors.

One lesson of linting is that catching typos or obvious bugs saves time.
But the impact is more profound than that.

Metaphorically, it’s worth extending the idea to include type checking and more broadly,
checking for a wide range of specific errors, both for humans and for LLMs.

<div class="boxed-text">

***Linting** is the use of tools that minimize the attention needed to fix errors or
inconsistencies.*

</div>

### Why is Linting Powerful?

For complex and difficult problems, the scarcest resource is attention.
Linters (broadly speaking) make small and common errors something you waste less
attention on. This benefit is compounding and significant even for one engineer.
It is even larger with a team of engineers or LLM agents.

<div class="boxed-text">

*Tools **increase in power** as they **remove the necessity of fixing small errors**
inessential to the core problems at hand.*

</div>

A key part of this broadened idea of linting is that it can include a more kinds of
tools:

- Tools that automatically fix small or trivial errors (some spell checking is like
  this)

- Tools that surface errors that support other automated processes (type checking with
  an LLM agent is often like this)

- Tools that flag issues that need to be addressed later or reviewed by humans

- Tools with a UI that interactively supports a human in writing or thinking with
  greater consistency or clarity (such as using colors or annotations)

- Tools with a UI that supports multiple people in writing or thinking or in resolving
  disagreements

If you think of linters generally in this way, it becomes apparent that with the power
of LLMs, we can build linters at various levels of the “stack” of human knowledge
work:[^drucker]

- **Language:** Spell checking and grammar (much like Grammarly)

- **Style rules:** Enforcing larger sets of language rules

- **Factuality:** Tools that surface and help confirm factuality of statements

- **Basic consistency:** Tools that help enforce logical consistency

- **Formal consistency:** Tools that formally model concepts or assertions and actually
  formally look for proofs and surface soundness or possible errors or inconsistencies

## Strategies for Building Tools

<div class="boxed-text sans-text">

This section is still in progress and I’d like to refine these ideas.
I’d welcome your suggestions!

</div>

What are the tools that can help people iteratively improve the quality of written work
and consequently, of their ideas, both individually and when collaborating?

We need to look for more reliable, small steps that makes meaningful adjustments and
improvements to content so it is better in different dimensions—clarity, rationality,
rigor, and so on. By improving content along the right dimensions, and using these tools
collaboratively, so the judgement of many people is combined, it seems we can
significantly improve the quality, rigor, and real-world effectiveness of many ideas.

### What Will Improve Tools for Thought?

For certain hard problems, the devil is in the details.
Often we can have exactly the right idea but not work on it at the right time.
Or we might be at the right time but not be in an organization or with a team of the
right structure and incentives to have the outcome we want.

I’m fortunate to have worked at the intersection of knowledge tools, publishing,
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

- **IA over AI:** Prioritize tools that *augment human ability* rather than just
  maximizing model performance

- **Extend primitive operations:** *Bottom-up development* of small, individually useful
  tools that are open source and composable so they can be combined in varied,
  unexpected ways

- **Simplify complexity for all layers:** This is the tricky part: Making things simple
  is hard, especially when the accidental complexity is spread across multiple layers.
  It’s necessary to innovate and experiment at three layers:

  - the content layer (text editing and annotation workflows that encourage
    transparency, quality, and rigor)

  - the UX layer (going beyond chat and doc UIs to more flexible hybrids that are easier
    for unplanned workflows and cases, especially GUI/Terminal hybrid design)

  - the engineering layer (restructuring and repackaging typical messy full-stack web
    development in simpler ways so that simple apps are simple and for both humans and
    LLM coders)

This may sound ambitious but I think we can be ruthlessly practical about it too.
(See below for some concrete examples of what I’ve begun building.)

### The Value of Flexible Primitive Operations

If we wish for LLMs to improve human rationality and our ability to work together, we
need more tools that make complex tasks feel like easy steps.

That’s why it makes sense to build tools that make individual steps more powerful, so
larger, human processes accelerate over time.

In software, big ideas often must be realized from practical, concrete pieces.

Typically there are two opposite pitfalls when building software:

- **Under-engineering (inadequate up-front design):** This is when you don’t plan ahead
  and just building a tool, realizing it doesn’t work as hoped, but then getting stuck
  because the complexity of the software is too high to change it.
  This too little design and too much technical debt.

- **Over-engineering (too much up-front design):** This is the opposite, which is that
  you’re so afraid of inadequate design that you design a much more complex
  architecture—but then it ships too slow and it too might not work as hoped.
  This is too much design without testing and learning.
  This is common among engineers of moderate experience and was called by Fred Brooks
  [the second-system effect](https://en.wikipedia.org/wiki/Second-system_effect).

Unfortunately, for products like knowledge tools, the use cases are complex and not
obvious. So both of these are real risks.

So what do you do?

My answer is you should work “bottom up”—that is, you should build small pieces that
combine in many ways, including in ways you can’t plan for right now.

If you can build small pieces that combine in many ways, the right combinations and
workflows become easier to discover.

There is an old analogy for this: if you are improving a college campus, you can try to
design all the walkways up front, or you can put down grass, wait for students to create
paths in the grass, then pave the discovered paths.

<div class="boxed-text">

*Tooling should aim for powerful **primitive operations** and allow **discoverd paths**
that combine these operations in varied, creative ways.*

</div>

### Principles for Compositional Tools

In software, big ideas often must be realized from practical, concrete pieces.
So I think it makes sense to work “bottom up.”

So what are some areas where we could begin to build better primitive operations?

Some key principles are:

1. **Transparency:** Increase visibility of content at all times, including text, edits,
   and LLM prompts used to make edits.
   (Many current AI tools don’t reveal all these details.)

2. **Flexibility:** Increase variety of operations.
   It should be easy to add new operations.

3. **Power:** Single operations should be able to do quite complex things.
   An example would be fact checking a document and adding annotations.
   Or transcribing, summarizing, and formatting a lecture.
   A key part of this is **reduced friction** around performing different operations.
   For example, it is far preferable to have a unified UX rather than having to
   copy/paste into and out of your ChatGPT window for each step.

4. **Reliable quality and groundedness:** So far, LLMs are great at plausibility and
   mediocre at factual and rigorously logical.
   Models, especially reasoning models are improving, but we also need ways to make
   unreliable steps more reliable.
   A key way is by having steps for additional checks like groundedness checks or
   careful reviewing of edits/diffs.

5. **Easy extensibility:** This is the biggest departure from many existing tools.
   It is easy to add new operations, and these operations should be in a simple format
   that’s also easy for an LLM to write (generally, possibly restricted Python or
   TypeScript/HTML/CSS, as these are well understood by LLMs).

6. **Built-in compositionality:** Typically missing in many tools is the idea of
   *data-driven user interfaces*. The idea is that you can combine items and operations
   in new ways *with no new code required for UI/UX*. Terminal apps are much like this
   and the idea of hybrid GUI/terminal UIs is a key way to improve them.

### Selected Ideas for Better Tools

Given this, here are some areas where I think are high leverage or underrated—where
building and exploring products could have surprisingly large impacts:

1. **Making quality of writing and clarity of reasoning more apparent**

   - **Consistent writing metrics:** Ways to measure and attributes of writing (clarity,
     cohesion, depth, rigor, factuality, warmth, etc.)

   - **Fact-check linting:** Workflows for LLM-based fact checking (perform searches,
     highlight inconsistencies, rank issues and concerns based on explicitly defined and
     revised credibility rules)

   - **Groundedness linting:** Workflows for LLM-based measurement and improvements to
     groundedness and citations

   - **Logical linting:** Surfacing areas of uncertainty or disagreement qualitatively
     and visually in text

   - **Visualizations:** Design both simple and more detailed visualizations for all of
     these

2. **Simpler and more flexible writing and editing workflows**

   - Editors and LLM-powered editing should not be apps—they should be features
     available anywhere

   - First-class support for semi-structured documents

     - The line between spreadsheet and doc should be blurred

     - The most effective way is via format conventions: a hybrid Markdown format that
       supports structured annotations that is both LLM friendly and convertible to any
       other format and that is easily editable with simple browser-based editing tools

   - Improved designs and UX for multi-role editing and review workflows

     - Key to proper collaboration is supporting workflows with disparate roles of
       different participants: writers, subject-matter experts, fact checkers, copy
       editors, etc.

     - Traditionally, we have used collaborative documents like Notion or Google Docs,
       but these are not designed with these different roles in mind

3. **Extraction and visualization of concepts and relationships**

   - Automated concept and relationship extraction

   - Automated semi-structured fact and assertion extraction

   - There should be much less friction to grasp key concepts in written works

   - LLMs make it trivial to extract concepts and relations, but the UX for visualizing
     and improving these visualizations is still primitive

4. **Simpler and more flexible publishing formats**

   - **Make complex docs simple to publish:** Complex docs (like deep research reports)
     should be both beautiful and easy to read, supporting tables, footnotes,
     annotations, table of contents, mouseovers on links, etc.

   - **Tree summaries:** Documents should have tree summaries, i.e. recursive summaries
     of sections and subsections, so you can quickly navigate and understand the
     structure of a document, and improved browser-based UX to support reading content
     in this format

5. **Collaborative editing of structured relations**

   - For example, facts that a text makes are readily summarized by an LLM as specific
     assertions

   - But UIs for editing and curating these changes are still primitive

   - This is needed for humans reviewing LLM content, for humans reviewing content from
     other humans, and for LLMs reviewing content from humans and LLMs

6. **Integration of formal reasoning with fact checking**

   - Historically, logic-based AI expert systems have had many limitations, leading to
     their abandonment as a primary approach to AI

   - However, blending formal reasoning with LLM-enhanced annotations of facts is a
     lightweight way to combine the rigor and consistency of formality with the reality
     that no writing is ever perfectly precise or consistent

   - Tools should highlight *apparent inconsistencies* so you effectively have *logic
     linters*

7. **Bridging-based ranking for resolving disagreements**

   - **Consistency improvements via bridging-based ranking:** Bridging-based ranking is
     among the most effective ways to find helpful consensus on areas of disagreement or
     dispute[^bridging]

   - **Conflict resolution workflows:** Send a draft to a group of people to resolve
     disputed or confusing facts or parts of a work

### Will Current Companies Build These Tools?

A reasonable question to ask about these ideas for tools is whether they will simply
emerge from existing tools from OpenAI, Google, Anthropic, Cursor, or other current
companies and AI startups.

My answer is yes, of course some of these features will emerge.

At the same time, without conscious design to simplify them, they will tend to emerge in
complex ways that add accidental complexity to content and processes to maintain them.

Increasingly, LLMs are writing more code for us.
This is a good thing.

But it remains the job of creative *human* engineers to shape the way we use tools.

### Tactics for Better Tool Engineering

The above list may sound like a laundry list.
But experimenting with many of them is easier than one might think, because the tools
discussed can be built from the same more primitive pieces.

Some key areas where document and tooling infrastructure needs to improve:

- **Simple formats and conventions for files:**

  - Consistent metadata on files that is backward-compatible and simple

  - Conventions for making information available in workspaces

  - Formats and conventions for *stand-off annotations* that are compatible with LLMs

  - Formats and conventions for semi-structured data blended with text documents,
    including formats and conventions for concepts and relations and for tables

- **Simple formats and conventions for documents:**

  - Tools for managing Markdown documents in powerful, consistent ways, including
    controlled edits and readable diffs

- **Data-driven UX with GUI/Terminal Hybrid Capabilities:**

  - Currently, building things like Vercel’s “rich chat”
    [AI SDK](https://ai-sdk.dev/docs/introduction) require extensive amounts of code for
    full-stack web development, involving many frameworks.
    This is far too slow as a way to build new UX.

  - As we’ve seen with Claude Code and other tools, the terminal, while not perfect,
    allows for much more flexible workflows.
    Claude Code can add features with almost zero effort on UX.

  - It’s time we find a way to blend these approaches.
    It’s definitely technically feasible, but we need to escape the history of complex
    web stacks.

- **Better shells:**

  - A special case of data-driven UX, the classic Unix shell offers a model of an
    extremely powerful and flexible UX

  - There are numerous ways shell and shell-like UIs can be enhanced to be *both* easier
    to use and more powerful

## Appendix: A Few Experiments

Over the past couple months, I’ve found that because I can build more myself with LLM
coding tools, I have been able to prototype a few of these bottom-up tools.
These are just a start but they are pieces that build on each other.

All of these are rough and I haven’t really promoted them yet as they are early
prototypes. But I’d love early feedback if you’re willing to share it:

- **Textpress:** A new platform for simple publishing of complex documents.
  You can publish or republish research reports for Gemini or OpenAI, PDFs or DOCX
  files, or other documents in a way that’s easier to share and read, with good
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
  Think of it as a “command line for knowledge tasks”.

  It lets you iterate and experiment with “Actions” like transcribing audio, converting
  documents, fact checking, annotating, and pretty much any other task possible with
  Python and LLM APIs, but interactively and each in a single command.
  Current actions that already work are conversion of PDFs to text, transcription of
  videos, captioning and annotating text, organizing and structuring transcripts, etc.

  It’s currently terminal based (think like Claude Code).
  It also lets you chain together commands and assemble the outputs in topical
  workspaces (think a bit like [Obsidian](https://obsidian.md/)). The goal is this
  framework would be open source and let more people experiment and discover more
  powerful AI workflows.
  (It’s also compatible with [MCP](https://modelcontextprotocol.io/).)

  Repo: [kash](https://github.com/jlevy/kash)

And some lower-level libraries I’ve found helpful for the above work:

- **Frontmatter format:** Simple, readable metadata attached to files can be useful in
  numerous situations, such as recording title, author, source, copyright, or the
  provenance of a file.

  Unfortunately, it’s often unclear how to format such metadata consistently across
  different file types while preserving valid syntax, making parsing easy, and not
  breaking interoperability with existing tools.

  Frontmatter format is a way to add metadata as frontmatter on any file.
  It is basically a micro-format: a simple set of conventions to put structured metadata
  as YAML at the top of a file in a syntax that is broadly compatible with programming
  languages, browsers, editors, and other tools.

  Frontmatter format specifies a syntax for the metadata as a comment block at the top
  of a file. This approach works while ensuring the file remains valid Markdown, HTML,
  CSS, Python, C/C++, Rust, SQL, or most other text formats.
  Frontmatter format is a generalization of the common format for frontmatter used by
  [Jekyll](https://en.wikipedia.org/wiki/Jekyll_(software)) and other CMSs for Markdown
  files. In that format, frontmatter is enclosed in lines containing `---` delimiters.

  This repository is a **description of the format** and an easy-to-use **reference
  implementation**. The implementation is in Python but the format is very simple and
  easy to implement in any language.

  Repo: [frontmatter-format](https://github.com/jlevy/frontmatter-format)

- **Flowmark:** Flowmark is a new Python implementation of **text and Markdown line
  wrapping and filling**, with an emphasis on making **git diffs** and **LLM edits** to
  text documents easier to diff and review.

  - Flowmark has the option to use **semantic line breaks** (using a heuristic to break
    lines on sentences when that is reasonable), which is an underrated feature that can
    **make diffs on GitHub much more readable**. The change may seem subtle but avoids
    having paragraphs reflow for very small edits, which does a lot to **minimize merge
    conflicts**. An example of what sentence-guided wrapping looks like, see the
    [Markdown source](https://github.com/jlevy/flowmark/blob/main/README.md?plain=1) of
    this readme file.)

  - Very simple and fast **regex-based sentence splitting**. It’s just based on letters
    and punctuation so isn’t perfect but works well for these purposes (and is much
    faster and simpler than a proper sentence parser like SpaCy).
    It should work fine for English and many other latin/Cyrillic languages but hasn’t
    been tested on CJK.

  Because **YAML frontmatter** is common on Markdown files, the Markdown autoformat
  preserves all frontmatter (content between `---` delimiters at the front of a file).

- **Chopdiff:** `chopdiff` is a small library of tools I’ve developed to make it easier
  to do fairly complex transformations of text documents, especially for LLM
  applications, where you want to manipulate text, Markdown, and HTML documents in a
  clean way.

  Basically, it lets you parse, diff, and transform text at the level of words,
  sentences, paragraphs, and “chunks” (paragraphs grouped in an HTML tag like a
  `<div>`). It aims to have minimal dependencies.

  Example use cases:

  - **Filter diffs:** Diff two documents and only accept changes that fit a specific
    filter. For example, you can ask an LLM to edit a transcript, only inserting
    paragraph breaks but enforcing that the LLM can’t do anything except insert
    whitespace. Or let it only edit punctuation, whitespace, and lemma variants of words.
    Or only change one word at a time (e.g. for spell checking).

  - **Backfill information:** Match edited text against a previous version of a document
    (using a word-level LCS diff), then pull information from one doc to another.
    For example, say you have a timestamped transcript and an edited summary.
    You can then backfill timestamps of each paragraph into the edited text.

  - **Windowed transforms:** Walk through a large document N paragraphs, N sentences, or
    N tokens at a time, processing the results with an LLM call, then “stitching
    together” the results, even if the chunks overlap.

  Repo: [chopdiff](https://github.com/jlevy/chopdiff)

* * *

## License

© 2025 by Joshua Levy

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International
License](http://creativecommons.org/licenses/by-sa/4.0/).

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)

* * *

## Notes

[^whitehead]: “It is a profoundly erroneous truism … that we should cultivate the habit
    of thinking of what we are doing.
    The precise opposite is the case.
    Civilization advances by extending the number of important operations which we can
    perform without thinking about them.”
    —Alfred N. Whitehead, *An Introduction to Mathematics* (1911), p. 61

[^kay]: https://news.ycombinator.com/item?id=24463842

[^engelbart]: https://en.wikipedia.org/wiki/Douglas_Engelbart

[^futurehistory]: In fact, this is true for many fields.
    I think the reason is that in newer but rapidly growing domains—such as physics or
    math in the early 20th century, or computer science and software engineering over
    the past 60 years—when a field is young, it is small enough for a few early
    visionaries to deeply understand the whole field.
    This lets them see further ahead than even brilliant people decades later, because
    the field has become so large that no human can truly grasp it all deeply.

[^oreilly]: https://www.oreilly.com/tim/wtf-book.html

[^progvseng]: There is a long-standing and pedantic debate about whether people who
    build software should be called *programmers*, *developers*, or *engineers*. Many
    people prefer the sound of “engineer” in their job title.
    Others fairly point out that “software engineering” is a rather pretentious term
    since hacking JavaScript is quite different from “hard” engineering disciplines with
    formal standards and training, like mechanical or structural engineering.
    Generally I prefer “engineering” over “programming” simply because it helps clarify
    that building software is a process that includes more than typing code.

[^combinedskills]: It’s worth pointing out that at any point in history, the most
    successful people at a given thing often combine a few related skills.
    For example, the best bloggers of the early Internet were often people who were a
    little bit tech savvy, because that combination of writing ability and HTML skills
    made it easier for them to gain traction.
    It doesn’t mean the core skill of blogging is HTML, but it is relevant to success.
    Later, blogging platforms matured and the most successful writers today are ones
    with discipline and skills to do well promoting their work on Substack.

    The same is likely true of engineering and writing code.
    The most successful engineers of recent years are extremely good at writing code.
    The most successful engineers of the future may combine have a different combination
    of skills.

[^whyfast]: A reasonable question is, why does good engineering mean building things
    *quickly*? Isn’t it more important to build them *right*?

    There are two answers.
    One is a business reason: if you don’t build it quickly, someone else might, and you
    may not have a successful product or company.
    But there’s an equally important and subtle reason: building more quickly means you
    learn more quickly in the process of exploring solutions.
    Engineering is exploration.
    And exploration is directly powered by learning.
    This is the real reason for the classic startup advice to ship fast and iterate.

[^infravsllm]: Another way to think of this: LLM training is generally not the most
    efficient way to design infrastructure, because essential information (such as the
    difficulty of writing code, or how error prone that code is in a given framework)
    simply isn’t in the training data (at least so far).

[^nosilverbullet]: Frederick P. Brooks, [*No Silver Bullet—Essence and Accident in
    Software
    Engineering*](https://worrydream.com/refs/Brooks_1986_-_No_Silver_Bullet.pdf), 1986.

[^techdebt]: Some call this technical debt.

[^english]: Please forgive me: for brevity, I sometimes say “English” to mean *natural
    language*, but of course people use many natural languages with LLMs.
    Since English is used for much of the training data and documentation, it often
    makes the most sense to use English when communicating with LLMs about code.

[^exact]: There are some subtleties to what “exact” means.
    Technically, depending on the scope of what code and parts of a system you’re
    looking at, code is not quite an exact description of the behavior of software.
    For example, how two threads in an application interact with a third-party service
    is not expressed in the code for either thread.
    But for our discussion, the point is that code is an exact description of the logic
    in *that piece* of the software.

[^aug]: *Augmenting Human Intellect: A Conceptual Framework* —\
    https://www.dougengelbart.org/pubs/augment-3906.html

[^uptimevscorrect]: In engineering, “counting nines” traditionally refers to *service
    availability* (uptime): 99.99% uptime means less than 52 minutes of downtime per
    year. However, the concept equally applies to *correctness nines* for critical
    processes.

[^christensen]: Clayton Christensen’s *The Innovator’s Dilemma: When New Technologies
    Cause Great Firms to Fail* (Harvard Business Review Press, 2015) famously discussed
    how successful companies fail to innovate in ways that would disrupt their existing
    business models.

[^bush]: Vannevar Bush, “As We May Think,” *The Atlantic Monthly* (July 1945). This
    essay envisioned the Memex, a device for storing and linking information to augment
    human memory and association.

[^drucker]: Peter F. Drucker, *The Landmarks of Tomorrow* (Harper & Row, 1959). Drucker
    predicted that knowledge work would become the dominant form of work in advanced
    economies.

[^matuschak]: The term “tools for thought” has been explored by several researchers.
    A good article Andy Matuschak and Michael Nielsen, “How can we develop
    transformative tools for thought?”
    (2019). https://numinous.productions/ttft/

[^bridging]: Aviv Ovadya, “Bridging-based ranking” and related work on bridging
    recommender systems.
    https://www.belfercenter.org/publication/bridging-based-ranking

[^sociotech]: The concept of socio-technical systems was developed by Eric Trist and
    Fred Emery at the Tavistock Institute in the 1960s, emphasizing the interdependence
    of social and technical factors in organizational design.

