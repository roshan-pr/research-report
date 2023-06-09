# Security Concerns

Once you’re generating trace data, you need to send it somewhere. Deploying tracing for your organization requires an understanding of where your software runs—for end users and their clients, as well as on servers—and how it’s operated. You’ll need to understand the security, privacy, and compliance implications of collecting and storing trace data. You may encounter trade-offs in overhead relating to how much data is kept, and how much is discarded through a process known as sampling.

## Logging sensitive information

Traces contain message headers when a message is in scope. When tracing is enabled, personal information in application-specific headers, such as, a query string; and body information, such as, a credit card number, can become visible in the logs. The application deployer is responsible for enforcing access control on the configuration and trace files. If you do not want this kind of information to be visible, you should disable tracing, or filter out part of the data if you want to share the trace logs.

 The following tips can help you to prevent the content of a trace file from being exposed unintentionally:

- Ensure that the log files are protected by Access Control Lists (ACL) both in WebHost and self-host scenarios.

- Choose a file extension that cannot be easily served using a Web request. For example, the .xml file extension is not a safe choice. You can check the IIS administration guide to see a list of extensions that can be served.

- Specify an absolute path for the log file location, which should be outside of the WebHost vroot public directory to prevent it from being accessed by an external party using a Web browser.

