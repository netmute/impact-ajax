# AJAX plugin for ImpactJS

Ajax in plain Javascript is painful? Including a big library just for `get` and `post` methods seems like overkill? Then this is for you.

## Usage

First initialize the class.

    ajax = new ig.Ajax();

### Requests

Asynchronously GET a resource:

    ajax.get( "http://example.com/", function(result) {
      console.log(result);
    });

Asynchronously GET a JSON resource:

    ajax.getJSON( "http://example.com/", function(result) {
      console.log(result);
    });

Synchronously GET a resource:

    var result = ajax.get_sync( "http://example.com/" );

Synchronously GET a JSON resource:

    var result = ajax.getJSON_sync( "http://example.com/" );

Asynchronously POST a resource:

    ajax.post( "http://example.com/", {test: "Bla", foo: "Bar"}, function(result) {
      console.log(result);
    });