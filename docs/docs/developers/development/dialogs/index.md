# Dialogs

The Dialogs framework which is a part of WebSight CMS that allows developers to define dialog field components. You can use these components to build the dialogs for submitting data that is saved in content resources.

WebSight CMS delivers a set of ready-to-use components for the purpose of working with dialogs. Use the navigation menu on the left to view the subsections of this Dialogs documentation to learn more details on each Dialogs component.

An example dialog structure definition looks like this:
```json
{
  "sling:resourceType": "wcm/dialogs/dialog",
  "tabs": {
    "sling:resourceType": "wcm/dialogs/components/tabs",
    "properties": {
      "sling:resourceType": "wcm/dialogs/components/tab",
      "label": "Properties",
      "title": {
        "sling:resourceType": "wcm/dialogs/components/textfield",
        "label": "Title",
        "name": "title"
      },
      "description": {
        "sling:resourceType": "wcm/dialogs/components/richtext",
        "label": "Description",
        "name": "description"
      }
    },
    "advanced": {
      "sling:resourceType": "wcm/dialogs/components/tab",
      "label": "Advanced",
      "shadows": {
        "sling:resourceType": "wcm/dialogs/components/toggle",
        "name": "shadows",
        "label": "Use shadows"
      },
      "style": {
        "sling:resourceType": "wcm/dialogs/components/select",
        "label": "Style",
        "name": "style",
        "primary": {
          "sling:resourceType": "wcm/dialogs/components/select/selectitem",
          "label": "Primary",
          "value": "primary"
        },
        "secondary": {
          "sling:resourceType": "wcm/dialogs/components/select/selectitem",
          "label": "Secondary",
          "selected": true,
          "value": "secondary"
        },
        "link": {
          "sling:resourceType": "wcm/dialogs/components/select/selectitem",
          "label": "Link",
          "value": "link"
        }
      }
    }
  }
}
```

This will result in the following UI dialog: 

![Dialog example tab1](dialog-example-tab1.png)

![Dialog example tab2](dialog-example-tab2.png)

Again, learn more about available fields and options by exploring the subsections of the Dialogs section of the documentation, which you can access using the navigation menu on the left.
