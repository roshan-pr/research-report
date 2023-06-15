# Tools

## Tracing

- Atatus
  Atatus is a distributed tracing tool that helps developers monitor, troubleshoot, and optimize their applications by providing detailed insights into how requests flow through a distributed system.

  With Atatus, developers can trace the journey of a request from the client to the server, and from server to server, identifying bottlenecks and performance issues along the way. Atatus provides real-time data visualization and analytics, enabling developers to quickly identify and resolve issues that can impact user experience.

- SigNoz
  SigNoz is a free and open-source APM. It aids in application monitoring & problem-solving for developers. SigNoz provides a uniform UI for metrics and traces so that there is no need to jump between multiple tools such as Jaeger and Prometheus.

- Jaeger
  Uber Technologies developed the distributed tracing technology known as Jaeger. It can be used to monitor distributed systems with microservices.

  Jaeger's visibility into the request flow between microservices allows developers to analyse the performance and behaviour of their applications. To assist developers in locating performance bottlenecks and problems, it is used to collect timing data and logs from several services and present them in a single view.

- Zipkin
  Zipkin is an open-source distributed tracing tool that assists in gathering information on how microservices interact in distributed systems.

  With the help of Zipkin, you can see how requests and responses move back and forth across services as well as how each request performs in terms of latency and response times.

  Zipkin's main feature is the ability to trace a request as it moves across numerous microservices. Teams may detect and fix performance and stability issues by using this information to get insights into how each service performs and how it interacts with other services.

  Grafana or Kibana, which have been set up to operate with the Zipkin data source, can be used in place of Zipkin's simple user interface.

- Grafana Tempo
  Grafana Tempo is an open-source, simple-to-use, and large-scale distributed tracing backend. Together, Tempo and Grafana offer a comprehensive solution for the observability of distributed systems and microservices.

  Tempo is inexpensive to use and has tight integration with Grafana, Prometheus, and Loki. It only needs object storage to run. Common open-source tracing protocols like Jaeger, Zipkin, and OpenTelemetry can all be ingested by Tempo.

  Tempo is highly suited for usage in large, complicated systems since it is optimised for excellent performance and can manage lots of tracing data. It offers a backend that is extremely scalable, highly available, and can be used to store, query, and display trace data.

- NewRelic
  New Relic is one of the first businesses in the application performance monitoring industry. Performance monitoring provides businesses with a variety of options. It provides New Relic Edge for distributed tracing, which may track all of an application's traces.

- HoneyComb
  A data tracking engine called Honeycomb is incredibly quick. Signal graphs that depict events in production allow you to quickly and accurately answer inquiries about what is happening in your system, despite its sophistication and high level of dimension.

  It might only take a single click to enter the tracing view by selecting a trace ID. Regardless of how complicated your system is, Honeycomb offers a seamless picture of every event taking place in it.

- Splunk
  The most remarkable aspect of Splunk is its original and practical AI-driven analytics, which shorten inquiry times by instantly alerting you to important patterns. Three different search options are offered by Splunk: fast, smart, and verbose.

  They give you the best tracing experience possible, with each mode's capabilities tailored based on how meticulous you need to be.
