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
# Component specifications
* [Button](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/Button.md)
* [MenuBar](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/MenuBar.md)
* [MenuBarMain](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/MenuBarMain.md)
* [MenuBarSide](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/MenuBarSide.md)
* [MenuBarItem](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/MenuBarItem.md)
* [MenuBarSubItem](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/specifications/MenuBarSubItem.md)
# APIs
* [Button](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/api/Button.md)
* [MenuBar](https://github.com/mitmeo-ui/vue-ui-documentation/blob/master/api/MenuBar.md)