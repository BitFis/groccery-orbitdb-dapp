# Grocery list dAPP [WIP - unstable]

This grocery list is using OrbitDB to synchronize the grocery list entries
between the peers. Generally there are clients and servers, which both are
always also peers. The difference between a client and a servers is its expected
availability. 

The idea is to have a seamless and stable list synchronization between multiple
clients but enable the app user to keep control over the data. The easies way to
provide this is by using existing frameworks and standards.

## Concept [WIP]

**Clients** will connect to the network in unexpected time intervals, while
**servers** are expected to be always online. The server peer enables
synchronization between clients which are never connected at the same time to
the internet.

## Structure [WIP]

| Project | Description |
|--|--|
| ./core | Core implementation used by all peers (server / client) |
| ./backend | Backend server implementation |
| ./android | Android app |

## Features [WIP]

User features:

- CRUD grocery list items
- Connect to "public database store" for easy use [WIP]
- Enable opt-out of "public database store" and use "private database
  store" [WIP]

Technical features:

- CICD [WIP]
- Android App [WIP]
- Dockerized Server [WIP]
- Different "base" Datastore endpoints [WIP]:
  - Django DB endpoint [WIP]
  - GTable [WIP]