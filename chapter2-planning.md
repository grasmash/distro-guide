# Planning a distrubution

* Determine a feature set
* Choose a configuration management strategy
* Build a prototype
* Provide test coverage

## Determine a feature set <a name="determine-features"></a>

The first step is to discover and define the set of features that your distribution will provide. Consider the following questions for each feature:

* Will this feature be used widely across many sites?
* Can this feature be easily toggled on and off? 
* How flexible and configurable should this feature be?
* Does this feature have security or performance consequences?

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

## Configuration management <a name="configuration-management"></a>

A typical Drupal feature has two components:

1. Code that lives in a module
2. Configuration that lives in the database

To effectively ship a feature as a product, a distribution maintainer must choose a strategy for exporting and shipping the configuration. In Drupal 7, there are two modules that can assist with this task:

1. [Features](https://www.drupal.org/project/features)
2. [Configuration](https://www.drupal.org/project/configuration)

Each of these solutions has its merits. 

### Features (the module)

The features module has been the defacto choice for configuration management in Drupal 7 for many years. 

#### Pros

* Stable, mature, battle-tested.
* Integrates with most major Drupal contributed modules

#### Cons

* _Feature configuration cannot be overridden in a maintainable way_. This can be somewhat mitigated by using the [Features Override](https://www.drupal.org/project/features_override) module.
* Features must be carefully exported to ensure that they are discrete
* Debugging features is challenging
* Relatively poor performance

### Configuration (the module)

