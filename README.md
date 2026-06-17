<b>IMPORTANT: The content of this site is replaced with the [Fail-safe Application Logger site](https://github.com/wandi-ssal/fail-safe-application-logger). It is the same information from this site, but was updated to include feedback and recommendations I received. For now, I will leave the content of this site as is, but eventaully this information will be replaced with artifacts related to the Secure Software Adaptable Logger work, which is an extension of the free Fail-Safe Application Logger API library to include protecting application log messages while the software is being developed and when running in a deployed environment. Thank you.</b>
<div align="center"> 

<ins>Free version of Wandi-SSAL is a C-Program application library that validates and generates application log message during development and deployment.</ins>

</div>

The primary benefit of this API library over other application loggers, is that it does extensive runtime validation to prevent application from crashing due to common unintentional mis-use of printf() style issues (e.g., passing %s a NULL value, using invalid NULL terminated string value, etc). If any of these runtime validation fails the API function generates an error code and simply returns, allowing the application to continue normal processing.

Refer to [Bound Capability Parameter Validation](Wandi-SSAL-Bound-Capabilities.pdf) to learn more about this robust, fail-safe and reliable API capability.

The library API:

1. uses C-Program print() style interface that is often used by programmers to log messages.
2. decodes log message strings and arguments into element/value pairs.
3. analyzes element/value pairs for accurate use of log message arguments.
4. validates element/value pairs for unintentional programmer’s misuse of log argument.
5. checks element/value pairs for some attackers printf() malicious patterns.
7. generates log messages for development and deployment environments.
8. provides robust, fail-safe and reliable API operations.

Quick how to use [Wandi-SSAL API functions in C/C++ Program application.](Wandi-SSAL-Using-API-Function.pdf)
* Details for [LoggerStartUp()](Wandi-SSAL-API-LoggerStartUp-Function.pdf) function.
* Details for [LoggerAppsMsg()](Wandi-SSAL-API-LoggerAppsMsg-Function.pdf) function.
* Details for [LoggerShutDown()](Wandi-SSAL-API-LoggerShutDown-Function.pdf) function.

Setup [LoggerMessageDefines.txt](Wandi-SSAL-LoggerMessageDefines.pdf) file used by Wandi-SSAL API functions.

Refer to [Wandi-SSAL-examples.c](Wandi-SSAL-examples.c) for detailed application examples using the Bound Capability Parameter Validation.

For Linux OS download [Wandi-SSAL-Free-Install_dst.zip](./Wandi-SSAL-Free-Install_dst.zip) file, unzip it and refer to the **README** file for further installation and execution instructions.

This library is part of another effort to provide [advanced logging capabilities](Benefit-over-other-logging-systems.pdf) over existing logging tools, utilities and systems.

Github repository for [files and downloads](https://github.com/wandi-ssal/secure-application-logger)

Contact: **bwoodley@istech.com**
