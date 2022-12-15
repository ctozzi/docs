# Select

**wcm/dialogs/components/select**

## Description

The Select component allows the user to choose one of several options.

## Properties

- **name** -  `string` (required)  
    Form field name

- **label** - `string`(required)  
    Display label value

- **required** - `string`  
    Indicates if field value is mandatory

- **description** - `string`  
    Display description value as a tooltip

It should contain child nodes with options:

# SelectItem

**wcm/dialogs/components/selectitem**

## Description

Defines one of the available options.

## Properties

- **label** - `string`(required)  
    Display label

- **value** - `string`(required)  
    Value of choosen option

- **selected** - `string`  
    Indicates if field is selected by default. By default, this option will not be saved in the properties unless the user selects an option manually. Thus, in order to make this work smoothly, we should use the same default value in the backend as well.

## Example

```json
"icon": {
  "sling:resourceType": "wcm/dialogs/components/select",
  "name": "socialLinkIcon",
  "label": "Social Link icon",
  "linkedin": {
    "sling:resourceType": "wcm/dialogs/components/select/selectitem",
    "label": "LinkedIn",
    "value": "icon-linkedin"
  },
  "facebook": {
    "sling:resourceType": "wcm/dialogs/components/select/selectitem",
    "label": "Facebook",
    "value": "icon-facebook"
  },
  "twitter": {
    "sling:resourceType": "wcm/dialogs/components/select/selectitem",
    "label": "Twitter",
    "value": "icon-twitter"
  },
  "instagram": {
    "sling:resourceType": "wcm/dialogs/components/select/selectitem",
    "label": "Instagram",
    "value": "icon-instagram"
  }
}
```
