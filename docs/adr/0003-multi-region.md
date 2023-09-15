---
tags: [adr]
---

# 0003 Multi Region

* Status: accepted
* Deciders: Valentyn Kuznietsov, Michael Eder, Andreas Eger

## Context and Problem Statement

The product should ensure certain response time, as well as should be able work internationally.

## Decision

The infrastructure setup must allow placement of services in databases in multiple regions. When designing infrastructure, multi-region should be talken into consideration for all services. 

Multi-region must be included not only within the system. It is possible that certain countries will have their own, fully detached infrastructure from other regions, deployed on different infrastructure providers available in this region.

Decision to localize certain services will be done case by case basis.

## Consequences

Some of microservices will have their data compartmentalized due to compliance and performance reasons. 

The system should have a few distributed entry points with geographically routed traffic.

## Links

n/a
