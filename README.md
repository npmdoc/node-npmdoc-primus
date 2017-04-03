# api documentation for  [primus (v7.0.0)](http://primus.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-primus.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-primus) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-primus.svg)](https://travis-ci.org/npmdoc/node-npmdoc-primus)
#### Primus is a simple abstraction around real-time frameworks. It allows you to easily switch between different frameworks without any code changes.

[![NPM](https://nodei.co/npm/primus.png?downloads=true)](https://www.npmjs.com/package/primus)

[![apidoc](https://npmdoc.github.io/node-npmdoc-primus/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-primus_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-primus/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-primus/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-primus/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Arnout Kazemier"
    },
    "bugs": {
        "url": "https://github.com/primus/primus/issues"
    },
    "dependencies": {
        "access-control": "~1.0.0",
        "asyncemit": "~3.0.1",
        "create-server": "~1.0.1",
        "diagnostics": "~1.1.0",
        "eventemitter3": "~2.0.2",
        "forwarded-for": "~1.0.1",
        "fusing": "~1.0.0",
        "setheader": "~0.0.4",
        "ultron": "~1.1.0",
        "yeast": "~0.1.2"
    },
    "description": "Primus is a simple abstraction around real-time frameworks. It allows you to easily switch between different frameworks without any code changes.",
    "devDependencies": {
        "binary-pack": "~1.0.2",
        "browserchannel": "~2.0.0",
        "browserify": "~14.1.0",
        "chai": "~3.5.0",
        "condenseify": "~1.1.1",
        "demolish": "~1.0.2",
        "derequire": "~2.0.3",
        "deumdify": "~1.2.3",
        "ejson": "~2.1.2",
        "emits": "~3.0.0",
        "engine.io": "~2.1.0",
        "engine.io-client": "~2.1.0",
        "faye-websocket": "~0.11.0",
        "inherits": "~2.0.3",
        "mocha": "~3.2.0",
        "pre-commit": "~1.2.0",
        "primus-msgpack": "~1.0.2",
        "pumpify": "~1.3.5",
        "querystringify": "~1.0.0",
        "recovery": "~0.2.6",
        "request": "~2.81.0",
        "rocambole": "~0.7.0",
        "rocambole-node-remove": "~1.0.0",
        "sockjs": "~0.3.18",
        "sockjs-client": "~1.1.1",
        "through2": "~2.0.1",
        "tick-tock": "~1.0.0",
        "url-parse": "~1.1.7",
        "uws": "~0.14.0",
        "ws": "~2.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "d37adff33954277139e76df222828160e0b563e3",
        "tarball": "https://registry.npmjs.org/primus/-/primus-7.0.0.tgz"
    },
    "gitHead": "30d4a46cb2c7e1ae53524519cdf9d1ca5c133d8f",
    "homepage": "http://primus.io",
    "keywords": [
        "abstraction",
        "browserchannel",
        "engine.io",
        "framework",
        "comet",
        "streaming",
        "pubsub",
        "pub",
        "sub",
        "ajax",
        "xhr",
        "polling",
        "http",
        "faye",
        "io",
        "primus",
        "prumus",
        "real-time",
        "realtime",
        "socket",
        "socket.io",
        "sockets",
        "sockjs",
        "spark",
        "transformer",
        "transformers",
        "websocket",
        "websockets",
        "ws",
        "uws"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        },
        {
            "name": "swaagie",
            "email": "info@martijnswaagman.nl"
        },
        {
            "name": "lpinca",
            "email": "luigipinca@gmail.com"
        },
        {
            "name": "davedoesdev",
            "email": "dahalls@gmail.com"
        },
        {
            "name": "v1",
            "email": "info@3rd-Eden.com"
        },
        {
            "name": "3rdeden",
            "email": "npm@3rd-Eden.com"
        }
    ],
    "name": "primus",
    "optionalDependencies": {},
    "pre-commit": "test, integration",
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/primus/primus.git"
    },
    "scripts": {
        "build": "mkdir -p dist && browserify primus.js -s Primus -p deumdify | derequire > dist/primus.js",
        "integration": "npm run build && mocha test/*.integration.js",
        "prepublish": "npm run build",
        "test": "npm run build && mocha test/*.test.js",
        "update": "find transformers -name update.sh -exec bash {} \\;"
    },
    "version": "7.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module primus](#apidoc.module.primus)
1.  [function <span class="apidocSignatureSpan">primus.</span>Spark (primus, headers, address, query, id, request)](#apidoc.element.primus.Spark)
1.  [function <span class="apidocSignatureSpan">primus.</span>Transformer (primus)](#apidoc.element.primus.Transformer)
1.  [function <span class="apidocSignatureSpan">primus.</span>createServer (fn, options)](#apidoc.element.primus.createServer)
1.  [function <span class="apidocSignatureSpan">primus.</span>createSocket (options)](#apidoc.element.primus.createSocket)
1.  [function <span class="apidocSignatureSpan">primus.</span>extend (protoProps, staticProps)](#apidoc.element.primus.extend)
1.  [function <span class="apidocSignatureSpan">primus.</span>get (method, getter)](#apidoc.element.primus.get)
1.  [function <span class="apidocSignatureSpan">primus.</span>predefine (obj, pattern)](#apidoc.element.primus.predefine)
1.  [function <span class="apidocSignatureSpan">primus.</span>readable (method, description, clean)](#apidoc.element.primus.readable)
1.  [function <span class="apidocSignatureSpan">primus.</span>set (method, getter, setter)](#apidoc.element.primus.set)
1.  [function <span class="apidocSignatureSpan">primus.</span>writable (method, description, clean)](#apidoc.element.primus.writable)
1.  object <span class="apidocSignatureSpan">primus.</span>errors
1.  object <span class="apidocSignatureSpan">primus.</span>json
1.  object <span class="apidocSignatureSpan">primus.</span>parsers
1.  object <span class="apidocSignatureSpan">primus.</span>transformers

#### [module primus.Spark](#apidoc.module.primus.Spark)
1.  [function <span class="apidocSignatureSpan">primus.</span>Spark (primus, headers, address, query, id, request)](#apidoc.element.primus.Spark.Spark)
1.  [function <span class="apidocSignatureSpan">primus.Spark.</span>extend (protoProps, staticProps)](#apidoc.element.primus.Spark.extend)
1.  [function <span class="apidocSignatureSpan">primus.Spark.</span>get (method, getter)](#apidoc.element.primus.Spark.get)
1.  [function <span class="apidocSignatureSpan">primus.Spark.</span>predefine (obj, pattern)](#apidoc.element.primus.Spark.predefine)
1.  [function <span class="apidocSignatureSpan">primus.Spark.</span>readable (method, description, clean)](#apidoc.element.primus.Spark.readable)
1.  [function <span class="apidocSignatureSpan">primus.Spark.</span>set (method, getter, setter)](#apidoc.element.primus.Spark.set)
1.  [function <span class="apidocSignatureSpan">primus.Spark.</span>writable (method, description, clean)](#apidoc.element.primus.Spark.writable)
1.  number <span class="apidocSignatureSpan">primus.Spark.</span>CLOSED
1.  number <span class="apidocSignatureSpan">primus.Spark.</span>OPEN
1.  number <span class="apidocSignatureSpan">primus.Spark.</span>OPENING

#### [module primus.Transformer](#apidoc.module.primus.Transformer)
1.  [function <span class="apidocSignatureSpan">primus.</span>Transformer (primus)](#apidoc.element.primus.Transformer.Transformer)
1.  [function <span class="apidocSignatureSpan">primus.Transformer.</span>extend (protoProps, staticProps)](#apidoc.element.primus.Transformer.extend)
1.  [function <span class="apidocSignatureSpan">primus.Transformer.</span>get (method, getter)](#apidoc.element.primus.Transformer.get)
1.  [function <span class="apidocSignatureSpan">primus.Transformer.</span>predefine (obj, pattern)](#apidoc.element.primus.Transformer.predefine)
1.  [function <span class="apidocSignatureSpan">primus.Transformer.</span>readable (method, description, clean)](#apidoc.element.primus.Transformer.readable)
1.  [function <span class="apidocSignatureSpan">primus.Transformer.</span>set (method, getter, setter)](#apidoc.element.primus.Transformer.set)
1.  [function <span class="apidocSignatureSpan">primus.Transformer.</span>writable (method, description, clean)](#apidoc.element.primus.Transformer.writable)

#### [module primus.errors](#apidoc.module.primus.errors)
1.  [function <span class="apidocSignatureSpan">primus.errors.</span>ParserError (message, spark)](#apidoc.element.primus.errors.ParserError)
1.  [function <span class="apidocSignatureSpan">primus.errors.</span>PrimusError (message, logger)](#apidoc.element.primus.errors.PrimusError)

#### [module primus.json](#apidoc.module.primus.json)
1.  [function <span class="apidocSignatureSpan">primus.json.</span>decoder (data, fn)](#apidoc.element.primus.json.decoder)
1.  [function <span class="apidocSignatureSpan">primus.json.</span>encoder (data, fn)](#apidoc.element.primus.json.encoder)

#### [module primus.predefine](#apidoc.module.primus.predefine)
1.  [function <span class="apidocSignatureSpan">primus.</span>predefine (obj, pattern)](#apidoc.element.primus.predefine.predefine)
1.  [function <span class="apidocSignatureSpan">primus.predefine.</span>create (property, description, pattern)](#apidoc.element.primus.predefine.create)
1.  [function <span class="apidocSignatureSpan">primus.predefine.</span>descriptor (obj)](#apidoc.element.primus.predefine.descriptor)
1.  [function <span class="apidocSignatureSpan">primus.predefine.</span>each (collection, iterator, context)](#apidoc.element.primus.predefine.each)
1.  [function <span class="apidocSignatureSpan">primus.predefine.</span>extend (protoProps, staticProps)](#apidoc.element.primus.predefine.extend)
1.  [function <span class="apidocSignatureSpan">primus.predefine.</span>lazy (obj, prop, fn)](#apidoc.element.primus.predefine.lazy)
1.  [function <span class="apidocSignatureSpan">primus.predefine.</span>merge (target, additional)](#apidoc.element.primus.predefine.merge)
1.  [function <span class="apidocSignatureSpan">primus.predefine.</span>mixin (target)](#apidoc.element.primus.predefine.mixin)
1.  [function <span class="apidocSignatureSpan">primus.predefine.</span>remove (obj, keep)](#apidoc.element.primus.predefine.remove)
1.  object <span class="apidocSignatureSpan">primus.predefine.</span>READABLE
1.  object <span class="apidocSignatureSpan">primus.predefine.</span>WRITABLE



# <a name="apidoc.module.primus"></a>[module primus](#apidoc.module.primus)

#### <a name="apidoc.element.primus.Spark"></a>[function <span class="apidocSignatureSpan">primus.</span>Spark (primus, headers, address, query, id, request)](#apidoc.element.primus.Spark)
- description and source-code
```javascript
function Spark(primus, headers, address, query, id, request) {
  this.fuse();

  var writable = this.writable
    , spark = this;

  query = query || {};
  id = id || yeast();
  headers = headers || {};
  address = address || {};
  request = request || headers['primus::req::backup'];

  writable('id', id);                   // Unique id for socket.
  writable('primus', primus);           // References to Primus.
  writable('remote', address);          // The remote address location.
  writable('headers', headers);         // The request headers.
  writable('request', request);         // Reference to an HTTP request.
  writable('writable', true);           // Silly stream compatibility.
  writable('readable', true);           // Silly stream compatibility.
  writable('queue', []);                // Data queue for data events.
  writable('query', query);             // The query string.
  writable('ultron', new Ultron(this)); // Our event listening cleanup.
  writable('alive', true);              // Flag used to detect zombie sparks.

  //
  // Parse our query string.
  //
  if ('string' === typeof this.query) {
    this.query = parse(this.query);
  }

  this.__initialise.forEach(function execute(initialise) {
    initialise.call(spark);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Transformer"></a>[function <span class="apidocSignatureSpan">primus.</span>Transformer (primus)](#apidoc.element.primus.Transformer)
- description and source-code
```javascript
function Transformer(primus) {
  this.fuse();

  this.ultron = new Ultron(primus.server);  // Handles listeners with ease.
  this.Spark = primus.Spark;                // Reference to the Spark constructor.
  this.primus = primus;                     // Reference to the Primus instance.
  this.service = null;                      // Stores the real-time service.

  this.initialise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.createServer"></a>[function <span class="apidocSignatureSpan">primus.</span>createServer (fn, options)](#apidoc.element.primus.createServer)
- description and source-code
```javascript
function createServer(fn, options) {
  if ('object' === typeof fn) {
    options = fn;
    fn = null;
  }

  options = options || {};

  var server = require('create-server')(Primus.prototype.merge.call(Primus, {
    http: function warn() {
      if (!options.iknowhttpsisbetter) [
        '',
        'We\'ve detected that you\'re using a HTTP instead of a HTTPS server.',
        'Please be aware that real-time connections have less chance of being blocked',
        'by firewalls and anti-virus scanners if they are encrypted (using SSL). If',
        'you run your server behind a reverse and HTTPS terminating proxy ignore',
        'this message, if not, you\'ve been warned.',
        ''
      ].forEach(function each(line) {
        console.log('primus: '+ line);
      });
    }
  }, options));

  //
  // Now that we've got a server, we can setup the Primus and start listening.
  //
  var application = new Primus(server, options);

  if (fn) application.on('connection', fn);
  return application;
}
```
- example usage
```shell
...

'''js
'use strict';

var Primus = require('primus')
  , http = require('http');

var server = http.createServer(/* request handler */)
  , primus = new Primus(server, {/* options */});
'''
The following options can be provided:

Name                | Description                               | Default
--------------------|-------------------------------------------|---------------
authorization       | Authorization handler                     | 'null'
...
```

#### <a name="apidoc.element.primus.createSocket"></a>[function <span class="apidocSignatureSpan">primus.</span>createSocket (options)](#apidoc.element.primus.createSocket)
- description and source-code
```javascript
function createSocket(options) {
  options = options || {};

  var primus = new Primus(new EventEmitter(), options);
  return primus.Socket;
}
```
- example usage
```shell
...
2. You might need to connect from a different node process where you don't have
   access to your 'primus' instance and the compatible 'Socket' instance. For
   these cases there a special 'createSocket' method where you can specify the
   'transformer', 'parser', 'plugin' that you are using on your server to create
   another compatible socket.

   '''js
   var Socket = Primus.createSocket({ transformer: transformer, parser: parser })
     , client = new Socket('http://localhost:8080');
   '''

When you are using plugins with Primus make sure you add them **before** you
reference the 'primus.Socket' or it will compile a client without your plugins.
If you're using the 'Primus.createSocket' api you can directly supply the
plugins as part of the options as it supports 'plugin' object:
...
```

#### <a name="apidoc.element.primus.extend"></a>[function <span class="apidocSignatureSpan">primus.</span>extend (protoProps, staticProps)](#apidoc.element.primus.extend)
- description and source-code
```javascript
function extend(protoProps, staticProps) {
  var parent = this
    , child;

  //
  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  //
  if (protoProps && has.call(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = mode(parent);
  }

  //
  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  //
  function Surrogate() {
    this.constructor = child;
  }

  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  //
  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  //
  if (protoProps) mixin(child.prototype, protoProps);

  //
  // Add static properties to the constructor function, if supplied.
  //
  copypaste(child, parent, staticProps);

  //
  // Set a convenience property in case the parent's prototype is needed later.
  //
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.get"></a>[function <span class="apidocSignatureSpan">primus.</span>get (method, getter)](#apidoc.element.primus.get)
- description and source-code
```javascript
function get(method, getter) {
  Object.defineProperty(Base.prototype, method, {
    configurable: false,
    enumerable: false,
    get: getter
  });

  return get;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.predefine"></a>[function <span class="apidocSignatureSpan">primus.</span>predefine (obj, pattern)](#apidoc.element.primus.predefine)
- description and source-code
```javascript
function predefine(obj, pattern) {
  pattern = pattern || predefine.READABLE;

  return function predefined(method, description, clean) {
    //
    // If we are given a description compatible Object, use that instead of
    // setting it as value. This allows easy creation of getters and setters.
    //
    if (
         !predefine.descriptor(description)
      || is(description, 'object')
         && !clean
         && !predefine.descriptor(predefine.mixin({}, pattern, description))
    ) { description = {
        value: description
      };
    }

    //
    // Prevent thrown errors when we attempt to override a readonly
    // property
    //
    var described = Object.getOwnPropertyDescriptor(obj, method);
    if (described && !described.configurable) {
      return predefined;
    }

    Object.defineProperty(obj, method, !clean
      ? predefine.mixin({}, pattern, description)
      : description
    );

    return predefined;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.readable"></a>[function <span class="apidocSignatureSpan">primus.</span>readable (method, description, clean)](#apidoc.element.primus.readable)
- description and source-code
```javascript
function predefined(method, description, clean) {
  //
  // If we are given a description compatible Object, use that instead of
  // setting it as value. This allows easy creation of getters and setters.
  //
  if (
       !predefine.descriptor(description)
    || is(description, 'object')
       && !clean
       && !predefine.descriptor(predefine.mixin({}, pattern, description))
  ) { description = {
      value: description
    };
  }

  //
  // Prevent thrown errors when we attempt to override a readonly
  // property
  //
  var described = Object.getOwnPropertyDescriptor(obj, method);
  if (described && !described.configurable) {
    return predefined;
  }

  Object.defineProperty(obj, method, !clean
    ? predefine.mixin({}, pattern, description)
    : description
  );

  return predefined;
}
```
- example usage
```shell
...
 * Simple function to output common errors.
 *
 * @param {String} what What is missing.
 * @param {Object} where Either Primus.parsers or Primus.transformers.
 * @returns {Object}
 * @api private
 */
Primus.readable('is', function is(what, where) {
var missing = Primus.parsers !== where
    ? 'transformer'
    : 'parser'
  , dependency = where[what];

return {
  missing: function write() {
...
```

#### <a name="apidoc.element.primus.set"></a>[function <span class="apidocSignatureSpan">primus.</span>set (method, getter, setter)](#apidoc.element.primus.set)
- description and source-code
```javascript
function set(method, getter, setter) {
  Object.defineProperty(Base.prototype, method, {
    configurable: false,
    enumerable: false,
    get: getter,
    set: setter
  });

  return set;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.writable"></a>[function <span class="apidocSignatureSpan">primus.</span>writable (method, description, clean)](#apidoc.element.primus.writable)
- description and source-code
```javascript
function predefined(method, description, clean) {
  //
  // If we are given a description compatible Object, use that instead of
  // setting it as value. This allows easy creation of getters and setters.
  //
  if (
       !predefine.descriptor(description)
    || is(description, 'object')
       && !clean
       && !predefine.descriptor(predefine.mixin({}, pattern, description))
  ) { description = {
      value: description
    };
  }

  //
  // Prevent thrown errors when we attempt to override a readonly
  // property
  //
  var described = Object.getOwnPropertyDescriptor(obj, method);
  if (described && !described.configurable) {
    return predefined;
  }

  Object.defineProperty(obj, method, !clean
    ? predefine.mixin({}, pattern, description)
    : description
  );

  return predefined;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.primus.Spark"></a>[module primus.Spark](#apidoc.module.primus.Spark)

#### <a name="apidoc.element.primus.Spark.Spark"></a>[function <span class="apidocSignatureSpan">primus.</span>Spark (primus, headers, address, query, id, request)](#apidoc.element.primus.Spark.Spark)
- description and source-code
```javascript
function Spark(primus, headers, address, query, id, request) {
  this.fuse();

  var writable = this.writable
    , spark = this;

  query = query || {};
  id = id || yeast();
  headers = headers || {};
  address = address || {};
  request = request || headers['primus::req::backup'];

  writable('id', id);                   // Unique id for socket.
  writable('primus', primus);           // References to Primus.
  writable('remote', address);          // The remote address location.
  writable('headers', headers);         // The request headers.
  writable('request', request);         // Reference to an HTTP request.
  writable('writable', true);           // Silly stream compatibility.
  writable('readable', true);           // Silly stream compatibility.
  writable('queue', []);                // Data queue for data events.
  writable('query', query);             // The query string.
  writable('ultron', new Ultron(this)); // Our event listening cleanup.
  writable('alive', true);              // Flag used to detect zombie sparks.

  //
  // Parse our query string.
  //
  if ('string' === typeof this.query) {
    this.query = parse(this.query);
  }

  this.__initialise.forEach(function execute(initialise) {
    initialise.call(spark);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Spark.extend"></a>[function <span class="apidocSignatureSpan">primus.Spark.</span>extend (protoProps, staticProps)](#apidoc.element.primus.Spark.extend)
- description and source-code
```javascript
function extend(protoProps, staticProps) {
  var parent = this
    , child;

  //
  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  //
  if (protoProps && has.call(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = mode(parent);
  }

  //
  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  //
  function Surrogate() {
    this.constructor = child;
  }

  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  //
  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  //
  if (protoProps) mixin(child.prototype, protoProps);

  //
  // Add static properties to the constructor function, if supplied.
  //
  copypaste(child, parent, staticProps);

  //
  // Set a convenience property in case the parent's prototype is needed later.
  //
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Spark.get"></a>[function <span class="apidocSignatureSpan">primus.Spark.</span>get (method, getter)](#apidoc.element.primus.Spark.get)
- description and source-code
```javascript
function get(method, getter) {
  Object.defineProperty(Base.prototype, method, {
    configurable: false,
    enumerable: false,
    get: getter
  });

  return get;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Spark.predefine"></a>[function <span class="apidocSignatureSpan">primus.Spark.</span>predefine (obj, pattern)](#apidoc.element.primus.Spark.predefine)
- description and source-code
```javascript
function predefine(obj, pattern) {
  pattern = pattern || predefine.READABLE;

  return function predefined(method, description, clean) {
    //
    // If we are given a description compatible Object, use that instead of
    // setting it as value. This allows easy creation of getters and setters.
    //
    if (
         !predefine.descriptor(description)
      || is(description, 'object')
         && !clean
         && !predefine.descriptor(predefine.mixin({}, pattern, description))
    ) { description = {
        value: description
      };
    }

    //
    // Prevent thrown errors when we attempt to override a readonly
    // property
    //
    var described = Object.getOwnPropertyDescriptor(obj, method);
    if (described && !described.configurable) {
      return predefined;
    }

    Object.defineProperty(obj, method, !clean
      ? predefine.mixin({}, pattern, description)
      : description
    );

    return predefined;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Spark.readable"></a>[function <span class="apidocSignatureSpan">primus.Spark.</span>readable (method, description, clean)](#apidoc.element.primus.Spark.readable)
- description and source-code
```javascript
function predefined(method, description, clean) {
  //
  // If we are given a description compatible Object, use that instead of
  // setting it as value. This allows easy creation of getters and setters.
  //
  if (
       !predefine.descriptor(description)
    || is(description, 'object')
       && !clean
       && !predefine.descriptor(predefine.mixin({}, pattern, description))
  ) { description = {
      value: description
    };
  }

  //
  // Prevent thrown errors when we attempt to override a readonly
  // property
  //
  var described = Object.getOwnPropertyDescriptor(obj, method);
  if (described && !described.configurable) {
    return predefined;
  }

  Object.defineProperty(obj, method, !clean
    ? predefine.mixin({}, pattern, description)
    : description
  );

  return predefined;
}
```
- example usage
```shell
...
 * Simple function to output common errors.
 *
 * @param {String} what What is missing.
 * @param {Object} where Either Primus.parsers or Primus.transformers.
 * @returns {Object}
 * @api private
 */
Primus.readable('is', function is(what, where) {
var missing = Primus.parsers !== where
    ? 'transformer'
    : 'parser'
  , dependency = where[what];

return {
  missing: function write() {
...
```

#### <a name="apidoc.element.primus.Spark.set"></a>[function <span class="apidocSignatureSpan">primus.Spark.</span>set (method, getter, setter)](#apidoc.element.primus.Spark.set)
- description and source-code
```javascript
function set(method, getter, setter) {
  Object.defineProperty(Base.prototype, method, {
    configurable: false,
    enumerable: false,
    get: getter,
    set: setter
  });

  return set;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Spark.writable"></a>[function <span class="apidocSignatureSpan">primus.Spark.</span>writable (method, description, clean)](#apidoc.element.primus.Spark.writable)
- description and source-code
```javascript
function predefined(method, description, clean) {
  //
  // If we are given a description compatible Object, use that instead of
  // setting it as value. This allows easy creation of getters and setters.
  //
  if (
       !predefine.descriptor(description)
    || is(description, 'object')
       && !clean
       && !predefine.descriptor(predefine.mixin({}, pattern, description))
  ) { description = {
      value: description
    };
  }

  //
  // Prevent thrown errors when we attempt to override a readonly
  // property
  //
  var described = Object.getOwnPropertyDescriptor(obj, method);
  if (described && !described.configurable) {
    return predefined;
  }

  Object.defineProperty(obj, method, !clean
    ? predefine.mixin({}, pattern, description)
    : description
  );

  return predefined;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.primus.Transformer"></a>[module primus.Transformer](#apidoc.module.primus.Transformer)

#### <a name="apidoc.element.primus.Transformer.Transformer"></a>[function <span class="apidocSignatureSpan">primus.</span>Transformer (primus)](#apidoc.element.primus.Transformer.Transformer)
- description and source-code
```javascript
function Transformer(primus) {
  this.fuse();

  this.ultron = new Ultron(primus.server);  // Handles listeners with ease.
  this.Spark = primus.Spark;                // Reference to the Spark constructor.
  this.primus = primus;                     // Reference to the Primus instance.
  this.service = null;                      // Stores the real-time service.

  this.initialise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Transformer.extend"></a>[function <span class="apidocSignatureSpan">primus.Transformer.</span>extend (protoProps, staticProps)](#apidoc.element.primus.Transformer.extend)
- description and source-code
```javascript
function extend(protoProps, staticProps) {
  var parent = this
    , child;

  //
  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  //
  if (protoProps && has.call(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = mode(parent);
  }

  //
  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  //
  function Surrogate() {
    this.constructor = child;
  }

  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  //
  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  //
  if (protoProps) mixin(child.prototype, protoProps);

  //
  // Add static properties to the constructor function, if supplied.
  //
  copypaste(child, parent, staticProps);

  //
  // Set a convenience property in case the parent's prototype is needed later.
  //
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Transformer.get"></a>[function <span class="apidocSignatureSpan">primus.Transformer.</span>get (method, getter)](#apidoc.element.primus.Transformer.get)
- description and source-code
```javascript
function get(method, getter) {
  Object.defineProperty(Base.prototype, method, {
    configurable: false,
    enumerable: false,
    get: getter
  });

  return get;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Transformer.predefine"></a>[function <span class="apidocSignatureSpan">primus.Transformer.</span>predefine (obj, pattern)](#apidoc.element.primus.Transformer.predefine)
- description and source-code
```javascript
function predefine(obj, pattern) {
  pattern = pattern || predefine.READABLE;

  return function predefined(method, description, clean) {
    //
    // If we are given a description compatible Object, use that instead of
    // setting it as value. This allows easy creation of getters and setters.
    //
    if (
         !predefine.descriptor(description)
      || is(description, 'object')
         && !clean
         && !predefine.descriptor(predefine.mixin({}, pattern, description))
    ) { description = {
        value: description
      };
    }

    //
    // Prevent thrown errors when we attempt to override a readonly
    // property
    //
    var described = Object.getOwnPropertyDescriptor(obj, method);
    if (described && !described.configurable) {
      return predefined;
    }

    Object.defineProperty(obj, method, !clean
      ? predefine.mixin({}, pattern, description)
      : description
    );

    return predefined;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Transformer.readable"></a>[function <span class="apidocSignatureSpan">primus.Transformer.</span>readable (method, description, clean)](#apidoc.element.primus.Transformer.readable)
- description and source-code
```javascript
function predefined(method, description, clean) {
  //
  // If we are given a description compatible Object, use that instead of
  // setting it as value. This allows easy creation of getters and setters.
  //
  if (
       !predefine.descriptor(description)
    || is(description, 'object')
       && !clean
       && !predefine.descriptor(predefine.mixin({}, pattern, description))
  ) { description = {
      value: description
    };
  }

  //
  // Prevent thrown errors when we attempt to override a readonly
  // property
  //
  var described = Object.getOwnPropertyDescriptor(obj, method);
  if (described && !described.configurable) {
    return predefined;
  }

  Object.defineProperty(obj, method, !clean
    ? predefine.mixin({}, pattern, description)
    : description
  );

  return predefined;
}
```
- example usage
```shell
...
 * Simple function to output common errors.
 *
 * @param {String} what What is missing.
 * @param {Object} where Either Primus.parsers or Primus.transformers.
 * @returns {Object}
 * @api private
 */
Primus.readable('is', function is(what, where) {
var missing = Primus.parsers !== where
    ? 'transformer'
    : 'parser'
  , dependency = where[what];

return {
  missing: function write() {
...
```

#### <a name="apidoc.element.primus.Transformer.set"></a>[function <span class="apidocSignatureSpan">primus.Transformer.</span>set (method, getter, setter)](#apidoc.element.primus.Transformer.set)
- description and source-code
```javascript
function set(method, getter, setter) {
  Object.defineProperty(Base.prototype, method, {
    configurable: false,
    enumerable: false,
    get: getter,
    set: setter
  });

  return set;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.Transformer.writable"></a>[function <span class="apidocSignatureSpan">primus.Transformer.</span>writable (method, description, clean)](#apidoc.element.primus.Transformer.writable)
- description and source-code
```javascript
function predefined(method, description, clean) {
  //
  // If we are given a description compatible Object, use that instead of
  // setting it as value. This allows easy creation of getters and setters.
  //
  if (
       !predefine.descriptor(description)
    || is(description, 'object')
       && !clean
       && !predefine.descriptor(predefine.mixin({}, pattern, description))
  ) { description = {
      value: description
    };
  }

  //
  // Prevent thrown errors when we attempt to override a readonly
  // property
  //
  var described = Object.getOwnPropertyDescriptor(obj, method);
  if (described && !described.configurable) {
    return predefined;
  }

  Object.defineProperty(obj, method, !clean
    ? predefine.mixin({}, pattern, description)
    : description
  );

  return predefined;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.primus.errors"></a>[module primus.errors](#apidoc.module.primus.errors)

#### <a name="apidoc.element.primus.errors.ParserError"></a>[function <span class="apidocSignatureSpan">primus.errors.</span>ParserError (message, spark)](#apidoc.element.primus.errors.ParserError)
- description and source-code
```javascript
function ParserError(message, spark) {
  Error.captureStackTrace(this, this.constructor);

  this.message = message;
  this.name = this.constructor.name;

  if (spark) {
    if (spark.listeners('error').length) spark.emit('error', this);
    spark.primus.emit('log', 'error', this);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.errors.PrimusError"></a>[function <span class="apidocSignatureSpan">primus.errors.</span>PrimusError (message, logger)](#apidoc.element.primus.errors.PrimusError)
- description and source-code
```javascript
function PrimusError(message, logger) {
  Error.captureStackTrace(this, this.constructor);

  this.message = message;
  this.name = this.constructor.name;

  if (logger) {
    logger.emit('log', 'error', this);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.primus.json"></a>[module primus.json](#apidoc.module.primus.json)

#### <a name="apidoc.element.primus.json.decoder"></a>[function <span class="apidocSignatureSpan">primus.json.</span>decoder (data, fn)](#apidoc.element.primus.json.decoder)
- description and source-code
```javascript
function decoder(data, fn) {
  var err;

  if ('string' !== typeof data) return fn(err, data);

  try { data = JSON.parse(data); }
  catch (e) { err = e; }

  fn(err, data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.json.encoder"></a>[function <span class="apidocSignatureSpan">primus.json.</span>encoder (data, fn)](#apidoc.element.primus.json.encoder)
- description and source-code
```javascript
function encoder(data, fn) {
  var err;

  try { data = JSON.stringify(data); }
  catch (e) { err = e; }

  fn(err, data);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.primus.predefine"></a>[module primus.predefine](#apidoc.module.primus.predefine)

#### <a name="apidoc.element.primus.predefine.predefine"></a>[function <span class="apidocSignatureSpan">primus.</span>predefine (obj, pattern)](#apidoc.element.primus.predefine.predefine)
- description and source-code
```javascript
function predefine(obj, pattern) {
  pattern = pattern || predefine.READABLE;

  return function predefined(method, description, clean) {
    //
    // If we are given a description compatible Object, use that instead of
    // setting it as value. This allows easy creation of getters and setters.
    //
    if (
         !predefine.descriptor(description)
      || is(description, 'object')
         && !clean
         && !predefine.descriptor(predefine.mixin({}, pattern, description))
    ) { description = {
        value: description
      };
    }

    //
    // Prevent thrown errors when we attempt to override a readonly
    // property
    //
    var described = Object.getOwnPropertyDescriptor(obj, method);
    if (described && !described.configurable) {
      return predefined;
    }

    Object.defineProperty(obj, method, !clean
      ? predefine.mixin({}, pattern, description)
      : description
    );

    return predefined;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.predefine.create"></a>[function <span class="apidocSignatureSpan">primus.predefine.</span>create (property, description, pattern)](#apidoc.element.primus.predefine.create)
- description and source-code
```javascript
function create(property, description, pattern) {
  pattern = pattern || {};

  if (!predefine.descriptor(description)) description = {
    enumberable: false,
    value: description
  };

  var definition = {};
  definition[property] = predefine.mixin(pattern, description);

  return definition;
}
```
- example usage
```shell
...
  throw new PrimusError('The 'timeout' option has been removed', this);
}

var primus = this
  , key;

this.auth = options.authorization || null;  // Do we have an authorization handler.
this.connections = Object.create(null);     // Connection storage.
this.ark = Object.create(null);             // Plugin storage.
this.layers = [];                           // Middleware layers.
this.heartbeatInterval = null;              // The heartbeat interval.
this.transformer = null;                    // Reference to the real-time engine instance.
this.encoder = null;                        // Shorthand to the parser's encoder.
this.decoder = null;                        // Shorthand to the parser's decoder.
this.connected = 0;                         // Connection counter.
...
```

#### <a name="apidoc.element.primus.predefine.descriptor"></a>[function <span class="apidocSignatureSpan">primus.predefine.</span>descriptor (obj)](#apidoc.element.primus.predefine.descriptor)
- description and source-code
```javascript
function descriptor(obj) {
  if (!obj || 'object' !== typeof obj || Array.isArray(obj)) return false;

  var keys = Object.keys(obj);

  //
  // A descriptor can only be a data or accessor descriptor, never both.
  // An data descriptor can only specify:
  //
  // - configurable
  // - enumerable
  // - (optional) value
  // - (optional) writable
  //
  // And an accessor descriptor can only specify;
  //
  // - configurable
  // - enumerable
  // - (optional) get
  // - (optional) set
  //
  if (
       ('value' in obj || 'writable' in obj)
    && ('function' === typeof obj.set || 'function' === typeof obj.get)
  ) return false;

  return !!keys.length && keys.every(function allowed(key) {
    var type = description[key]
      , valid = type === undefined || is(obj[key], type);

    return key in description && valid;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.predefine.each"></a>[function <span class="apidocSignatureSpan">primus.predefine.</span>each (collection, iterator, context)](#apidoc.element.primus.predefine.each)
- description and source-code
```javascript
function each(collection, iterator, context) {
  if (arguments.length === 1) {
    iterator = collection;
    collection = this;
  }

  var isArray = Array.isArray(collection || this)
    , length = collection.length
    , i = 0
    , value;

  if (context) {
    if (isArray) {
      for (; i < length; i++) {
        value = iterator.apply(collection[ i ], context);
        if (value === false) break;
      }
    } else {
      for (i in collection) {
        value = iterator.apply(collection[ i ], context);
        if (value === false) break;
      }
    }
  } else {
    if (isArray) {
      for (; i < length; i++) {
        value = iterator.call(collection[i], i, collection[i]);
        if (value === false) break;
      }
    } else {
      for (i in collection) {
        value = iterator.call(collection[i], i, collection[i]);
        if (value === false) break;
      }
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.predefine.extend"></a>[function <span class="apidocSignatureSpan">primus.predefine.</span>extend (protoProps, staticProps)](#apidoc.element.primus.predefine.extend)
- description and source-code
```javascript
function extend(protoProps, staticProps) {
  var parent = this
    , child;

  //
  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  //
  if (protoProps && has.call(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = mode(parent);
  }

  //
  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  //
  function Surrogate() {
    this.constructor = child;
  }

  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  //
  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  //
  if (protoProps) mixin(child.prototype, protoProps);

  //
  // Add static properties to the constructor function, if supplied.
  //
  copypaste(child, parent, staticProps);

  //
  // Set a convenience property in case the parent's prototype is needed later.
  //
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.predefine.lazy"></a>[function <span class="apidocSignatureSpan">primus.predefine.</span>lazy (obj, prop, fn)](#apidoc.element.primus.predefine.lazy)
- description and source-code
```javascript
function lazy(obj, prop, fn) {
  Object.defineProperty(obj, prop, {
    configurable: true,

    get: function get() {
      return Object.defineProperty(this, prop, {
        value: fn.call(this)
      })[prop];
    },

    set: function set(value) {
      return Object.defineProperty(this, prop, {
        value: value
      })[prop];
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.predefine.merge"></a>[function <span class="apidocSignatureSpan">primus.predefine.</span>merge (target, additional)](#apidoc.element.primus.predefine.merge)
- description and source-code
```javascript
function merge(target, additional) {
  var result = target
    , undefined;

  if (Array.isArray(target)) {
    each(additional, function arrayForEach(index) {
      if (JSON.stringify(target).indexOf(JSON.stringify(additional[index])) === -1) {
        result.push(additional[index]);
      }
    });
  } else if ('object' === typeof target) {
    each(additional, function objectForEach(key, value) {
      if (target[key] === undefined) {
        result[key] = value;
      } else {
        result[key] = merge(target[key], additional[key]);
      }
    });
  } else {
    result = additional;
  }

  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.predefine.mixin"></a>[function <span class="apidocSignatureSpan">primus.predefine.</span>mixin (target)](#apidoc.element.primus.predefine.mixin)
- description and source-code
```javascript
function mixin(target) {
  Array.prototype.slice.call(arguments, 1).forEach(function forEach(o) {
    Object.getOwnPropertyNames(o).forEach(function eachAttr(attr) {
      Object.defineProperty(target, attr, Object.getOwnPropertyDescriptor(o, attr));
    });
  });

  return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.primus.predefine.remove"></a>[function <span class="apidocSignatureSpan">primus.predefine.</span>remove (obj, keep)](#apidoc.element.primus.predefine.remove)
- description and source-code
```javascript
function remove(obj, keep) {
  if (!obj) return false;
  keep = keep || [];

  for (var prop in obj) {
    if (has.call(obj, prop) && !~keep.indexOf(prop)) {
      delete obj[prop];
    }
  }

  return true;
}
```
- example usage
```shell
...
'''js
// add a middleware after the first two in the stack
primus.use('name', function (req, res) {

}, 2);
'''

#### Primus.remove(name)

This method allows you to remove configured middleware. This works
for the middleware layers that you added but also the middleware layers that we
add by default. If you want to use a different way to serve the 'primus.js'
file you can simply:

'''js
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
