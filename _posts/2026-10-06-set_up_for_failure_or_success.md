---
title: 'Are You Setting Your Team Up for Failure or Success?'
date: 2026-10-06
permalink: /posts/are_you_setting_your_team_up_for_failure_or_success/
tags:
  - EM
---

> Engineering teams rarely fail because of technology alone. For engineering leaders, setting a team up for success means creating the conditions for people to think, collaborate, challenge assumptions, and solve the right problems together.


## Set up for failure

A friend of mine (staff engineer with a decade plus of experience) called me recently to complain and commiserate.  The project he has been working on had a planned launch date of end of September. But that date had come and gone and they were nowhere close to ready. There were many outstanding bugs and capability gaps. 

It turns out he had talked to senior management in April to warn that he thought the project was off-track and wouldn’t hit milestones. And then brought it up with senior management again in May and July. 

His complaints read like a list of engineering management anti-patterns to me:
- **Centralized decision-making**  
    EM acts as the sole thinker/decider, treats ICs as order takers, and doesn’t meaningfully collaborate with staff engineers.
- **Weak technical judgment**  
    EM lacks relevant agentic-AI experience, doesn’t understand or run the codebase, and makes architectural or evaluation decisions without enough technical grounding.
- **No real team operating model**  
    Engineers work in silos, there is little planning or roadmap discipline, and “move fast” becomes a substitute for coordination.
- **Short-term fixes over system design**  
    Everything is framed as a bug, quick patches are preferred over addressing underlying capability gaps, and daily urgency crowds out deliberate engineering.


In my opinion the EM and leadership said they wanted success but evidence points to setting up for failure.

## The Problem May Not Be Technical: Software failure is often a people problem

As Tom DeMarco and Timothy Lister write in *Peopleware* there is rarely a single technological issue to explain failure. More often than not the cause is *sociological*. 

> “The major problems of our work are not so much technological as sociological in nature.” - Peopleware

Failure is usually found in people issues and the human side of the project. So too I think in my friend’s case. My friend complained about the EM, the lack of support from senior leadership, the poor work done by other ICs. But that is all just a symptom of poor engineering team *sociology*. The EM constantly chased down technological issues (the implementation gaps they called “bugs”) rather than building an effective team and solving the people issues. Without managing the sociological part of the work, the technological remains at risk. 

> Most EMs “manage as though technology were their principal concern. They spend their time puzzling over the most convoluted and most interesting puzzles that their people will have to solve, almost as though they themselves were going to do the work rather than manage it. … The most strongly people-oriented aspects of their responsibility are often given the lowest priority. … If you find yourself concentrating on the technology rather than the sociology, you’re like the vaudeville character who loses his keys on a dark street and looks for them on the adjacent street because, as he explains, ‘The light is better there’” - Peopleware

## Software Development Is Knowledge Work

*Peopleware* notes that software development is not production-line work (like making a cheeseburger). People aren’t fungible commodities and the work isn’t “order taking”. ICs have to have their brain in gear. The thinking **is** the job. And fostering effective team dynamics around knowledge-work is an essential foundation. 

> "The more heroic the effort required, the more important it is that the team members learn to interact well and enjoy it." - Peopleware

## The Trap of the Quickest Solution

You present a few different options. Someone asks “what is the quickest?”. It’s a trap. Quickest to addressing this one, very narrow use case or quickest to a robust, holistic, well-architected solution that will address the underlying capability gap. When you put it that way obviously the first will take less time. But the second is probably the better approach. EMs like the above only care about quickest wall-clock approach. They always choose option one.

## Local Optimization Isn’t Optimization

Most computer scientists will recognize this as the Greedy Algorithm assumption. But like finding a shortest path in a graph, only considering the shortest next step, and not considering holistically will often not lead to an optimal solution. 

> “The project that has to be done by an impossible fixed date is the very one that can’t afford *not* to have frequent brainstorms …to help the individual participants knit into an effective whole.” - Peopleware

Taking the time to step back and deliberate about a holistic solution is often more effective, more robust **and quicker**!

## Slow and Deliberate Can Be Faster

10 years ago for my mother’s 80th birthday party my sister-in-law organized a scavenger hunt in the small town my parents lived in. She created teams (1 car each) of all the attendees and gave each a sheet with a list of ~50 things to get a photo of. We were to return within 30 minutes and the winning team would be the one with the most items checked off. I remember that all the teams raced to a car and sped off … except my team. I would have also sped off to get started in a hurry but my older (and much wiser) brother was the driver and said we should take the time to come up with a plan of attack. So we sat in the car went through the list. We collaborated by each tackling a different part of the list - adding notes about where things could be found. And then worked together to create a rough order of operation and set off. We ended up winning. IMO **that** is team-work and that is how to set up for success when the clock is ticking. 

## Setting the Conditions for Success

An EM’s job is not to make every decision. It is not to be the *Tip of the Spear*, “smartest guy in the room” master. The EM’s job is to create the environment where good decisions can emerge from the team. Staff and senior engineers should be treated as *thinking partners*, not just execution capacity. A good EM creates structures for the team to think together.

Speed should be measured at the system level, but by speed of closing individual tasks. Process isn’t bad in itself. Deliberate, effective processes are a precursor to success. The question is whether a practice reduces uncertainty, improves coordination and prevents rework. Spending a small amount of time improving a team’s collective decision making before acting is a real winning move.

The management question shouldn’t be “How do I get everyone to move faster”. It should be “What conditions will allow this team to succeed.”
