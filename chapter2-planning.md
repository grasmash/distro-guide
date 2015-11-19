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
