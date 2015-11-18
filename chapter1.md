# What is a distribution?

A Drupal distribution is an [installation profile](https://www.drupal.org/developing/distributions) intended for use as tool for managing features and configuration across multiple separate Drupal sites. It typically includes the following components:

* An [installation profile](https://www.drupal.org/developing/distributions)
** A set of functions that provision a new Drupal site upon initial setup
** A set of update functions that are used to roll out configuration changes to existing sites
* A set of module, theme, and library dependencies that work in concert to provide discrete features
* Documentation

The maintainer of a distribution has the following responsibilities: 

* Ensure that the installation process is fully automated and fully functional.
* Ensure that all features and processes are adequately documented in a manner that is comprehensible to the intended audience.
* Provide continuous monitoring and proactive updates for security vulnerabilities posed by any of the [modules](https://www.drupal.org/glossary#module), [themes](https://www.drupal.org/glossary#theme), or [libraries](https://www.drupal.org/glossary#library) required by the distribution.


# Anatomy of a distribution

