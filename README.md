# grunt-regex-replace

Grunt plugin to search and replace text content of files based on regular expression patterns

## Getting Started
Install this grunt plugin next to your project's [grunt.js gruntfile][getting_started] with: `npm install grunt-regex-replace`

Then add this line to your project's `grunt.js` gruntfile:

```javascript
grunt.loadNpmTasks('grunt-regex-replace');
```

[grunt]: http://gruntjs.com/
[getting_started]: https://github.com/gruntjs/grunt/blob/master/docs/getting_started.md

## How to use
Sample Code
      regex-replace: {
        src: ['/foo/'],
        actions: [
          {
            search: '(^|\\s)console.log',
            replace: '//console.log',
            flags: 'g'
          },{
            search: 'var v = \'[^\']*\';',
            replace: 'var v = \'<%= pkg.release.version_code %>\';',
            flags: 'g'
          }
        ]
      }

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [grunt][grunt].

## Release History
_(Nothing yet)_

## License
Copyright (c) 2012 Hubert Boma Manilla  
Licensed under the MIT license.
=======
grunt-regex-replace
===================

Grunt plugin to search and replace text content of files based on regular expression patterns
