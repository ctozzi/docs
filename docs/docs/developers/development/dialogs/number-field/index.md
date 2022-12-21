# Number Field

**wcm/dialogs/components/numberfield**

## Description

The Number Field component allows the user to enter numbers. If it is empty, the respective property in JCR does not exist.

## Properties

- **name** - `string` (required)  
    Form field name

- **label** - `string`  
    Display label value

- **min** - `string`  
    Minimal value possible to enter

- **max** - `string`  
    Maximum value possible to enter

- **step** - `string` (default value = 1)  
    The value granularity.  
    `number` - greater than zero. Indicates that the field accepts only values at multiples of the step. `"any"` - special value. Indicates that the value can be any number.

- **required**  
    Indicates if field value is mandatory

- **description** - `string`  
    Display description value as a tooltip

## Example

```json
"width": {
  "sling:resourceType": "wcm/dialogs/components/numberfield",
  "name": "width",
  "label": "Width",
  "min": 0,
  "max": 1000,
  "step": 0.01
}
```
