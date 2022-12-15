# Container

**wcm/dialogs/components/container**

## Description:

The Container component allows the user to group multiple elements. It's useful for showing or hiding groups of components.

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
