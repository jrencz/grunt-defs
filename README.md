# grunt-defs

> Static scope analysis and transpilation of ES6 block scoped const and let variables, to ES3.

## Getting Started
This plugin requires Grunt.

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-defs --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-defs');
```

## The "defs" task

### Overview
In your project's Gruntfile, add a section named `defs` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  defs: {
    options: {
      // Task-specific options go here.
    },
    your_target: {
      // Target-specific file lists and/or options go here.
    },
  },
})
```

#### Options

The `defs` task accepts a couple of options:

```js
{
    // If files are provided without a destination, each file is processed
    // separately and each of them is saved under original name with appended suffix provided here.
    outputFileSuffix: string,

    // If files are provided without a destination and this option is set, each file is processed
    // separately and each of them is saved under original name processed by this function.
    transformDest: function (sourcePath) {},

    // Here one can set `defs` options; see: https://npmjs.org/package/defs
    defsOptions: {
        disallowDuplicated: true,
        disallowUnknownReferences: false,
        disallowVars: true,
    },

    // Instead of providing `defsOptions` manually, one can provide a URL to the `defs-config.json`
    // configuration file; see: https://npmjs.org/package/defs
    defsConfigUrl: string,
}
```

### Usage Examples

TODO

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_(Nothing yet)_

## License
Copyright (c) 2013 Laboratorium EE. Licensed under the MIT license.
