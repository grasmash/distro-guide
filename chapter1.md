# What is a distribution?

A Drupal distribution is an [installation profile](https://www.drupal.org/developing/distributions) intended for use as tool for managing features and configuration across multiple separate Drupal sites. It typically includes the following components:

* An [installation profile](https://www.drupal.org/developing/distributions)
** A set of functions that provision a new Drupal site upon initial setup
** A set of update functions that are used to roll out configuration changes to existing sites
* A set of [module](https://www.drupal.org/glossary#module), [theme](https://www.drupal.org/glossary#theme), and [library](https://www.drupal.org/glossary#library) dependencies that work in concert to provide discrete features
* Documentation

The maintainer of a distribution has the following responsibilities: 

* Ensure that the _installation process_ is fully automated and fully functional.
* Ensure that all features and processes are _adequately documented_ in a manner that is comprehensible to the intended audience.
* Provide continuous monitoring and proactive updates for _security vulnerabilities_ posed by any of the modules, themes, or libraries required by the distribution.
* Provide a mechanism for soliciting or accepting feedback. E.g., bug reports, feature requests, etc.


# Anatomy of a distribution

