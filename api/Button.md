# Usage
`<vue-ui-button type="primary" :loading="loading" @click.native="click">Button</vue-ui-button>`
# Props
| Name | PropType | Default | Values |
|------|----------|---------|--------|
| type | string | `'default'` | `'default' | 'primary' | 'alternate' | 'danger'` |
| loading | boolean | `false` | `false | true` |
| loading-text | string | `Loading...` | Any text |
# Events
| Name | Args | Description |
|------|------|-------------|
| @click.native | N/A | Just the default Vue click handler.
