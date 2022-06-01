**An autocompletion library to autocomplete mentions, smileys etc. just like on Github!**  
![atjs](https://github.com/Spuds/At.js/workflows/atjs/badge.svg)

#### Help / Build

At.js now **depends on** [Caret.js](https://github.com/ichord/Caret.js).  
Please read [**CONTRIBUTING.md**](CONTRIBUTING.md) for details on how to make code edits and setup your own enviroment.

### Documentation
https://github.com/ichord/At.js/wiki

### Compatibility

* `textarea` - Chrome, Safari, Firefox, IE7+ (maybe IE6)
* `contentEditable` - Chrome, Safari, Firefox, IE9+

### Features Preview

* Support IE 7+ for **textarea**.
* Supports HTML5  [**contentEditable**](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_Editable) elements (NOT including IE 8)
* Can listen to any character and not just '@'. Can set up multiple listeners for different characters with different behavior and data
* Listener events can be bound to multiple inputors.
* Format returned data using templates
* Keyboard controls in addition to mouse
    - `Tab` or `Enter` keys select the value
    - `Up` and `Down` navigate between values (and `Ctrl-P` and `Ctrl-N` also)
    - `Right` and `left` will re-search the keyword.
* Custom data handlers and template renderers using a group of configurable callbacks
* Supports AMD

### Requirements

* jQuery >= 3.0.0.
* [Caret.js](https://github.com/ichord/Caret.js)
    (You can use `Component` or `Bower` to install it.)

### Integrating with your Application

Simply include the following files in your HTML and you are good to go.

```html
<link href="css/jquery.atwho.css" rel="stylesheet">
<script src="http://code.jquery.com/jquery.js"></script>
<script src="js/jquery.caret.js"></script>
<script src="js/jquery.atwho.js"></script>
```

```javascript
$('#inputor').atwho({
    at: "@",
    data:['Peter', 'Tom', 'Anne']
})
```
