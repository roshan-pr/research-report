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