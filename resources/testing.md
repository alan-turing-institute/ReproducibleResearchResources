# Introduction to testing your code
_Reproducible Research Lunch on 12 Nov 2018 by Martin O'Reilly_ 

Here's a list of some of the things that people think about when considering building tests for their code:

* **randomness**: if there's some randomness in your code, how will you get the same results each time over?
* **compare**: is it easy to compare outputs - for example if they have different floating point precision!
* **time to run**: will it take a long time to run all these checks?
* **different systems**: will my code give the same results on different systems?
* **managing test files**: where do I keep the scripts, inputs, outputs etc
* **edge cases**: how will I know I've found all the different reasons why a function could fail!?
* **time to add the tests**: is it worth my time to add these tests? Will anyone use the code again?

## Automating existing sanity checks

## Automated testing frameworks
### Automated testing in Python with pytest
- [Semaphore tutorial](https://semaphoreci.com/community/tutorials/testing-python-applications-with-pytest)

### Automated testing in R with testthat
- [Hadley Wickham guide to testthat](http://r-pkgs.had.co.nz/tests.html)

## Integrating automated testing with Github

## General resources
- The [testing lesson](https://alan-turing-institute.github.io/rsd-engineeringcourse/ch03tests/) of the Turing's [Research Software Engineering with Python](https://alan-turing-institute.github.io/rsd-engineeringcourse/) course.

## Glossary

* **regression** test: is the output the same as previously generated?
* **end to end**, **system**, **integration**: when you run the whole pipeline on a given input, do you get the same output?
* **unit tests**: low level tests for individual functions

To be clear, all of the tests are "regression" tests - they're all trying to check if things are the same!
Usually people will introduce a regression test when something has gone wrong to try to check a) when it has been fixed and b) to check whether the bug comes back in the future!

In our discussion on 12 November, we came up with a rubric that end to end and unit tests are on one axis (low to high level) and regression is another dimension - with test-driven development on the other end of that scale.
It isn't super important though, the point is that you can test at different times and at different scales.
