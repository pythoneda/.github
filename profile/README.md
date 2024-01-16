# PythonEDA

PythonEDA is an ecosystem of Event-Driven Applications written in Python, following Domain-Driven Design and Hexagonal Architecture.
It applies the as-code principle to Pescio's three-space approach:
- the decision space (your domain), obviously;
- the artifact space (files, changes, repositories, tags, releases) is represented as code;
- the runtime space (how your bounded context gets deployed, monitored, and behaves upon runtime changes).

Additionally, it adopts a different perspective on how software is executed. There's only one way the user interacts with PythonEDA: requesting information about how to execute code. That's the value of PythonEDA: providing the code to fulfill user's requests.
To make the approach more convenient, the user can delegate the provided code to be executed in an automated way on her behalf.

Glossary:
- artifact: the way code is represented and manipulated.
- realm: how each user interacts with PythonEDA.
- domain: a model used to represent a cohesive set of concepts.
- infrastructure: implementations of primary and secondary ports in the domain.
- application: the entity in charge of launching a bounded context with the infrastructure bound to the domain ports.
- shared: A shared module, with no runtime identity.
- event: A relevant fact.
- event-infrastructure: module providing classes needed by the infrastructure layer to support the events.
