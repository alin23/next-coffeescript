# Next.js + Coffeescript 2

Use [Coffeescript](http://www.coffeescript.org/) with [Next.js](https://github.com/zeit/next.js)

> This plugin uses `coffee-loader`.

# Notice
For the moment, only the canary version of Next.js supports pages with different extensions.
Until this feature is released into the stable version, do this:
```
npm install --save next@canary
```

or

```
yarn add next@canary
```

## Installation

```
npm install --save next-coffeescript coffeescript
```

or

```
yarn add next-coffeescript coffeescript
```

## Usage

Create a `next.config.js` in your project

```js
// next.config.js
const withCoffeescript = require('next-coffeescript')
module.exports = withCoffeescript()
```

Optionally you can add your custom Next.js configuration as parameter

```js
// next.config.js
const withCoffeescript = require('next-coffeescript')
module.exports = withCoffeescript({
  webpack(config, options) {
    return config
  },
  coffeescriptLoaderOptions: {
    literate: true
  }
})
```
