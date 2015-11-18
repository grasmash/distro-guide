# Planning a distrubution

* Determine a feature set
* Choose a configuration management strategy
* Build Prototype
* Provide test coverage

## Determine a feature set

The first step is to discover and define the set of features that will be provided by your distribution. Consider the following questions for each feature:

* Will this feature be used widely across many sites?
* Can this feature be easily toggled on and off? I.e., site users and opt in or out of using it.
* How flexible and configurable should this feature be to address the majority of use cases?
* Does this feature security or performance consequences that make maintaining it difficult or risky?

### Example features

#### Press Room

The Press Room feature provides the following components:

* A "Press Room" page that aggregates all site news.
* An RSS feed of the Press Room content.
* An API endpoint for discovering Press Room content.
 
To provide this feature, the following Drupal configuration must be defined:

* Module dependencies:
  *  views
  *  ckeditor
  *  field_group
  *  url
* Exported configuration:
  * "Press Release" content type.
  * "Press Room" view
* Documentation
  * Training materials for site administrator use
  * Technical documentation outlining architecture, configurability, etc.

