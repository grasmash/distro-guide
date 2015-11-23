# Determine a feature set

After you've gathered and documented the distribution requirements, you must translate those requirements into a set of features. 

This document is not intended to fully describe Agile Methodology, but let's briefly review what is meant by "feature" in agile terminology. A feature is a distinct element of functionality that meets a requirement. For instance, you may have documented the following requirement:

> The distribution must provide a Press Room that displays all press releases on the website.
 
 You likely will have documented additional requirements of that feature that will later be expressed as user stories. E.g., 
 
> As a public user, I should be able to comment on a press release. 

Note that we have not expressed any implementation details at this stage.

As a distribution owner, you must analyze all of the requirements and potential features in order to determine which are appropriate for inclusion in the distribution.

Consider the following questions for each feature:

* Will this feature be used widely across many sites?
* Can this feature be easily toggled on and off? 
* How flexible and configurable should this feature be?
* Does this feature have security or performance consequences?

The answers to these questions will determine prioritization, schedule, and ultimately which features are included.

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