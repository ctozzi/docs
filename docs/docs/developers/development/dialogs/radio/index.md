# Radio

**wcm/dialogs/components/radio**

## Description

The Radio component allows users to select exactly one option from multiple available options.

## Properties

- **name** -  `string` (required)  
    Form field name

- **label** - `string`(required)  
    Display label value

- **description** - `string`  
    Display description value as a tooltip

- **required** - `string`  
    Indicates if field value is mandatory

- **removeIfEmpty** - `string` (if not defined `false`)  
    Indicates if property in JCR will be removed if it contains an empty string, or will be kept with that value

It should contain child nodes with options. One of these options will be checked by default. If no option is explicitly configured to be marked as selected by default, the first one will be automatically selected. If more than one option is explicitly configured to be marked as selected, only the first of them will be marked.

# Option

**wcm/dialogs/components/radio/option**

## Description

Defines one of the available options

## Properties

- **label** - `string`(required)  
    Display label

- **value** - `string`(required)  
    Value of choosen option

- **selected** - `string`  
    Indicates if field is selected by default. By default, this option will not be saved in the properties unless the user selects an option manually. Thus, in order to make things work smoothly, we should use the same default value in the backend as well.

## Example

```json
{
  "sling:resourceType": "wcm/dialogs/components/radio",
  "name": "headingLevel",
  "description": "HTML heading level help to communicate the organization and hierarchy of the content (for SEO and accessibility)",
  "label": "Heading level",
  "h1": {
    "sling:resourceType": "wcm/dialogs/components/radio/option",
    "label": "H1",
    "value": "h1"
  },
  "h2": {
    "sling:resourceType": "wcm/dialogs/components/radio/option",
    "label": "H2",
    "selected": true,
    "value": "h2"
  },
  "h3": {
    "sling:resourceType": "wcm/dialogs/components/radio/option",
    "label": "H3",
    "value": "h3"
  }
}
```
