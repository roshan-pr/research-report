# Modern Infrastructure Challenges to Production Debugging

Today’s infrastructures are becoming more and more distributed. While this is mostly to maintain big applications efficiently, it is difficult to debug because it is difficult to trace the bug back to its source. In a distributed application, there are many moving parts, and when a problem occurs in the system, it must first be isolated to see its origin.

An example of such a phenomenon is serverless computing. Not only does it use a distributed architecture, but it represents an abstraction of the underlying application infrastructure and its abilities. In this architecture, the application is decoupled at the functional level, which is single-purpose, programmatic functions hosted on managed infrastructure.

Therefore, it’s almost impossible for a developer to perform a debugging process in normal conditions because the application does not run in a local environment.

Under these circumstances, developers need to gather enough information to solve the problem directly from the running application (function in case of serverless). Therefore, a remote troubleshooting procedure is required. As mentioned earlier, production debugging can also be done remotely through a remote debugging process.


### Why should you not use “Debug Mode” in Production?

The answer is “performance”. Using Development mode, or enabling debugging on an eSpace in Production, adds debugging symbols to the compiled code. This greatly increasing its size (and therefore how much RAM it uses) as well as significantly slowing down its execution speed. You won’t notice the difference in a development or QA environment, but load hundreds or thousands or users against it and there will be a difference for sure.


### Production challenges:
- Security Concerns
- Inconsistency in data
- Compatability issues
- Resource issues
- Job failures
- Hard to get real time data