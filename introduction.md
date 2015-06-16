---
layout: page
title:  "Introduction"
---

## Background

As we learned more about Domain Driven Design we had discussions about which patterns to apply. Often it came down to "it depends". What we realized was that in order to have meaningful discussions we needed a concrete domain to which we could apply patterns. Our initial attempt was to model a restaurant with menus, recipes, inventory, etc. Incidentally, we had the idea while eating pizza. Although we like pizza, we realized that this domain was a bit boring. We couldn't really motivate why we needed to apply CQRS and event sourcing for a single restaurant. What we wanted was a domain that:

* was fun
* had inherent challenges, eg many concurrent users
* was simple and easy to understand
* had room for exploration

What we came up with was the domain of "Internet scale Rock-Paper-Scissors". The idea is a two player game where each player selects either Rock, Paper or Scissors. The players make their decision in secret and the moves are revealed at the same time. Depending on certain rules a winner is selected. If you want to learn more about the game, have a look at the hilarious site [worldrps](http://www.worldrps.com/game-basics) or perhaps the more advanced rules as [explained by Sheldon in Big Bang Theory](https://www.youtube.com/watch?v=fqlDc2VICZ0&t=0m21s).

## What is this site?

It is useful to have a common domain while exploring different subjects. By comparing different implementations it becomes easier to understand the advantages of a certain programming language, a new kind of database and so on. We have now used this domain in all kinds of explorations, for example:

* [Eventsourcing](http://www.jayway.com/2013/03/08/aggregates-event-sourcing-distilled/)
* [Datomic](http://www.jayway.com/2013/08/20/commands-and-aggregates-in-datomic/)
* [F#](http://www.jayway.com/2014/10/16/exploring-f-through-modeling-4/)
* [REST and hypermedia](http://vimeo.com/99524301)

The goal of this site is to collect all these experiments in one place and encourage others to do their own experiments using the same domain. Besides blogs and presentations we also intend to have live versions of our different implementations. Perhaps using a message based microservice architecture that you can experiment with? 

## What is not in scope?

All experiments will not solve exactly the same problem since different tradeoffs have to be made. One of the purposes is to explore different architectures. Sometimes we only want to explore a part of the domain.

Another thing that is not in scope is to update old blog posts and code bases as we learn more about the domain or some technique. New entries will of course reference old material! As always, please note the time when things were published and be aware that newer material may be available. The purpose of this site is only to make it easier to find the various experiments.

## Projects

Interested? Then go check out the [Projects](../projects/).

## Ideas for future projects

* Microservices och messaging
* Timeseries databases
* Client push (for example when other player has made a move)
* Deployment on different cloud providers
* More about REST API design
* Single page web vs server generated responsive web
