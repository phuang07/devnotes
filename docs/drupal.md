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

## Json API

### Questions
Does json api restrict access to unpublished content?
No.


### References
* https://www.youtube.com/playlist?list=PLZOQ_ZMpYrZsyO-3IstImK1okrpfAjuMZ
* https://drupalize.me/tutorial/what-are-web-services?p=3003
* [An very good overview on Authentication and Authorization](https://drupalize.me/tutorial/api-authentication-and-authorization?p=3003)
* [jsonapi.org](https://jsonapi.org)

