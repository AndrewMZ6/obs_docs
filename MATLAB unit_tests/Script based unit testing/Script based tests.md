#script-based-tests #unittests


Conventions of test scripts:
- The name of the test script ***must*** start or end with the word `test` (case insensitive)
- Each test is placed in different sections of the script (sections are defined with `%%`)
	- The first test is considered to be the section after the first `%%` 
	- Anything before `%%` is considered to be *shared* between tests *preconditions*
	- Each test **resets** the shared variables at the start of it's section
	- Variables defined in one test **cannot** be accesed by other tests
- Each test consists of set of [[Assertions]]



An example is reffered here: [[Test Example]]

