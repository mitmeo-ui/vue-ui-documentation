> Working in progress

# Component name: `vui-menubar-item`
```
export default {
  name: 'vui-menubar-item',
  data() {
    // ...
  },
  // ...
}
```
# Composition
* [MenuBarSubItem](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/MenuBarSide.md)
# Props
| Name | PropType | Required | Default | Description |
|------|-----------|----------|---------|-------------|
| item | [item](#item-object) | NO | `null` | Bindable item |
# `item` object
| Property | Data type | Description |
|----------|-----------|-------------|
| text | string | Menu item text |
| icon | string | Menu item icon  |
| command | function | Menu item click callback |
| subItems | array[[item](#item-object)] | Sub menu of the item |
# Events
> N/A