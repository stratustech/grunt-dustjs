grunt-dustjs
----------

Grunt task to compile Dust.js templates.

Getting Started
===============

Install this grunt plugin next to your project's [grunt.js gruntfile][getting_started] with: `npm install grunt-dustjs`.

Then add this line to your project's `grunt.js` gruntfile:

```javascript
grunt.loadNpmTasks('grunt-dustjs');
```

[npm_registry_page]: http://search.npmjs.org/#/grunt-dustjs
[grunt]: https://github.com/cowboy/grunt
[getting_started]: https://github.com/cowboy/grunt/blob/master/docs/getting_started.md

Documentation
=============

Inside your `grunt.js` file, add a section named `dustjs`. This section specifies the Dust.js template files to compile.

##### files ```object```

This defines what files this task will process and should contain key:value pairs.

The key (destination) should be an unique filepath (supports [grunt.template](https://github.com/cowboy/grunt/blob/master/docs/api_template.md)) and the value (source) should be a filepath or an array of filepaths (supports [minimatch](https://github.com/isaacs/minimatch)).

### Example

```javascript
// project configuration
grunt.initConfig({
  dustjs: {
    compile: {
      files: {
        "js/templates.js": ["src/templates/**/*.html"]
      }
    }
  },
});
```

Contributing
============

In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [grunt][grunt].

Release History
===============
*   __25/09/2012 - 0.1.2__: Initial release.

License
=======

Copyright (c) 2012 Stanislav Lesnikov
Licensed under the MIT license.
