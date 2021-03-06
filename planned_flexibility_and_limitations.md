# Planned flexibility and limitations

Define a discrete, limited scope of responsibility for a feature. 

* Intentionally place boundaries on the feature. Don't allow it to exceed it's intended scope.
* Provide flexibility within the feature itself. E.g., provide configuration options that permit administrators and users to modify the feature's functionality without overriding configuration or changing code.
* Assume that at some point, users will need to override and customize a feature. Plan to accommodate that eventuality.
* Carefully place limits on access control

## Common mistakes

* Sharing fields between features. This often created unintended dependencies.
* Mixing global configuration in with a non-global feature.