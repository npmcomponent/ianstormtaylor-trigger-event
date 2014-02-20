*This repository is a mirror of the [component](http://component.io) module [ianstormtaylor/trigger-event](http://github.com/ianstormtaylor/trigger-event). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/ianstormtaylor-trigger-event`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# trigger-event

  Programmatically trigger a DOM event. Useful for testing mostly.

## Installation

    $ component install ianstormtaylor/trigger-event

## Example
  
```js
var trigger = require('trigger-event');
trigger(button, 'click', { meta: true });
trigger(document, 'keydown', { key: 'enter' });
```

Shorthand for keys:

```js
trigger('keydown', { key: 'enter' })
```

## API

### trigger(type, [element], [options])

  Types:

    'click'
    'dblclick'
    'keydown'
    'keyup'

  Element will default to `document` if none is provided.

  Default `options`:

    alt        : false,
    bubbles    : true,
    button     : 0,
    cancelable : true,
    clientX    : 0,
    clientY    : 0,
    ctrl       : false,
    detail     : 1,
    key        : 0, // can be a string like 'enter' for convenience
    meta       : false,
    screenX    : 0,
    screenY    : 0,
    shift      : false,
    view       : window

## License

  MIT
