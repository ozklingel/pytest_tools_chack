# pytest_project

- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Debugging](#debugging)
- [Additional Practice](#additional-practice)
- [Feedback](#feedback) - Please create issues to provide feedback!


## Prerequisites
**Install Docker**
  - These tests have been packaged to run with all dependencies
    installed within a Docker container. Due to the use of f-strings,
    this must be run with python 3.6+. The Docker image is based on python 3.7


## Usage
**To run open a shell**

  ```bash

  $ docker-compose build
  $ docker-compose run test sh
  ```


**This will open the docker shell and you can run one of the following commands:**


  *Run the entire test suite*
    
  ``` bash
  $ pytest 
  ```

  *Run the tests for a certain file matching a keyword*
    
  ``` bash
  $ pytest -k <test_file_name>
  ```

  *Run tests while printing all variables and verbose output*

  ``` bash
  $ pytest -vvl
  ```

**To exit the shell**
  ```bash
  $ exit
  ```


## Debugging

1. If you page up `(ctrl + fn)` within the debug output when running `pytest -vvl` or
when encountering test errors, your cursor may stick and be unable to continue 
writing in the docker shell. You can get past this by typing `q` to return to
entry mode in the docker container.


1. If you'd like to debug a piece of code, you can add either of the following built-in functions
   to a section of the code to enter into the pdb debugger while running pytest. 
   * `breakpoint()` (python 3)
   * `import pdb; pdb.set_trace()` (python 2)



- Add validation to the delete function in the fitness log class. First,
refactor your test to account for this.

- Additionally, you may consider contributing to open source projects that use
pytest. If you are new to open source, there are several resources to get
started.

- The awesome for beginners github repository and the first timers only website
contain ideas for beginner-friendly open source contributions.
   - Awesome First PR Opportunities: https://github.com/MunGell/awesome-for-beginners
   - Find open source projects with issues for beginners: https://www.firsttimersonly.com/

- Also, the mediawiki parser library lists issues perfect for someone looking
to get started with open source contributions to their project.


## Feedback
- After watching the course, if you have any feedback, I'd love to hear from
you! Please make an issue on this repository, and I will get back to you. 
