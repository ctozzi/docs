# Rich Text Editor

**wcm/dialogs/components/richtext**

## Description

The Richtext component provides many features that allow authors to edit text content.  

The component requires a [configuration](./richtext-editor-configuration.md/) that defines which features should be available and how the menu bar should appear.

## Properties

- **name** -  `string` (required)  
    Form field name

- **label** - `string` (optional)  
    Display label value

- **required** - `string` (optional, default `false`)  
    Indicates if field value is mandatory

- **removeIfEmpty** - `string` (optional, default `false`)  
    Indicates if the property in JCR will be removed if it contains an empty string, or will be kept with that value

- **description** - `string` (optional)  
    Display description value as tooltip

- **configuration** - `string` (optional, default `/apps/wcm/dialogs/components/richtext/configuration`)  
    Absolute path to configuration node. The configuration can be also defined inline; see [RichText Editor - configuration](./richtext-editor-configuration.md/) for details

Example:

```json
"content": {
  "sling:resourceType": "wcm/dialogs/components/richtext",
  "name": "content",
  "label": "Content"
}
```

![RichText Editor](rte1.png)
