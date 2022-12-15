# Text Field

**wcm/dialogs/components/textfield**

## Description

The Text Field component allows user to enter text within a field.

## Properties

- **name** -  `string` (required)  
    Form field name

- **label** - `string`  
    Display label value

- **required** - `string`  
    Indicates if field value is mandatory

- **removeIfEmpty** - `string` (if not defined `false`)  
    Indicates if the property in JCR will be removed if it contains an empty string, or will be kept with that value

- **description** - `string`  
    Display description value as tooltip

## Example

```json
"title": {
  "sling:resourceType": "wcm/dialogs/components/textfield",
  "name": "title",
  "label": "Title"
}
```
