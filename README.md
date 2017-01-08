[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://beta.webcomponents.org/element/owner/my-element)
# \<feathersjs-client\>

A web component wrapper around the feathersjs-client library that also takes care of establishing a server connection. If you are not familiar with feathers.js please check out their awesome website [http://feathersjs.com/].

A typical use case looks like this:

    <feathersjs-client app="{{app}}" server="{{url}}" connected="{{isConnected}}"></feathersjs-client>

When the server url is set, feathersjs-client tries to establish a connection to the server. Once this is successful
the `connected` attribute is set to true, the `feathersjs-connected` event is thrown and the `app` property is set.
The `app` property then can be used to access a feather.js service:

    var service = app.service('todos');

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
