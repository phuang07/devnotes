# Drupal

## Debug
```
// Debug entityQuery
// Enable devel module, add `$query->addTag('debug')`
// The query string would display on the message block section
 
$query = $this->entity_query->get('node');
$query->condition('status', NODE_PUBLISHED);
$query->addTag('debug');
$query->execute();

```
