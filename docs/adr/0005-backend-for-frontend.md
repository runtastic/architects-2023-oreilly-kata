---
tags: [adr]
---

# 0005 Backend For Frontend

* Status: accepted
* Deciders: Valentyn Kuznietsov, Michael Eder, Andreas Eger

## Context and Problem Statement

The product aims to have a richest interface possible for both Web and Mobile clients.

To reduce complexity of implementation of various clients, and impose consistency between them, it makes little sense to implement public APIs in each of the microservices that client needs for their use cases.

It is critical for a startup that aims to build native clients, yet wants to reduce time to market.

## Decision

We use backend-for-frontend pattern that will aggregate required data and present it to clients in the way they need.

## Consequences

It is required to maintain good coding culture and deprecation policy, to be able to add, or remove data in a rigid backend-for-frontend interface.

## Links

n/a
