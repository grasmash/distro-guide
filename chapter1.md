# What is a distribution?

A Drupal [distribution](https://www.drupal.org/developing/distributions) is a tool intended for managing a discrete set of features across more than one Drupal site. Using a distribution makes it possible to quickly set up a complex site. It also permits feature sets to be updated and maintained in a structured way.

For example, an [installation profile for conferences](http://drupal.org/project/cod) might automatically install and configure modules for advanced user registration, attendee profiles, ticketing, and a list of speakers and sessions.

A distribution typically includes the following components:

* An [installation profile](https://www.drupal.org/developing/distributions)
* A set of [modules](https://www.drupal.org/glossary#module)
* A [theme](https://www.drupal.org/glossary#theme)
* Third party [libraries](https://www.drupal.org/glossary#library)
* Documentation

### Technical References
* [Developing installation profiles and distributions](https://www.drupal.org/developing/distributions)
* [Using an installation profile](Using an installation profile)
* [Distribution developers guide](https://www.drupal.org/node/1555384)
* [How to Write a Drupal 7 Installation Profile](https://www.drupal.org/node/1022020)

## Distribution ownership

As the name implies, a distribution is intended to be distributed and implemented by many sites. It is a software product. Consequently, the maintainer of a distribution has the responsibilities of a product owner. 

Distribution maintainers typically have the following responsibilities: 

* Ensuring that the _installation process_ is fully automated and functional.
* Ensuring that all features and processes are _adequately documented_.
* Providing proactive updates for _security vulnerabilities_ posed by any of the included modules, themes, or libraries.
* Providing a mechanism for soliciting or accepting feedback. E.g., bug reports, feature requests, etc.

From a project management standpoint, developing and maintaining a Drupal distribution is vastly different that developing a single Drupal site.

