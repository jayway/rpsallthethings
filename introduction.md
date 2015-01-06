---
layout: page
title:  "Introduction"
---

## Background

Initially when starting to learn more about Domain Driven Design and had discussions around which patterns to apply it often came down to "it depends". What we realized was that in order to have meaningful discussions we needed a concrete domain in which to apply the patterns. Our initial attempt was to model a restaurant with menus, reciepes, inventory etc, incidentally while eating a pizza. Although we like pizza, we realized that this domain was a bit boring. We couldn't really motivate why we needed to apply CQRS and event sourcing for a single restaurant. What we wanted was a domain that:

* is fun
* has inherent challenges, eg many concurrent users
* is simple and easy to understand
* has room for exploration

What we came up with was the domain of "Internet scale Rock-Paper-Scissors". The idea is a two player game where each player selects either Rock, Paper or Scissors. The players make their decision in secret and then their move is revealed at the same time. Depending on certain rules a winner is selected. If you want to learn more about the game, then you should have a look at the hilarious site [worldrps](http://www.worldrps.com/game-basics) or perhaps the more advanced rules as [explained by Sheldon in Big Bang Theory](https://www.youtube.com/watch?v=fqlDc2VICZ0&t=0m21s).

## What is this site?

It turns out that it is useful to have a common domain while exploring different subjects. By comparing different implementations it becomes easier to understand the advantages with a certain programming language, a new kind of database and so on. We have now used this domain in all kind of explorations, for example:

* [Eventsourcing](http://www.jayway.com/2013/03/08/aggregates-event-sourcing-distilled/)
* [Datomic](http://www.jayway.com/2013/08/20/commands-and-aggregates-in-datomic/)
* [F#](http://www.jayway.com/2014/10/16/exploring-f-through-modeling-4/)
* [REST and hypermedia](http://vimeo.com/99524301)

The goal of this site is to collect all these experiments in one place and encourage others to do their own experiments using the same domain. Besides blogs and presentations we also intend to have live versions of our different implementations. Perhaps using a message based microservice architecture that you can experiment with? 

## What is not in scope?

One of the purposes is to explore different architectures and sometimes you also only want to explore a part of the domain. This means that all solutions will not be identical, since different tradeoffs are made. For example, it would be very interesting to see how a classic SQL + Spring MVC solution compares to an event sourced solution. What is easy to do with SQL? With events?

Another thing that is not in scope is to update old blog posts and code bases as we learn more about the domain or some technique. New entries will of course reference old material! As always, please note the time when things were published and be aware the newer material may be available. The purpose of this site is only to make it easier to find the various experiments.

## Projects

Interested? Then go check out the [Projects](../projects/).

