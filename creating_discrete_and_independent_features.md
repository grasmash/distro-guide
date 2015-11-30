# Creating discrete and independent features

You distribution will provide a suite of features. Client site should be able to opt-in or opt-out of using any single feature. Additionally, they should be able to override any given feature to meet their own unique requirements.

This only possible if features have been intentionally designed to be discrete and independent. Feature dependencies should be carefully considered! Specifically, observe the following principles:

* Features should be made as small as possible.
* Each feature should have as few dependencies as possible.
* All dependencies should be one-way. Circular dependencies should never exist.

### Common mistakes

* Creation of large features that encompass many components. E.g., content types, views, roles, permissions are all bundled into a single feature.
* Poor design of dependencies
  * Creation of circular dependencies.
  * Each feature has too many dependencies, so no one feature can be used in isolation.
    * Poor separation of field bases and field instances. E.g., the "Workflow" feature depends on the "Press Room" feature because it requires field_body which is provided by "Press Room."
