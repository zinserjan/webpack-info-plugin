# webpack-info-plugin

```js

// webpack.config.js

var WebpackInfoPlugin = require('webpack-info-plugin');

var info = new WebpackInfoPlugin({
  stats: { // provide false to disable displaying stats
      // pass options from http://webpack.github.io/docs/node.js-api.html#stats-tostring
      colors: true,
      version: false,
      hash: false,
      timings: true,
      assets: false,
      chunks: false,
      chunkModules: false,
      modules: false
    },
    state: true // show bundle valid / invalid
});

module.exports = {
  entry: {
    ...
  },
  output: {
    ...
  },
  plugins: [
    info
  ]
}
```
