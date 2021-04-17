# UOCIS322 Project 1 #
> **Author: Ellie Yun, yyun@uoregon.edu**

Creating a web server in Python with the following functionalities:
 1. If URL ends with `name.html` or `name.css` (i.e., if    `path/to/name.html` is in document path (from DOCROOT)), send content    of `name.html` or `name.css` with proper http response. 
 2. If `name.html` is not in current directory Respond with 404 (not found). 
 3. If a page starts with or includes one of the symbols(~ // ..),    and that includes the initial forward slash that all requests have,    respond with 403 forbidden error. For example,    `url=hostname:5000/..name.html` or `/~name.html` would give 403 forbidden error.

### How to run and test the server? ###
- Copy the credentials-skel.ini file to credentials.ini,
then edit it to contain correct information including your
GitHub repository URL. 
- Testing can be done by using both automated tests
(the script in the 'tests' directory) and some manual tests.

	-- Test deployment in other environments. Deployment should work "out of the box" with this command sequence:
  ```
  git clone <yourGitRepository> <targetDirectory>
  ```

  ```
  cd <targetDirectory>
  ```

  ```
  make run
  ```
  or
  ```
  make start
  ```

  *test it with a browser now; send a request*

  ```
  make stop
  ```

	-- Alternatively, use the script under "tests" folder to test the
expected outcomes in an automated fashion. It is accompanied by README file and comments (inside tests.sh)
explaining how to test your code.  

### Credits ###

Michal Young, Ram Durairajan, Steven Walton, Joe Istas.

