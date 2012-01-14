# JSONFormatter.js

JSONFormatter takes JSON and renders it into an HTML list.

## Prerequisites

* jQuery
* Valid string of JSON

## Basic usage

The basic usage for JSONFormatter passing in the json:

    JSONFormatter.format(json, {});

### Options

An options object can can be passed as a second parameter to the format function call (defaults shown):

        JSONFormatter.format(json, {
          collapse: false, // Setting to 'true' this will format the JSON into a collapsable/expandable tree
          append_to: 'body', // A string of the id, class or element name to append the formatted json
          list_id: 'json' // The name of the id at the root ul of the formatted JSON
        })

### Styling

A basic stylesheet is available to layout the list slightly nicer than the default styles.

        <link href='stylesheets/jsonFormatter.css' media='all' rel='stylesheet' type='text/css' />