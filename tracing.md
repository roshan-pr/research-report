# Tracing

Application traces are detailed records of the actions performed by the application, and of messages about events that occurred during operation of the application.

### Involves:

Specialized use of logging to record info about program's execution


### Used for:

- Debugging, diagnose common problems in S/W

### Used by:

- System administrators
- Technical-support


### Event logging & S/W tracing:

Event logging and software tracing arise from the fact that some of the same technologies are used for both


|Event Logging | S/W Tracing|
|---|---|
Consumed primarily by system administrators | Consumed primarily by developers
Logs "high level" information | Logs "low level" information 
Must not be too "noisy" | Can be noisy
A standards-based output format is often desirable, sometimes even required | Few limitations on output format


Another important consideration for software tracing is performance. Because software tracing is low-level, the possible volume of trace messages is much higher. To address performance concerns, it often must be possible to turn off software tracing, either at compile-time or run-time.

### Special concerns :

- In proprietary software, tracing data may include sensitive information about the product's source code.
- If tracing is enabled or disabled at run-time, many methods of tracing require the inclusion of a significant amount of additional data in the binary, which can indirectly hurt performance even when tracing is disabled.
- If tracing is enabled or disabled at compile-time, getting trace data for a problem on a customer machine depends on the customer being willing and able to install a special, tracing-enabled version of the software and then duplicating the problem.
- Many uses of tracing have very stringent robustness requirements. This is both in the robustness of the trace output but also in that the use-case being traced should not be disrupted.
- In operating systems, tracing is sometimes useful in situations (such as booting) where some of the technologies used to provide event logging may not be available.
- in embedded software, tracing requires special techniques.


