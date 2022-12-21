# Toggle

**wcm/dialogs/components/toggle**

## Description

The Toggle comonent allows the user to enable or disable a selected state.

## Properties

- **name** -  `string` (required)  
    Form field name

- **label** - `string`(required)  
    Display label value

- **checkedByDefault** - `string`  
    Indicates if field should be checked by default. Default: “false”.

- **checkedValue** - `string`  
    Defines what value will be saved in JCR if the checkbox is checked. Default: “true” String

- **uncheckedValue** - `string`  
    Defines what value will be saved in JCR if the checkbox is NOT checked. Default: “false” String

- **description** - `string`  
    Displays description value as a tooltip

## Example

```json
"openInNewTab": {
  "sling:resourceType": "wcm/dialogs/components/toggle",
  "name": "openInNewTab",
  "label": "Open in new tab"
}
```
