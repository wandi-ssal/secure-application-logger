NOTE: The original artifacts of this site moved to [Fail-safe Application Logger site](https://github.com/wandi-ssal/fail-safe-application-logger). It is the same information from this site, but was updated to include feedback and recommendations I received. This site will be used for artifacts related to the Secure Software Adaptable Logger work, which is an extension of the free Fail-Safe Application Logger API library to include protecting application log messages while the software is being developed and when running in a deployed environment (as described below).

<div align="center">

  ## Provide a Secure Software Adaptable Logger solution not currently available with existing logging tools, utilities or systems
  
  </div>

***Project goal:*** Protect application critical/sensitive log information from malicious and unauthorize users during software development and runtime deployment. 

***Log message risk:*** Software programs often generate unprotected log messages that contain critical and sensitive information about the execution flow of the software program and the data it uses during execution. Current approaches to protect log messages have been limited to protecting log messages after the software program has generated the log messages and saved to external storage.

***Solution:*** To reduce this exposure, a holistic approach is needed to protect log data during the development of the software programs, during the generation of software program executables, and during runtime execution of executables.

***Result:*** Prevent unauthorized users access to log message data in software programs (during development), executable file stored on disk (from being reverse engineered), and runtime application execution (from monitoring and extracting information).
