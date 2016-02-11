### annalka

annalka is a jQuery plugin that provides a simple text transformation effect that works by randomizing characters.  
  
![annalka.js example](examples/annalka-gif.gif)
  
**Feedback welcome.**  

## Installation
Include script *after* the jQuery library:
```html
<script src="/path/to/jquery.annalka.js"></script>
```

## Usage

Basic usage:
```javascript
$('#element').annalka("Target String");
```

You can also customize the behaviour by passing in an optional options object:
```javascript
$('#element').annalka("Target String", {
    //Time between each randomized letter. Default: 15
    tick: 25,
    //Number of randomizations before moving towards target length. Default: 4
    step: 5,
    //String with characters to randomize from. Default: ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789
    chars: 'ABC'
});
```

The options object can also contain a callback method which is invoked when animation finishes:
```javascript
$('#element').annalka("Target String", {
    callback: function() {
        //Animation finished.
    }
});
```

## Todo

- Improve animation appearance
- Write tests
- Test performance

## License

jquery.annalka.js is available under MIT license.
See LICENSE file for more information.