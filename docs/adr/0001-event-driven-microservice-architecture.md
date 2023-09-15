---
tags: [adr]
---

# 0001 Event Driven Microservice Architecture

* Status: accepted
* Deciders: Valentyn Kuznietsov, Michael Eder, Andreas Eger

## Context and Problem Statement

The startup builds a product that plans to accomodate more than 15 million user accounts. 

The nature of product involves high amount of async workload. For example, the system is expected to poll user emails every 5 minutes or less, analyze bookings of users to compose them into trips, and provide analytics on this data.

Additionally, the system will integrate many different travel agencies that will pipe bookings information into the system. Each integration must be encapsulated.

The system should also have very high uptime, which means ability to failover in case of failing instances, and independently deploy different bits of functionality.

## Decision

We will use a microservice architecture. Microservices will communicate via an event bus. Microservices will be scaled (in number) proportionally to number of users.

## Consequences

n/a

## Links

n/a
