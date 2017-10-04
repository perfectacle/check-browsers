# Check Browsers
[![NPM](https://nodei.co/npm/check-browsers.png)](https://www.npmjs.com/package/check-browsers)
[![jsdelivr](https://img.shields.io/badge/cdn-v1.0.4-ff69b4.svg)](https://www.jsdelivr.com/projects/check-browsers)
![npm](https://img.shields.io/npm/dt/check-browsers.svg?style=plastic)
![npm](https://img.shields.io/npm/v/check-browsers.svg?style=plastic)
  
It is detect your browser and version(Ineternet Explorer).  
It detects only desktop browser not mobile browser.  
It helps your page styling for each browser.  
It appends class with html root element.  
```html
<html class="browser type">
```
If you known some idea for mobile browser, you could send pull request.

## Index
1. [Installation](#installation)
2. [Usage](#usage)
    1. [In HTML](#in-html)
    2. [In module, Webpack, etc.](#in-module-webpack-etc)
    3. [In CSS](#in-css)
3. [Browser List](#browser-list)

## Installation
Using CDN: 
```
<script src="//cdn.jsdelivr.net/npm/check-browsers@1.0.8/dist/check-browsers.min.js"></script>
```
Using npm:
```
$ npm i -S check-browsers
```
Using yarn:
```
$ yarn add check-browsers
```

## Usage
### In HTML
```html
<head>
  ...
  <script src="/node_modules/check-browsers/dist/check-browsers.min.js"></script>
  ...
  <link rel="stylesheet" href="..." />
  ...
</head>
```
You should import it in head element and before stylesheet.  
Because importing in head is processed before page rendering.  
and importing before stylesheet is processed before styling.  
So page styling is more fast.

### In module, Webpack, etc.
#### require statement
```javascript
require('check-browsers');
```

#### import syntax
```javascript
import 'check-browsers';
```

### In CSS
```css
@charset "utf-8";
/* default style */
#test {
  font-size: 3em
}

/* each browser style */
.ie6 #test {
  color: salmon
}

.ie7 #test {
  color: red
}

.ie8 #test {
  color: blue
}

.ie9 #test {
  color: purple
}

.ie10 #test {
  color: orange
}

.ie11 #test {
  color: green
}

.edge #test {
  color: gray
}

.chrome #test {
  color: navy
}

.firefox #test {
  color: lime
}

.safari #test {
  color: fuchsia
}

.opera #test {
  color: brown
}
```

## Browser List
* IE6~11: ie6~11
* MS Edge: edge
* Google Chrome: chrome
* Mozilla Firefox: firefox
* Apple Safari: safari
* Opera: opera
