# Planning a distrubution

* Gather requirements
* Determine a feature set
* Communicate plan

## Gather requirements

As with all projects, you must begin by gathering requirements. 

* Ask your intended users which features are most important to them
* Draft requirements from the user perspective
* Consider all user roles/personas. E.g., both the administrative users and the end/public   user.

#### Common mistakes at this stage:

* Defining implementation details rather than requirements. E.g., stating "we need a press release content type" rather than "As a public user, I want to be able to search an archive of press releases."
* Designing the wireframes and mockups before gathering requirements.

#### Resources

* [Write a Great User Story](https://help.rallydev.com/writing-great-user-story) (INVEST)
* [How to write Well-Formed User Stories](https://blog.pivotal.io/labs/labs/well-formed-stories) (Gherkin syntax)

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
