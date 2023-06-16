# Distributed Tracing 

Distributed tracing is a technique that addresses logging information in microservice-based applications. A unique transaction ID is passed through the call chain of each transaction in a distributed topology.

Distributed tracing helps measure the time it takes to complete key user actions, such as purchasing an item. Traces can help identify backend bottlenecks and errors that are harming the user experience. In microservice architectures, different teams may own the services that are involved in completing a request.

`One example of a transaction is a user interaction with a website.`

> Moving your applications from a monolithic design to a microservices-oriented design introduces several advantages during development and in operations. However, that move has a price. New challenges are introduced, as traditional metrics and log information tend to be captured and recorded in a component and machine-centric way. When your components are spread across machines and physical locations and are subject to dynamic horizontal scaling over transient compute units, traditional tools to capture and analyze information become powerless.
