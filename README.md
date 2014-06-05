## Mojo Animator [![Build Status](https://travis-ci.org/classdojo/mojo-animator.svg)](https://travis-ci.org/classdojo/mojo-animator)

Mojo Animator is a component used to update parts of the application where the DOM might be manipulated. It's used in [paperclip](github.com/classdojo/paperclip.js), and [mojo-views](https://github.com/classdojo/mojo-views).

```javascript
var Application = require("mojo-application");

var MyApplication = Application.extend({
  registerPlugins: function () {
    this.use(require("mojo-animator"));
  }
});

var app = new MojoApplication();

// calls requestAnimationFrame
app.animate({
  update: function () {
    // do something
  }
})
```
