replace-bundle-webpack-plugin-edited
===
replace string for webpack compiled bundle, different with string-replace-webpack-plugin, this plugin is run at depends modules compiled, so you can replace any string, even   `require`.
---

original code from : https://github.com/kimhou/replace-bundle-webpack-plugin
fixed code from : https://github.com/Kearns/replace-bundle-webpack-plugin

### i did not do anything, except publish to npm

#  Example Usage
```js
var ReplaceBundleStringPlugin = require('replace-bundle-webpack-plugin')

plugins: [
    new ReplacePlugin([{
        pattern: /window.require/g,
        replacement: function () {
            return 'require';
        }
    }])
]

```
