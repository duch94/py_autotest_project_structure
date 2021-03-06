# py_autotest_project_structure
This repository describes project structure for SDK testing purposes using python

Here is the description of each directory and file:
* `conf` - this directory is for storing settings and configs, like where you should find test data or what version of SDK you need to test
* `mocks` - this directory is for storing files with mocks/fakes/stubs/expected results. Inside of it you can find 2 files, each file is for storing mocks for each functionality and can used in each regression and other type of tests.
* `sdk_wrapper` - this directory is for storing wrapper, which will translate your python method calls to our SDK method calls
* `tests` - this directory is for storing our test cases. Inside you can find directories like `regression` or `hardware_usage`, where tests of each type are stored, for example
  * `hardware_usage` - test cases for exploring how much hardware our SDK uses
  * `regression` - test cases for testing basic functionality
  * `work_speed` - test cases for exploring how fast our SDK works
* `requirements.txt` - this file is needed to store the dependency list.
* `test_runner.py` - this script is the main file, where we run our test project.
