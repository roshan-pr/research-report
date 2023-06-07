
# Monitoring

### What is monitoring?

 Application performance monitoring is a process that ensures that a software application is performing all its processes as expected. This is done by identifying, measuring, and evaluating its performance and then providing the necessary information to isolate and resolve any abnormalities.


### What to monitor?

- There are all sorts of metrics generated by apps as they run, and part of the challenge of monitoring performance with a view to optimizing it is knowing which stats to focus on. 

- Hardware resource usage monitoring should be a priority, as if your server’s CPU is being pushed to its limits, the memory is near capacity or the I/O activity is spiking in unexpected ways, we  will know that something is awry. 

- Checking in on general app availability and uptime is also worthwhile. This is not just important for moment-to-moment performance, but also to give you an overview of app performance over longer periods. 

- Taking a broader view can help you see patterns which would otherwise be obscured.  


### Why monitoring is important?

- Alerts us to downtime before it occurs and prevents outages..
- Provides insight into complex Enterprise Resource Planning landscape.
- Aligns with cloud-based ERPs’ continuous development and updates process.
- Enhances the performance and stability of all your integrations.

### Popular Tools for monitoring :-
- Datadog
- Newrelic
- ManageEngine
- AppDynamics
- Dynatrace
- IBM’s performance management tool


—------------------------------------------------------------

One of the biggest arguments for testing and monitoring in production is the fact that testing and production environments will always be different.
Teams spend a lot of time building test environments that perfectly replicate production with things like hardware provisioning and automated deployment scripts. But let's face it, there will always be differences, and even the smallest differences can have a huge impact on the data you collect in your tests.


#### How these differences affect your testing:
Traffic load with real user requests
Monitoring in production helps you measure how your application is performing during peak and low traffic hours. With web applications, slow response times can make new users and customers frustrated. This is a concern for QA, and generally it's near impossible to exactly replicate traffic load in test and staging environments.
Latency with production databases
Databases in production often contain more (or different) data than testing environments. Latency in a database can cause weird errors that may not have been caught pre-production. Seeding data in testing environments is always a good idea, but it's not the same as production data.
Stub components in test environments
Many teams have stub components built-in to test certain parts of an application in isolation. This is especially true for large web applications that rely on external APIs and services. When these components are moved from test to production, there's a million little pieces between them that may behave differently than expected.