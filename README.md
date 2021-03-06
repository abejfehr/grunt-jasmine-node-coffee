# grunt-jasmine-node-coffee

A grunt.js task to run your jasmine feature suite using jasmine-node with coffeescript support.

## Getting Started
Install this grunt plugin next to your project's grunt.js gruntfile with: `npm install grunt-jasmine-node-coffee`

Then add this line to your project's `Gruntfile.js` grunt file:

```javascript
grunt.initConfig({
  jasmine_node: {
    forceExit: true,
    // Default is already spec so not necessary
    specNameMatcher: 'spec',
    projectRoot: 'scripts/folder',
    // This tells jasmine-node to add .coffee files
    extensions: 'coffee'
  }
});

grunt.loadNpmTasks('grunt-jasmine-node-coffee');

grunt.registerTask('default', 'jasmine_node');
```

Or in CoffeeScript in your `Gruntfile.coffee` grunt file:
```coffeescript
grunt.initConfig {
  jasmine_node:
    forceExit: true
    # Default is already spec so not necessary
    specNameMatcher: 'spec'
    projectRoot: 'scripts/folder'
    # This tells jasmine-node to add .coffee files
    extensions: 'coffee'
}

grunt.loadNpmTasks 'grunt-jasmine-node-coffee'

grunt.registerTask 'default', 'jasmine_node'
```

## Bugs

Help us squash them by submitting an issue to the [author](https://github.com/beautifulcoder) that describes how you encountered it; please be as specific as possible including operating system, node, grunt, and grunt-jasmine-node-coffee versions. This version of the software strictly deals with coffeescript support so please stay on topic.

## Release History

see [GitHub Repository](https://github.com/beautifulcoder/grunt-jasmine-node-coffee).

## License
Copyright (c) 2014 "beautifulcoder" Camilo Reyes & contributors. Based on [grunt-jasmine-node](https://github.com/jasmine-contrib/grunt-jasmine-node) Copyright (c) 2012 "s9tpepper" Omar Gonzalez & contributors.
Licensed under the MIT license.
