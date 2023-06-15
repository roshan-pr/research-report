# What is tracing?

A typical monolithic application consists of a database layer, which is an application layer that is usually exposed via a load balancer. During the development phase, several development teams can work simultaneously at various services within the application, so that they can finally merge all processes into a big monolithic binary and get it deployed for production.

So far so good...until you gradually **scale up the application** and its infrastructure as the traffic picks up or you add new features and make it a complex setup. With **added complexity**, you're almost guaranteed one or more services won’t work as expected or will have performance issues. So it becomes a nightmare to dig into various service logs, co-relate the incident times, and so on.

`Even if you convert your monolithic application into various microservices, the need to crunch the logs to get insights into the microservices is still there.`

Until we know the exact problem and where it lies, it may cause longer downtimes and can affect the MTTR (mean time to recovery). Using a tracing tool can help a ton in such situations, and we are going to talk about this in detail below.

**Tracing an application means logging or collecting required information when the application is executing.** A common tracing framework is integrated with each service or microservice so that they can publish their data to a centralized infrastructure.

`This traced data can be used to visualize for debugging the application or measuring its performance, instead of analyzing various core dumps or stack traces.`

Usually, the tracing tools will have a web-based Graphic User Interface(GUI), which helps you consume or visualize the traced data for reporting purposes, identifying abnormalities in applications behavior, etc.

# Examples
Here is an example visualization in AWS X-Ray: a frontend application interacting with various AWS services like DynamoDB, SNS, SQN, and other microservices. The X-Ray SDK establishes service mapping in between the services as well as records latency data between each other

# Why is tracing important?

In the current landscape of fast-paced Internet with increasing dependencies on microservices and their distributed architecture, it is becoming very important that you have a **common framework for all the deployed microservices** to report their performance and other relevant data to a common platform.

The uniformity in the data will help you co-relate various application data and detect anomalies, both of which are very difficult to achieve without any tracing framework.

Tracing provides a high level of insight into how your application has been running in production and provides valuable information about opportunities for performance improvements.

# We can note some top tracing tools:
- Jaeger
- X-ray(AWS)
- Cloud Trace(GCP)
- Azure Monitor
- Dynatrace
- New Relic.

# What are the drawbacks of tracing?

Though the latest and top-rated tracing solutions are all automated, developers still need to understand how tracing works, what all tools need to be integrated, how systems work, what all features are supported by each tracing solution, etc., all these contributing to a steep learning curve when it comes to mastering tracing.

Also, since your application data is being shared with a 3rd party, it may pose some concerns if the data is sensitive and confidential.

# What benefits come with the visibility that Tracing brings?

- Visual representation of traced data could be very useful to identify anomalies that are usually not possible to detect with traditional service monitoring systems or by attaching debuggers. With some tracing features, you can follow request paths to pinpoint what is causing performance issues and detect where high latencies are occurring.
- Tracing works **across multiple applications** and programming languages; i.e. React frontend service can pass the traces to Python backend applications over HTTP, RabbitMQ, WebSockets, or other transports and all of the relevant information can still be uploaded, processed, and visualized by the same tracing engine.
- **Developer productivity and output are significantly improved** by making it easy to understand the behavior of applications. Tracing tools are easy to integrate with existing code base as it has support for various programming languages and they will help you and your team drastically reduce time spent debugging and troubleshooting issues with your systems.
- Another important point: the tracing helps significantly **reduce the MTTR** (Mean Time To Recover - the average time it takes to recover from a product or system failure) by facilitating cross-team communication, and thus improving the ability to get to the root cause of the incident much faster.

