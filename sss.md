**TECHNICAL SUMMARY SHEET**

**The free C-Program API Library is easy to use and fail-safe for
applications to generate log messages.**

This C-Program Library is free to use under the MIT License agreement.
It provides a simple printf() style API function interface to generate
application log messages:

  ----------------------------------------------------------------------
  LoggerAppsMsg( DeOp, LogicalName, SeverityLevel, \"Format string
  specification, string specifier value %s\", "string value" );
  ----------------------------------------------------------------------

  ----------------------------------------------------------------------

Technical benefits of this API function:

1.  DeOp directs generating log messages during development, production
    or both.

2.  LogicalName indicates file name, function name or common name across
    multiple files.

3.  SeverityLevel indicates different levels of severity importance.

4.  The remainder of the arguments are similar to printf() style
    specification.

5.  API Arguments Validation:

    a.  Generate log messages to both development and production only.

    b.  Use only LogicalName defined for use by the API.

    c.  Use only SeverityLevel defined for use by the API.

    d.  Decode printf() format string specification for string
        specifiers and match to corresponding arguments.

6.  API Bound Argument Validation:

    a.  Validate length of format string specification to prevent use of
        unbounded strings.

    b.  Validate length of string argument to prevent the use of
        improper NULL terminated strings.

    c.  Validate specific ASCII characters to avoid use of unwanted
        characters in log message.

    d.  Validate against an acceptable set of format string specifiers
        to prevent unsafe and malicious use of attacker string
        specifiers.

7.  Robust and Fail-Safe API:

    a.  Application does not need to check API return status.

    b.  Most failures should not impact application execution flow.

8.  Standard Output Log File Content Format:

  ------------------------------------------------------------
  02/09/2026 12:01:55 \[3650:sample_program\] \[DATABASE\]
  \[INFO\] Message that generates 1 string and 2 integer
  arguments \[String Argument\], \[98\] and \[99\]
  ------------------------------------------------------------

  ------------------------------------------------------------

> where:

+-----------------------------------------------------------+
| "02/09/2026 12:01:55" date and timestamp when the log     |
| message was generated.                                    |
|                                                           |
| "\[3650:sample_program\]" application process id and      |
| name.                                                     |
|                                                           |
| "\[DATABASE\]" logical message group for related          |
| application log messages.                                 |
|                                                           |
| "\[INFO\]" severity for log message.                      |
|                                                           |
| The remainder of the output is derived from the           |
| C-Programming Language printf() format string             |
| specification and corresponding arguments.                |
+===========================================================+

Contact: <bwoodley@istech.com>

Download: <https://github.com/wandi-ssal/secure-application-logger>
