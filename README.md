# JSONFormatter.js (beta)

JSONFormatter takes JSON and renders it into an HTML list.

[View a demo](http://emmasax.github.com/json-formatter/)

## Basic usage

This library requires jQuery

The basic usage for JSONFormatter is passing in the JSON and an empty options object:

    JSONFormatter.format(json, {});

## Options

An options object can can be passed as a second parameter to the format function call (defaults shown):

    JSONFormatter.format(json, {
      collapse: false, // Setting to 'true' this will format the JSON into a collapsable/expandable tree
      appendTo: 'body', // A string of the id, class or element name to append the formatted json
      list_id: 'json' // The name of the id at the root ul of the formatted JSON
    })

## Styling

A basic stylesheet is available to layout the list slightly nicer than the default styles.

    <link href='jsonFormatter.css' media='all' rel='stylesheet' type='text/css' />
    
## To do:

  * Fix the object of objects - don't output 0:, 1:, 2:, etc.
  * Fix array of strings in first child node
  * General refactor - lots of code duplication

## Development

Source hosted at [GitHub](http://github.com/emmasax/json-formatter).
Report Issues/Feature requests on [GitHub Issues](http://github.com/emmasax/json-formatter/issues).

### Note on Patches/Pull Requests

 * Fork the project.
 * Make your feature addition or bug fix.
 * Commit, do not mess with rakefile, version, or history.
   (if you want to have your own version, that is fine but bump version in a commit by itself I can ignore when I pull)
 * Send me a pull request. Bonus points for topic branches.
