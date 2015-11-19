## Configuration management

A typical Drupal feature has two components:

1. Code that lives in a module
2. Configuration that lives in the database

To effectively ship a feature as a product, a distribution maintainer must choose a strategy for exporting and shipping the configuration. In Drupal 7, there are two modules that can assist with this task:

1. [Features](https://www.drupal.org/project/features)
2. [Configuration](https://www.drupal.org/project/configuration)

Each of these solutions has its merits. 

### Features (the module)

The features module has been the de facto choice for configuration management in Drupal 7 for many years. 

#### Pros

* Stable, mature, battle-tested.
* Integrates with most major Drupal contributed modules

#### Cons

* _Feature configuration cannot be overridden in a maintainable way_. This can be somewhat mitigated by using the [Features Override](https://www.drupal.org/project/features_override) module.
* Features must be carefully exported to ensure that they are discrete
* Debugging features is challenging
* Relatively poor performance

### Configuration (the module)

## Performance, security, and maintenance

## Test coverage