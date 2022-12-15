# Text Area

**wcm/dialogs/components/textarea**

## Description

The Text Area component allows users to enter text across multiple lines.

## Properties

- **name** -  `string` (required)  
    Form field name

- **label** - `string` (required)  
    Display label value

- **required** - `string`  
    Indicates if field value is mandatory

- **removeIfEmpty** - `string` (if not defined `false`)  
    Indicates if the property in JCR will be removed if it contains an empty string, or will be kept with that value

- **description** - `string`  
    Display description value as a tooltip

## Example

```json
"content": {
  "sling:resourceType": "wcm/dialogs/components/textarea",
  "name": "content",
  "label": "Content"
}
```
