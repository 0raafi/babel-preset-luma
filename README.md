# babel-preset-clodeo-app

This package includes the Babel preset used by [Create Clodeo App](https://www.npmjs.com/package/@clodeo/create-clodeo-app).
<br/>

## Usage in Create Clodeo App Projects

The easiest way to use this configuration is with [Create Clodeo App](https://www.npmjs.com/package/@clodeo/create-clodeo-app), which includes it by default. **You don’t need to install it separately in Create Clodeo App projects.**

## Usage Outside of Create Clodeo App

If you want to use this Babel preset in a project not built with Create React App, you can install it with the following steps.

First, [install Babel](https://babeljs.io/docs/setup/).

Then install babel-preset-clodeo-app.

```sh
npm install babel-preset-clodeo-app --save-dev
```

Then create a file named `.babelrc` with following contents in the root folder of your project:

```json
{
  "presets": ["clodeo-app"]
}
```

This preset uses the `useBuiltIns` option with [transform-object-rest-spread](https://babeljs.io/docs/plugins/transform-object-rest-spread/) and [transform-react-jsx](https://babeljs.io/docs/plugins/transform-react-jsx/), which assumes that `Object.assign` is available or polyfilled.
