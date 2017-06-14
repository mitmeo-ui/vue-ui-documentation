> Working in progress

# Component name: `vui-button`
```
export default {
  name: 'vui-button',
  data() {
    // ...
  },
  // ...
}
```
# Composition
> N/A
# Props
| Name | PropType | Required | Default | Description |
|------|-----------|----------|---------|-------------|
| type | string | NO | `'default'` | Look 'n Feel of the button. MUST handle `'default', 'primary', 'alternate', 'danger'` types.<br>Non-handled types i.e. no CSS supports from the original framework, should fall back to `'default'` |
| loading | boolean | NO | `false` | Loading state i.e. after a long run submit |
| loading-text | string | NO | `'Loading...'` | Text to show in loading state |
# Events
> N/A