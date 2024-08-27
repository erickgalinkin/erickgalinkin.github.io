---
layout: post
title:  "The Future of Software""
date:   2021-10-10 11:23:00 -0500
usemathjax: false
categories: artificial intelligence
---

A friend recently linked me an article on "the end of classical computer science" and it hit on a notion that I think is increasingly common but totally nonsensical -- specifically, the notion that artificial intelligence and modern generative models somehow spell the end of programming.
I spent a bit of time consulting with [Anthropic](https://anthropic.com), an AI safety company on AI security and one of my tasks involved exploring the problem of building generative code models.
One of the things that I did, using one of the best code models in the world, was ask it to write simple programs, then try to compile those programs.
When those programs (inevitably) failed to compile, I provided the errors back to the model and asked it to fix the errors. 
What happened was that while, in general, the model performed well in terms of diagnosing the errors it encountered, it frequently failed to write fixed code. 
One would be forgiven for thinking that this implies that we are very close to solving the problem, and I'll explain why it is not so simple and why we should not fear robotic programming.


