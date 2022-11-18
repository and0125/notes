# API Notes

## Intro to APIs

Application programming interfaces are meant to define the ways computer systems interact. Web APIs allow these interactions to be exposed over a network and used remotely by lots of people.

The tough trade-off of web APIs is that the builders have a lot of control over the interactions, and the users have very little control.

The advantage in this is that it keeps propriatary data handling methods behind a wall; exposing only the output of these methods to the user.

APIs are important because they allow computers to interact in an automated manner without requiring human intervention.

Many web based APIs act like waiters, they perform a call and serve some data. These are called Resource-oriented APIs. REST-oriented APIs are a type of resource-oriented API.

Resource-oriented APIs are contrasted with Remote Procedure Call (RPC) APIs. RPC APIs are oriented around the actions a user wants to perform, rather than the data a user wants to receive. A resource-oriented API is an RPC, but with a clear and standardized pattern of access controls.

These standard patterns of control are:

- creating a resource
- getting a specific resource
- listing all instances of a specific resource
- deleting a specific resource
- updating a specific resource

These are aligned to the HTTP methods GET, POST, PUT, PATCH, and DELETE.

These patterns allow users to learn the API faster and access more of the functionality of the API more quickly.

## What Makes an API Good?

This is often two simple points:

- the API has funcitonality that users want
- Those users want to use this functionality programmatically

Additionally, APIs should meet:

- operational requirements: it must do what the users actually want
- non-operational requirements: it must meet some performance requirements that may be outside of the main functionality. Like be interpretable into different languages; have documentation available; return data within a certain time window, etc.
- Expressive requirements: a user should be able to dictate exactly what they want the API to do and even how they want that to be done.
- Simplicity requirements: the API should provide the functionality that users want in the most straightforward way possible, but not simplify to the point of obfuscating the user's interaction with the API.
  - try not to add more endpoints than necessary, but as many as required to achieve the functionality required.
- Predictable: APIs should rely on repeated and predicatable patterns because they are easier and faster to learn, and that makes them more efficient.
  - this means maintaining names, and naming things in easy ways.
