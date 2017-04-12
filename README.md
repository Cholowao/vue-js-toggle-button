### Vue.js 2.0+ toggle / switch button - simple, pretty, customizable.

[![npm version](https://badge.fury.io/js/vue-js-toggle-button.svg)](https://badge.fury.io/js/vue-js-toggle-button)

![Imgur](http://i.imgur.com/a2Hf7pm.png)

Feel free to ask questions or propose features in the "Issues" section

[Live demo here](http://vue-js-toggle-button.yev.io/)

Install:
```bash
npm install vue-js-toggle-button --save
```
Import:
```javascript
import ToggleButton from 'vue-js-toggle-button'
Vue.use(ToggleButton)
```
Use: 
```vue
<toggle-button @change="..."/>
<toggle-button :value="false" :color="#82C7EB" :sync="true" :labels="true""/>
```

### Properties

| Name      | Type              | Default     | Description                        |
| ---       | ---               | ---         | ---                                |
| value     | Boolean           | false       | Initial state of the toggle button |
| sync      | Boolean           | false       | If set to `true`, will be watching changes in `value` property and overwrite the current state of the button whenever `value` prop. changes |
| color     | String            | `#75C791`   | Color of the button when checked   |
| labels    | [Boolean, Object] | false       | If `Boolean` - shows/hides default labels ("on" and "off") <br>If `Object` - sets custom labels for both states. <br>Format: `{checked: 'Foo', unchecked: 'Bar'}`   |
| width     | Number            | 50          | Width of the button, default is 50 |

### Events

| Name   | Description              |
| ---    | ---                      |
| change | Triggered whenever state of the component changes. <br>Contains: <br>`value` - state of the object <br>`srcEvent` - source click event |
