# Forward compatbility

As a distribution owner, you are responsible for providing an upgrade path to your users. I.e., if you release a new feature or update an existing feature, your users should be able to easily implement those updates.

All features should have a well defined upgrade path. E.g., version 1.0 of the "Press Room" feature should be easily and automatically upgraded to version 1.1.
Typically, this is accomplished through:

* Updating a make file.
* Updating a feature module with new configuration.
* Defining update hooks via `hook_update_n()`.
* Providing "Change Log" or "Release Notes" documentation.

### Make files

The preferred method for managing a distribution (or any Drupal project) is via a `drush make` file. There are specific instructions for managing distributions make files are [provided on Drupal.org](https://www.drupal.org/developing/distributions/drupalorg).

### Update hooks

Drupal's [update hooks](https://api.drupal.org/api/drupal/modules%21system%21system.api.php/function/hook_update_N/7) permit a distribution maintainer to execute code during an update. 

This enables all required updates to be performed via Drupal core's update script. Ideally, there should be no additional steps required for a distribution update. This ensures that updates follow a predictable, testable, repeatable process.

### Release notes

Every new release of the distribution should be accompanied by Release Notes or a Change Log. This is an industry standard. It serves the following purposes:

* Documents bug fixes
* Documents new features
* Document change existing to features

This documentation should at a minimum include:

* A release version
* Guidance to users if their experience has changed
* Links to related issues for reference