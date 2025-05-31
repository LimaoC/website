---
title: "GeneralizedJacksonSim.jl"
summary: "A discrete event simulation engine for a generalized Jackson network built in Julia"
date: "2022-10-21"
tags: ["discrete event simulation"]
readTime: true
---

[Jackson networks](https://en.wikipedia.org/wiki/Jackson_network) are a type of stochastic model that is used to model queuing systems. A network consists of a number of queues, which can have varying service rates and queue lengths. Jobs receive service at queues and can travel between queues after being serviced or leave the system.

*Generalized* Jackson networks relax some of the assumptions on the distribution of transitions between nodes and the distribution of service times. In particular, here we investigate the effect of varying the squared coefficient of variation of the service processes on queue sizes. We model this using a discrete event simulation engine, which can be used to estimate the total mean queue length via simulation.

This was a [MATH2504](https://courses.smp.uq.edu.au/MATH2504/) group project that I worked on in 2022 Semester 2.

---

* <a href="https://github.com/LimaoC/GeneralizedJacksonSim.jl/" target="_blank">GitHub</a>
