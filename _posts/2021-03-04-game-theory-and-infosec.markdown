---
layout: post
title:  "Game Theory and Infosec"
date:   2021-03-04 12:37:48 -0500
usemathjax: true
categories: game theory, phd, security
---

So I've decided on a topic for my PhD.
We're going to consider game theory and infosec, which is actually a really exciting intersection of topics.
I gave my candidacy talk [[linked here](/publications/Galinkin_CE_preso.pdf)] on the literature review I did [[linked here](/publications/Galinkin_Candidacy.pdf)], where I identified some shortcomings in the literature and some opportunities to make things better.

In short, the crux of the issue is that by and large, the people looking at security games are thinking about game theory problems which can be used to model security problems, and not security problems that can fit into game theoretic frameworks.
I'm hoping that by coming at this from the other side, we might be able to reconcile some of those near-misses.

One example is that the complexity of security systems is **incredibly** hard to manage.
So what we often see in those cases is that the modelers make a lot of assumptions that simplify the problem, which obviously makes sense!
What gets lost, however are things like "let $$u_d$$ be a utility function for the defender such that..." which misses the incredible complexity of the damage breaches can do.
As another example, consider: "$$\Sigma_d = \{\sigma_1, \sigma_2, ...\}$$ is the set of strategies available to the defender" which again completely loses the intricate dance of security appliances, and what can slip through the cracks.

Meaningfully, there is also a ton of uncertainty in the strategy space as it pertains to attackers.
We can try to infer the capabilities of attackers from what we observe them do - this is more or less the entire field of threat intelligence.
But at the end of the day, if we're a defender, we cannot possibly know the full set of strategies available to the attacker, or at least, it is going to be a very large space.

What really excites me though, is the possiblity of exploring these spaces that explode with uncertainty and figuring out how to solve these optimization problems given all the stochasticity and uncertainty.
There's compositionality to explore - by way of [open games](https://julesh.com/2017/09/29/a-first-look-at-open-games/), some interesting relationships to graph coloring problems, semidefinite programming, and all kinds of computational complexity issues to consider.
On top of that, there are some relationships between the sorts of min-max problems we'll need to examine and reinforcement learning.
Plus, it's a fun and exciting way to pair policy with math.

What really sticks with me, though, is that there is an incredibly rich framework do do mathematics in - more or less any mathematics we'd like - and it all comes with this broad program of making computers safer to use.
Essentially, this could unlock the ability to model security phenomena in such a way that machine learning is more tractable.
I think I'll probably need to write something (at some point) on the intractability of security problems and sketch out the computational complexity of many of these problems.
