[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://beta.webcomponents.org/element/owner/my-element)
# \<feathersjs-client\>

A web component wrapper around the feathersjs-client library that also takes care of establishing a server connection. If you are not familiar with feathers.js please check out their awesome website http://feathersjs.com/.

A typical use case looks like this:
```html
<feathersjs-client app="{{app}}" server="{{url}}" connected="{{isConnected}}"></feathersjs-client>
```

When the server url is set, feathersjs-client tries to establish a connection to the server. Once this is successful
the `connected` attribute is set to true, the `feathersjs-connected` event is thrown and the `app` property is set.
The `app` property then can be used to access a feather.js service:

```javascript
var service = app.service('todos');
```
