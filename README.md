# vue-semantic
A collection of vue components for integrating the semantic ui library 
## Contributing
Work In Progress. Any PRs welcome.

## Installation
You can use NPM to install this package
```bash
npm install --save https://github.com/CroudSupport/vue-semantic.git
```
Install the plugin
```js
Vue.use(require('vue-semantic'))
```

You will also need to include the semantic js and css files to your project. The easiest way would be to include them in your html

```html
<link rel="stylesheet" type="text/css" href="semantic/dist/semantic.min.css">
<script src="semantic/dist/semantic.min.js"></script>
```
For more advanced builds see http://semantic-ui.com/introduction/getting-started.html

### Webpack Tips
If you are using webpack, you can add jQuery to your webpack.base.conf.js
```js
plugins: [
  new webpack.ProvidePlugin({
    $: "jquery",
    jQuery: "jquery",
    "window.jQuery": "jquery"
  })
],
```

And include the semantic js + css at the top of your main.js file
```
import 'path/to/semantic.css'
import 'path/to/semantic.js'
```
