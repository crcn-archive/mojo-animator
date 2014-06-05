## Mojo Animator [![Build Status](https://travis-ci.org/classdojo/mojo-animator.svg)](https://travis-ci.org/classdojo/mojo-animator)

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
