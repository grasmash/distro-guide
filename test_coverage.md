# Test coverage

Software testing has been around for decades, and it has been proven to provide many crucial benefits, including:

* Reduce the number of bugs and regressions
* Increase project velocity (in the long run)
  * Improves accuracy of scheduling estimates
  * Saves time and money
* Increase user trust and satisfaction

You should use automated testing. Do not fall prey to common rationalizations and excuses relating to insufficient time, money, or resources. Time spent developing tests is repaid ten fold.

> Quality is the ally of schedule and cost, not their adversary. If we have to sacrifice quality to meet schedule, it’s because we are doing the job wrong from the very beginning.
>
> -- <cite>James A. Ward</cite>

> The bitterness of poor quality remains long after the sweetness of meeting the schedule has been forgotten.
>
> -- <cite>Karl Wiegers</cite>

That being said, two important things should be acknowledge.

1. It is possible to do automated testing incorrectly such that it is too expensive. See [Why Test Automation Costs Too Much](http://testobsessed.com/2010/07/why-test-automation-costs-too-much/).
2. It is possible to write automated tests that have little value.

This document will avoid becoming a treatise of correct automated testing practices. Suffice it to say that due diligence should be done to ensure that testing is implemented properly on both a project and a developmental level.

### Types of testing

It is suggested that you use the following types of automated tests for your distribution:

* [Code sniffing](https://www.drupal.org/project/coder)
* Code linting
* Functional tests
* Unit tests

## Functional testing

Functional tests will be written with [Behat](http://docs.behat.org/en/v2.5/) using a [Behavior Driven Development](http://dannorth.net/introducing-bdd/) methodology.

The high-level purpose BDD is to create a strong connection between business requirements and the actual tests. Behat tests should mirror ticket acceptance criteria as closely as possible.

Consequently, proper Behat tests should be written using business domain language. The test should be comprehensible by the stakeholder and represent a clear business value. It should represent a typical user behavior and need not be an exhaustive representation of all possible scenarios. 


## Unit testing

@todo This whole section

### Resources

* @todo Add Behat testing best practice resource
* @todo Add sources for claims to improvements in velocity.
* 