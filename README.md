> Working in progress
# What is a Vue UI wrapper
Basically it is just a Vue plugin that takes any suitable vanilla Javascript/CSS UI framework in.

Then "wrap" them into a __standard__ Vue component where the names are consistent across multiple Wrappers, as well as the props and events etc.

It means the consumer of the Wrappers only need to update the `Vue.use(WrapperName)` to switch to another UI without any changes on the consumer code at all.

A Wrapper MUST expose a Vue plugin install point, perhaps the main entry point of the package.json.

Below is an example of a valid Wrapper entry point.

```
// src/index.js

// Also import the original UI JS and CSS here
import 'office-ui-fabric-js/dist/js/fabric';
import 'office-ui-fabric-js/dist/css/fabric.min.css';
import 'office-ui-fabric-js/dist/css/fabric.components.min.css';

import MenuBar from '@/components/MenuBar';
import Button from '@/components/Button';
// ...

export default {
  install(Vue) {
    Vue.component(MenuBar.name, MenuBar);
    Vue.component(Button.name, Button);
    // ...
  },
};
```

This way all Wrappers should register same set of components/names.
# Component specs
* [Button](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specs/Button.md)
* [Menu Bar](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specs/MenuBar.md)
# APIs
* [Button](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/api/Button.md)
* [Menu Bar](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/api/MenuBar.md)