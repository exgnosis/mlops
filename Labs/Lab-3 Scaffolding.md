# Lab 3 - Scaffolding

## Objectives
This lab is a hands-on review of working with continuous integration scaffolding with source code.

_Errata: Due to a naming error, the name of the code repository refers to Lab 2 instead of Lab 3._

Source code for this lab can be found at:
https://github.com/ExgnosisClasses/MLOPSLAB2

The lab should be done in Cloud9 so that the code can be easily viewed.

## Part 1 - Scaffolding
Most programming languages have conventions for organizing project.  In this lab we will look at one such scheme for python. There are many other conventions but they all have the same goals:
1. Make the build and deployments standardized to eliminate human errors and variance in results
2. Reduce work with automated builds and testing
3. Make life easier for us


### Step 1-1 - Walkthrough
The instructor will walk through the example lab with you.

### Step 2-2 - Instructions
Create a virtual environment and activate it
```Console
$ python3 -m venv ~/.lab3
$ source ~/.lab3/bin/activate
```
Download the code into the venv and experiment with the different make commands.

```Console
$ git clone https://github.com/ExgnosisClasses/MLOPSLAB2.git
$ make install
$ make lint
$ make unittest
```
Change the code to cause an error and linting problem as demonstrated and rerun the commands.

There are much more complex scaffolding schemes that allow for deployment as well and conditional steps, like aborting a build if a test stage does not pass because of unit test errors.

---






