# Performance and security

As a distribution owner, you are responsible for all of the sites that use your distribution. Preventing the introduction of a bug, performance issue, or security vulnerability into the distribution should be a major concern. 

These defects may be introduced via a contributed module, or they may stem from custom code or configuration. Regardless, you are responsible for discovering these proactively and providing remediation in the event that a defect makes its way into a release.

To mitigate the risks of such defects, follow these best practices:

* Ensure that all features are covered by automated test (discussed in the next section)
* Review all custom and contributed code that is added to the distribution
* Make frequent small releases rather than infrequent large releases.

## Performance concerns

Some sites using your distribution may support a large volume of anonymous or authenticated traffic. These sites may be hosted on a shared architecture. They may have high traffic events that represent a high business value. Consequently, you should consider how well your distribution will perform in a variety of scenarios.


* Follow Drupal best practices when developing features
* Follow [Acquia best practices](https://docs.acquia.com/cloud/performance) for hosting configuration
* [Use profiling tools](https://docs.acquia.com/articles/using-xhprof-evaluate-code-performance) to identify bottlenecks in application performance 
* [Perform load testing](https://docs.acquia.com/cloud/load) to determine the breaking point for your application
* Consider purchasing a [Performance Audit](https://www.acquia.com/resources/collateral/acquia-performance-audit) from Acquia's Professional Services

### Specific best practices

It is impossible to have a perfectly secure site. All sites have vulnerabilities. As a distribution owner, you must be vigilant for security vulnerabilities. You must both proactively prevent issues and also remediate issues that make it to production systems.

* Ensure that your distribution uses recommended modules. E.g., memcache, entity cache, etc.
* Consider default caching settings for pages, panels, views, blocks, etc.
* Carefully watch custom code for typical performance mistakes. E.g., incorrect usage of `hook_boot()` and `hook_init()`
* Enable caching and set TTLs to sane values

## Security concerns

* Only include full module releases. Alpha and beta releases are not monitored by the [Drupal Security Team](https://www.drupal.org/security-team).
* Monitor [Drupal Security Advisories](https://www.drupal.org/security) for announcements related to modules used by your distribution
* Follow [security best practices](https://www.drupal.org/writing-secure-code) and carefully watch custom code for typical [security mistakes](https://docs.acquia.com/cloud/arch/drupal-security#animated)