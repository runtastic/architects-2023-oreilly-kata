---
tags: [adr]
---

# 0003 Multi Region

* Status: accepted
* Deciders: Valentyn Kuznietsov, Michael Eder, Andreas Eger

## Context and Problem Statement

The product should ensure certain response time, as well as should be able work internationally.

## Decision

Most cloud providers group their data centers into geographic regions (e.g. frankfurt). Regions then typically consist of three or more availability zones (AZ), being distinct data centers but co-located in this region. Typically direct connectivity between AZs within a single region is given and resources can be easily managed within a region without great architectural effort. Distributing resources across multiple regions is way more complex, introducing, among other restrictions, higher cost, high(er) latency, no direct connectivity, etc. 

Multi region also introduces the need for a more complex architecture. The increased cost and maintenance effort would be too much for a new startup. 

## Consequences

Do not deploy services in multiple regions. To match the expected resonse times, employ caching and CDN, if needed. 

## Links

n/a
