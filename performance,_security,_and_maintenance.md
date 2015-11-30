# Performance, security, and maintenance



## Performance concerns

* Ensure that your distribution uses recommended modules. E.g., memcache, entity cache, etc.
* Consider default caching settings for pages, panels, views, blocks, etc.
* Carefully watch custom code for typical performance mistakes. E.g., incorrect usage of `hook_boot()` and `hook_init()`

## Security concerns

* Only include full module releases. Alpha and beta releases are not monitored by the Drupal Security Team.
* Carefully watch custom code for typical [security mistakes](https://docs.acquia.com/cloud/arch/drupal-security#animated)
* 

## Maintenance concerns

