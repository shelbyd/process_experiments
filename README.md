## Purpose

I've been thinking a lot lately about the approaches we use for developing software (and systems in general).
Many practices have clear benefits to their practitioners, TDD, refactoring, functional programming.
But, I'm curious about optimizing the higher level algorithm of software development.

My goal is to find the best "system algorithm" that:
given a software system, change its behavior, such that existing (desired) behavior is preserved, and subjective experience is maximized.

## Approach

I'll implement the same set of behavior changes, in the same order, with different algorithms and compare the approaches afterwards.
I'll be focusing on my subjective experience of these approaches, since I'll have far too little data to draw any scientific conclusions.

I'll implement the systems completely in one algorithm before moving on to the next.
Sequences of commits in this repository will show the evolution of the system inside each algorithm.

## Project

To draw any useful conclusions about software projects in general, we must implement something more complex than a single module.

### Spec

I'll be making a command line twitter client modeled after Gary Bernhardt's [Toot, reconstructed here](https://github.com/bf4/toot).
This will be enlightening because it:

- includes networking
- integrates with an external api
- requires user interaction
- can be command based or interactive
- can require posting to an external api
- can become realtime
- can use a local mock api for QA testing

### Constants

To minimize explorable surface area, all implementations will:

- Be written in rust
- Target the same behavior
- Target behavior in the same order
- Only consider existing and next desired behavior, not known future modifications
- Attempt to not reuse knowledge learned from previous examples with regards to architecture

## Approaches TODO

Notes for me.

- [ ] Control (do what feels right)
- [ ] Cowboy coding
- [ ] Functional core imperative shell
- [ ] Make the change easy, make the easy change
- [ ] Write desired code, then integrate
- [ ] Inside out
- [ ] Outside in
- [ ] Simplest thing that could possibly work
- [ ] Easiest change
- [ ] KISS
- [ ] YAGNI
- [ ] Full BDD/TDD
- [ ] Recursive TDD
- [ ] Design up front
