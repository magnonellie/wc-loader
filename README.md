<div align="center">
  <img width="200" height="200"
    src="http://webcomponents.org/img/logo.svg">
   <img width="200" height="140" vspace="30"
    src="https://www.polymer-project.org/images/logos/p-logo.png">
  <a href="https://github.com/webpack/webpack">
    <img width="200" height="200" vspace="" hspace="25"
      src="https://worldvectorlogo.com/logos/webpack.svg">
  </a>
  <h1>WC Loader</h1>
  <p>Webcomponents webpack loader **With Hot Code Reload Support For All Imports**.<p>
</div>

[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/aruntk/meteorwebcomponents?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[![Donate](https://dantheman827.github.io/images/donate-button.svg)](https://www.paypal.me/arunkumartk)

DEMO - https://github.com/aruntk/polymer-webpack-demo

## About

wc-loader helps you use webcomponents (polymer, x-tags etc also) with webpack.

### Under the hood

wc-loader uses [parse5](https://github.com/inikulin/parse5) which parses HTML the way the latest version of your browser does. 
Does not use any regex to parse html. :)

#####Main functions

1. Handles html link imports. **With Hot Code Reload Support**
2. Handles external script files (script src). **With Hot Code Reload Support**
3. Handles external css files (link rel stylesheet)
4. Handles template tags.
5. Removes comments and unecessary whitespaces.
5. Handles loading order of html and js inside the polymer files
4. Adds components to document during runtime.

## Installation

```sh
npm i -D wc-loader
```

## Usage

```js
module: {
  loaders: [{
    test: /\.html$/,
    loader: 'wc'
  }]
}
```
