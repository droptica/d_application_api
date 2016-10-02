Service: Revert(Import) a feature programmatically - Drupal 8

\Drupal::service('d_application_api.features')->import($modules);


Example usage:

```
<?php

/**
 * Update 8002
 */
function mymodule_update_8002() {
  \Drupal::service('d_application_api.features')->import(['feature_module_1', 'feature_module_2']);
}
```
