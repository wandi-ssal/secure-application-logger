<div align="center">
  
##  Free version of Wandi-SSAL (Secure Software Adaptable Logger) is a C-Program application framework that validates application log messages during development and deployment

</div>

Software applications use log messages to monitor, analyze and diagnose execution flow. Often these messages contain critical and sensitive information about the behavior and use of data. Current approaches do not do enough to protect this information. Wandi-SSAL provides a secure and adaptable approach to address this and many other logging limitations and challenges. This free version of Wandi-SSAL capabilities is based on a [Patent Software Design Technology](https://www.istech.com/) that:

1. uses C-Program print() style interface that is often used by programmers to log messages.
2. decodes log message strings and arguments into element/value pairs.
3. analyzes element/value pairs for accurate use of log message arguments.
4. validates element/value pairs for unintentional programmer’s misuse of log argument.
5. checks element/value pairs for some attackers printf() malicious patterns.
6. generates log messages for development and deployment environments.
7. uses a [Bound Capability Parameter Validation](Wandi-SSAL-Bound-Capabilities.pdf) to ensure robust and eliable API functions.

How to use [Wandi-SSAL API functions in C/C++ Program application.](Wandi-SSAL-Using-API-Function.pdf)
* Details for [LoggerStartUp()](Wandi-SSAL-API-LoggerStartUp-Function.pdf) function.
* Details for [LoggerAppsMsg()](Wandi-SSAL-API-LoggerAppsMsg-Function.pdf) function.
* Details for [LoggerShutDown()](Wandi-SSAL-API-LoggerShutDown-Function.pdf) function.

Setup [LoggerMessageDefines.txt](Wandi-SSAL-LoggerMessageDefines.pdf) file used by Wandi-SSAL API functions.

Refer to [Wandi-SSAL-examples.c](Wandi-SSAL-examples.c) for detailed application examples.

For Ubuntu Linux OS download [Wandi-SSAL-Install_dst.zip](./Wandi-SSAL-Install_dst.zip) file, unzip it and refer to the **README** file for further installation and execution instructions.

Curent and expanding list of [Wandi-SSAL Capabilities](https://www.istech.com/?page_id=570) for Free and Paid versions.

Contact: **bwoodley@istech.com**
