# Check Browsers
It is detect your browser and version(Ineternet Explorer).  
It detects only desktop browser not mobile browser.  
It helps your page styling for each browser.  
It append class with html root element.  
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
You must install node.js and open terminal or CMD.  
and change directory your project directory.  
and type below.
```
$ npm i -S detect-browser
```

## Usage
### In HTML
```html
<head>
  <script src="/node_modules/detect-browser/dist/detect-browser.min.js"></script>
</head>
```
You should import it in head element.  
Because importing in head is processed before page rendering.  
So page styling is more fast.

### In module, Webpack, etc.
#### require statement
```javascript
require('detect-browser');
```

#### import syntax
```javascript
import 'detect-browser';
```

### In CSS
```css
@charset "utf-8";
/* default style */
#test {
  font-size: 3em
}

/* each browser style */
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
  color: brown;
}
```

## Browser List
* IE6~11: ie6~11
* MS Edge: edge
* Google Chrome: chrome
* Mozilla Firefox: firefox
* Apple Safari: safari
* Opera: Opera