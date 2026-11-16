---
layout: single
title: "Conversational AI — but where is the I?"
date: 2019-02-21
permalink: /blog/conversational-ai-but-where-is-the-i/
excerpt: "Why today's conversational AI is Turing-exhaustive rather than intelligent — and what true language understanding requires."
categories: writing
tags:
  - conversational AI
  - NLP
  - deep learning
author_profile: true
read_time: true
---
> Originally published in the [Wluper Blog](https://medium.com/wluper/conversational-ai-but-where-is-the-i-599e2430f42a) on 21 February 2019. This is a lightly reformatted copy; the original remains the canonical version.

I remember the first time I saw a computer. It was a Power Macintosh 5260, with Monkey Island on it. I was around five years old and looked at it as if it belonged to another universe. It did — I was not allowed within a five-mile radius of it. It was my older brother's. That did not stop me. I browsed it for hours. The possibilities of computers were infinite, and the inspiration of sci-fi worlds — **the dream** of talking machines, machines that can assist humans, think for themselves, and even have feelings — **never stopped**. I kept dreaming about the possibilities of the future.

Fast forward 20 years. We saw great leaps in technology: powerful silicon chips, the rise of the internet, and the end of a long AI winter with the dawn of Big Data and deep learning. The unreachable future that was beyond comprehension is starting to become a reality: [flying taxis](https://www.uber.com/gb/en/elevate/), "[Terminators](https://www.youtube.com/watch?v=rVlhMGQgDkY)", [intelligent agents](https://deepmind.com/blog/alphazero-shedding-new-light-grand-games-chess-shogi-and-go/) — just a few things that once seemed unattainable. However, machines that can speak, reason, and think on their own — a core part of any future — are still missing. This state of affairs, and my dreams from a young age, kept pushing me. Two years ago I embarked on my most daring adventure: I joined the journey to help shape the future and build true conversational AI — a journey I am not treading alone, thanks to my team at [Wluper](https://wluper.com).

Conversational AI is a big phrase these days. The Siris and Alexas among us are rising. CES 2019 in Las Vegas was [dominated by voice](https://www.bbc.co.uk/news/technology-46818797). But while they are becoming ubiquitous and embedded in ever more devices, we ask ourselves: where is the intelligence? "Alexa, please flush my toilet?" Really? Deep learning is the magic secret sauce behind many of these advances. There is no doubt that deep learning has been phenomenal; it pushed conversational AI and NLP to a new frontier. Yet I agree with critics such as [Gary Marcus](https://medium.com/u/d7e74ac84d28) who are [skeptical about deep learning](https://medium.com/@GaryMarcus/in-defense-of-skepticism-about-deep-learning-6e8bfd5ae0f1). I am not here to criticise deep learning, but to make a stand and call on people to be critical, to ask the hard questions, and not to be satisfied with the mediocre. The future should be grand.

### Turing Complete or "Turing Exhaustive"

Intelligence is a hard concept to define. It can mean many things, and it has many layers of understanding and discussion. I will not get started on that. A good starting point for intelligence in natural language, however, is Turing completeness: the ability to understand and execute any statement or program. We humans are arguably Turing complete — bar the finite memory and time, and the random (and sometimes stupid) transition function. This means we can express any logical expression to one another and are able to "understand" and "execute" it. This is how we describe the world around us, argue about Brexit and Hawaiian pizza, and debate [Emacs versus Vim](https://en.wikipedia.org/wiki/Editor_war) (undecidable?), although I would call some unnamed people Turing Faulty, to say the least.

Now Microsoft, Google, Amazon, and Apple have billions of devices — or, as they call them, "IPDAs" (Intelligent Personal Digital Assistants). Intelligent? Why is nobody talking about Turing completeness in dialogue systems, and even less so for IPDAs? Even [Minecraft is Turing complete](https://www.youtube.com/watch?v=1X21HQphy6I). You can have a [while loop with Google Home, Siri, and Alexa](https://www.youtube.com/watch?v=vmINGWsyWX0).

Let me introduce "Turing Exhaustiveness" — a neologism in which today's intelligence is achieved by covering every possible eventuality with a bespoke rule or action. We have all seen it: intents and actions. Not only Alexa and Google provide them; many other pioneers and players do so as the core building block of voice assistants. The idea is to describe every permutation of possibilities with a standalone action, every possible human interaction with a standalone rule, to achieve true intelligence. Clearly, Turing Exhaustiveness will never lead to Turing completeness.

### I Am Better Than You (on Average) — or What SOTA Means

But what about machine learning? Yes, machine learning. Machine learning and deep learning are taking care of writing the rules. They are outperforming rule-based and industry-dominated approaches. Hurrah! But let us have a second look at what state of the art (SOTA) means.

These models are evaluated on F1 score, exact match, accuracy. SOTAs are established by outperforming everyone and everything out there — on the average score. Average? Not a score on every use case. But are humans interested in averages over infinite time horizons? I don't think so. It doesn't matter if your system gets stuck in some use case, or that your Google Home is calling the police and you cannot make it stop, as long as you have set the new SOTA.

So where exactly is the problem? What are we humans doing differently? We can easily deal with ambiguity, for one thing. Language is inherently ambiguous. Just think of "Mac". Do I mean an Apple Mac? The makeup company MAC? Or am I really hungry and thinking of mac 'n' cheese? Currently the best solutions try to solve this with confidence thresholds or black boxes. Humans, on the other hand, have interactive dialogues: we ask clarification questions and seek true understanding. SOTAs alone are not going to cut it. A fundamental shift in natural language understanding is necessary to get us closer to intelligence — superficial results will only draw [the wrath of](https://medium.com/@yoav.goldberg/an-adversarial-review-of-adversarial-generation-of-natural-language-409ac3378bd7) [Yoav Goldberg](https://medium.com/u/e6103cf4ea89).

### More Data, Give Me More Data — or How Everyone Is Doing Shallow Understanding

Data is important for machine learning; nobody will have it any other way. But data alone is not going to solve our problems. One can have all the data in the world and nothing good will come of it, especially if one needs annotated data. The problem is that natural language understanding, dialogue state tracking, and similar tasks are done in a shallow way with our beloved deep learning models. The models are performing perception similar to machine vision models, which recognise that there is an apple in the picture but have no clue what an apple actually *is*. The same happens in NLP: current models perceive that a location, a person, or an action was uttered in a sentence, and then the system reacts, but it does not "understand" or "know" what is going on.

More data, deeper models, and hyperparameter tuning (such as random seed) are usually the go-to tools of NLP practitioners — if not whacky rules. Sometimes there is a leap, such as Google's [BERT](https://ai.googleblog.com/2018/11/open-sourcing-bert-state-of-art-pre.html). But fundamentally this is still perception. Understanding whether "somebody can still catch a bus" does not happen via superficial perception of the words "catch" or "bus". Rather, an understanding — a model of the world and the user — needs to exist. Certainly, the user does not mean catching the bus as Superman might. More data is not the solution.

Even with the best data collection and the most advanced deep learning models, all that is happening is mere perception. Defining what [understanding and meaning](https://en.wikipedia.org/wiki/Epistemology) are is not part of this post; I believe due respect needs to be shown to the centuries of philosophers who have dedicated their time to that issue. Instead, I will limit myself to saying that the "I" will not appear by building bigger models trained on more data. I cannot agree more with Kevin Gimpel's quote from [Sebastian Ruder's post](http://ruder.io/4-biggest-open-problems-in-nlp/):

> "I think the biggest open problems are all related to natural language understanding. [...] **we should develop systems that read and understand text the way a person does**, by forming a representation of the world of the text — with the agents, objects, settings, relationships, goals, desires, and beliefs of the agents, and everything else that humans create to understand a piece of text. Until we can do that, all of our progress is in improving our systems' ability to do pattern matching."
>
> — Kevin Gimpel

### Overture

Machine reasoning needs the hardest questions answered; it needs courageous (or crazy) people. We are an underdog, we are just getting started, and we are here to solve these hard problems. Turing exhaustiveness, shallow understanding, and data-hungry models are our enemies. At Wluper, we are critical of the approaches out there and of our own. We believe in working on the fundamental problems in order to achieve true conversational AI. Do you?

Nikolai

*P.s. Keep looking out for more — especially for some of the answers.*

---

*Reference: [Conversational AI — but where is the I?](https://medium.com/wluper/conversational-ai-but-where-is-the-i-599e2430f42a), Wluper Blog, 21 February 2019.*
