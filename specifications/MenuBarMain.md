> Working in progress

# Component name: `vue-ui-menu-bar-main`
```
export default {
  name: 'vue-ui-menu-bar-main',
  data() {
    // ...
  },
  // ...
}
```
# Composition
* [MenuBarSearch](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/MenuBarSearch.md)
* [MenuBarItem](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/MenuBarItem.md)
* [MenuBarSubItem](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/MenuBarSubItem.md)
# Props
| Name | PropType | Required | Default | Description | Requirement |
|------|-----------|----------|---------|-------------|-------------|
| search | function | NO | `null` | Search callback |  |
| search-placeholder | string | NO | `Press Enter to search...` | Placeholder shows on the search box | |
| items | array[[item](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/MenuBarItem.md#item-object)] | NO | `null` | Bindable items list | |
# Events
> N/A