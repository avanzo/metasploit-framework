## Vulnerable Application

 This module exploits a feature of Splunk whereby a custom application can be
 uploaded through the web based interface. Through the \'script\' search command a
 user can call commands defined in their custom application which includes arbitrary
 perl or python code. To abuse this behavior, a valid Splunk user with the admin
 role is required. By default, this module uses the credential of "admin:changeme",
 the default Administrator credential for Splunk. Note that the Splunk web interface
 runs as SYSTEM on Windows, or as root on Linux by default. This module has been
 tested successfully against Splunk 5.0, 6.1, 6.1.1 and 7.2.4.
 Version 7.2.4 has been tested successfully against OSX as well

## Verification Steps

  Example steps in this format (is also in the PR):

  1. Install the application
  2. Start msfconsole
  3. Do: ```use [module path]```
  4. Do: ```run```
  5. You should get a shell.

## Options

  **Option name**

  Talk about what it does, and how to use it appropriately.  If the default value is likely to change, include the default value here.

## Scenarios

### Version of software and OS as applicable

  Specific demo of using the module that might be useful in a real world scenario.

  ```
  code or console output
  ```

  For example:

  To do this specific thing, here's how you do it:

  ```
  msf > use module_name
  msf auxiliary(module_name) > set POWERLEVEL >9000
  msf auxiliary(module_name) > exploit
  ```
