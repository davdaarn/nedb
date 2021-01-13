## NeDB Electron

This is a simple fork of [Louis Chartriot's](https://github.com/louischatriot) [NeDB](https://github.com/louischatriot/nedb).

The only change made was the removal of the following code from `package.json` to allow setting custom db paths from the renderer process.

```javascript
...
  "browser": {
    "./lib/customUtils.js": "./browser-version/browser-specific/lib/customUtils.js",
    "./lib/storage.js": "./browser-version/browser-specific/lib/storage.js"
  },
...
```