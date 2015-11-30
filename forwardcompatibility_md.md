# Forward compatbility

All features should have a well defined upgrade path. E.g., version 1.0 of the "Press Room" feature should be easily and automatically upgraded to version 1.1. It is your responsibility to provide that upgrade path.

Typically, this is accomplished through:

* Updating a make file.
* Updating a feature module with new configuration.
* Defining update hooks via `hook_update_n()`.
* Providing "Change Notes" documentation.
* 
