---
tags: [adr]
---

# 0002 Templated External Service Update Services

* Status: accepted
* Deciders: Valentyn Kuznietsov, Michael Eder, Andreas Eger

## Context and Problem Statement

The system wants to integrate with many travel agencies, including an internal one. All integrations, despite their differences, should have very similar structure and interface.

## Decision

A creation of an integration service should be templated. Developers should not write each integration from scratch but rather use a tool that generates a skeleton of a service.

## Consequences

All integration services look very similar.

## Links

n/a
