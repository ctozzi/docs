# Container

**wcm/dialogs/components/container**

## Description:

The Container dialog component allows the user to group elements. It may be useful for showing or hiding a group of components, for example.

## Example:

```json
"container": {
  "sling:resourceType": "wcm/dialogs/components/container",
  "firstelement": {
    "sling:resourceType": "wcm/dialogs/components/textfield",
    "name": "firstelement",
    "label": "First element"
  },
  "secondelement": {
    "sling:resourceType": "wcm/dialogs/components/textfield",
    "name": "secondelement",
    "label": "Second element"
  }
}
```
