# Python Architecture Patterns

## Chapter 1

software architecture is what defines the structure of a software system, and deals with the long-term implications of trading short-term wins for long-term operational performance.

Some considerations to keep in mind when designing software are:

- business vision
- technical requirements
- security concerns
- reliability concerns
- division of tasks (to work in a flexible way)
- use of specific technologies

A software architect is responsible for implementing the application vision and matching it with specific technologies and teams that will develop it. To do this, the architect should keep in mind clear boundaries and facilitate the creation of channels between the system components and follow-up on implmentation details.

The architectural design should happen at the beginning of the application, with a well-thought out design based on the requirements for the product.

## Techniques for System Design

the main technique for software architecture is to divide the whole system into smaller eleents and describe how they interact with each other. Each smaller element or unit should have a clear function and interace.

This division follows the single responsibility principle: every distinct element has a distinct function.

These units then have different requirements and characteristics based on the application's needs.

The most critical and valuable element of a system is almost always the stored data.

## Conway's law

Any organization that designs a system will produce a design whose structure is a copy of the organization's communication structure.
