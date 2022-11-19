# System Design Notes

## Scalability

Scalability is the ability for a service to scale to handle intense traffic, into the millions of requests, tens of thousands of transactions per second.

### Single Server Design (not scalable)

You can have your database, middleware, and frontend all served on the same server. this may be ok for a personal web server for a personal website, but this would never work for a commercial grade system because this server is a single point of failure.

If this one server goes down everything is lost. To repair, you'd have to provision another server, restore everything to it from a backup, then switch the DNS entry somewhere to point to the new server so that people hit the new server.

This can happen for personal sites too, which can be a pain as well.

This single server design is only suitable for projects that are unimportant and small in scale. Not a choice to use in any interview.

### Separating out the database

This breaks the database out to be separate from the middleware and front-end. A bit better, since the data is not lost if the server goes down.

This doesn't improve the resiliency much, because both the database and the web server are still single points of failures, but it does allow you to scale the database independently of the server.
