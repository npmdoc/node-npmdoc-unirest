# api documentation for  [unirest (v0.5.1)](https://github.com/Mashape/unirest-nodejs#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-unirest.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-unirest) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-unirest.svg)](https://travis-ci.org/npmdoc/node-npmdoc-unirest)
#### Simplified, lightweight HTTP client library

[![NPM](https://nodei.co/npm/unirest.png?downloads=true)](https://www.npmjs.com/package/unirest)

[![apidoc](https://npmdoc.github.io/node-npmdoc-unirest/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-unirest_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-unirest/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-unirest/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-unirest/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mashape",
        "email": "opensource@mashape.com",
        "url": "https://www.mashape.com"
    },
    "bugs": {
        "url": "https://github.com/Mashape/unirest-nodejs/issues"
    },
    "dependencies": {
        "form-data": "^0.2.0",
        "mime": "~1.3.4",
        "request": "~2.74.0"
    },
    "description": "Simplified, lightweight HTTP client library",
    "devDependencies": {
        "body-parser": "^1.15.1",
        "express": "^4.13.4",
        "mocha": "~2.4.5",
        "should": "~8.3.1"
    },
    "directories": {
        "test": "tests"
    },
    "dist": {
        "shasum": "9df5766187280f245b4e9a75ce1fad313337d6ed",
        "tarball": "https://registry.npmjs.org/unirest/-/unirest-0.5.1.tgz"
    },
    "gitHead": "028e4fd2b104b4209e54cd871f83cde1e6a49605",
    "homepage": "https://github.com/Mashape/unirest-nodejs#readme",
    "keywords": [
        "request",
        "http",
        "library",
        "superagent",
        "simple",
        "util",
        "utility",
        "method"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "nijikokun",
            "email": "nijikokun@gmail.com"
        }
    ],
    "name": "unirest",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/Mashape/unirest-nodejs.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "0.5.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module unirest](#apidoc.module.unirest)
1.  [function <span class="apidocSignatureSpan">unirest.</span>cookie (str)](#apidoc.element.unirest.cookie)
1.  [function <span class="apidocSignatureSpan">unirest.</span>delete (uri, headers, body, callback)](#apidoc.element.unirest.delete)
1.  [function <span class="apidocSignatureSpan">unirest.</span>firstMatch (string, map)](#apidoc.element.unirest.firstMatch)
1.  [function <span class="apidocSignatureSpan">unirest.</span>get (uri, headers, body, callback)](#apidoc.element.unirest.get)
1.  [function <span class="apidocSignatureSpan">unirest.</span>head (uri, headers, body, callback)](#apidoc.element.unirest.head)
1.  [function <span class="apidocSignatureSpan">unirest.</span>jar (options)](#apidoc.element.unirest.jar)
1.  [function <span class="apidocSignatureSpan">unirest.</span>matches (string, map)](#apidoc.element.unirest.matches)
1.  [function <span class="apidocSignatureSpan">unirest.</span>options (uri, headers, body, callback)](#apidoc.element.unirest.options)
1.  [function <span class="apidocSignatureSpan">unirest.</span>patch (uri, headers, body, callback)](#apidoc.element.unirest.patch)
1.  [function <span class="apidocSignatureSpan">unirest.</span>post (uri, headers, body, callback)](#apidoc.element.unirest.post)
1.  [function <span class="apidocSignatureSpan">unirest.</span>put (uri, headers, body, callback)](#apidoc.element.unirest.put)
1.  [function <span class="apidocSignatureSpan">unirest.</span>request (uri, options, callback)](#apidoc.element.unirest.request)
1.  [function <span class="apidocSignatureSpan">unirest.</span>request.Request (options)](#apidoc.element.unirest.request.Request)
1.  [function <span class="apidocSignatureSpan">unirest.</span>trim (s)](#apidoc.element.unirest.trim)
1.  [function <span class="apidocSignatureSpan">unirest.</span>type (type, parse)](#apidoc.element.unirest.type)
1.  object <span class="apidocSignatureSpan">unirest.</span>Request
1.  object <span class="apidocSignatureSpan">unirest.</span>Response
1.  object <span class="apidocSignatureSpan">unirest.</span>enum
1.  object <span class="apidocSignatureSpan">unirest.</span>parsers
1.  object <span class="apidocSignatureSpan">unirest.</span>request.Request.prototype
1.  object <span class="apidocSignatureSpan">unirest.</span>serializers

#### [module unirest.Request](#apidoc.module.unirest.Request)
1.  [function <span class="apidocSignatureSpan">unirest.Request.</span>serialize (string, type)](#apidoc.element.unirest.Request.serialize)
1.  [function <span class="apidocSignatureSpan">unirest.Request.</span>uid (len)](#apidoc.element.unirest.Request.uid)

#### [module unirest.Response](#apidoc.module.unirest.Response)
1.  [function <span class="apidocSignatureSpan">unirest.Response.</span>parse (string, type)](#apidoc.element.unirest.Response.parse)
1.  [function <span class="apidocSignatureSpan">unirest.Response.</span>parseHeader (str)](#apidoc.element.unirest.Response.parseHeader)
1.  object <span class="apidocSignatureSpan">unirest.Response.</span>statusCodes

#### [module unirest.parsers](#apidoc.module.unirest.parsers)
1.  [function <span class="apidocSignatureSpan">unirest.parsers.</span>json (data)](#apidoc.element.unirest.parsers.json)
1.  [function <span class="apidocSignatureSpan">unirest.parsers.</span>string (data)](#apidoc.element.unirest.parsers.string)

#### [module unirest.request](#apidoc.module.unirest.request)
1.  [function <span class="apidocSignatureSpan">unirest.</span>request (uri, options, callback)](#apidoc.element.unirest.request.request)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>Request (options)](#apidoc.element.unirest.request.Request)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>cookie (str)](#apidoc.element.unirest.request.cookie)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>defaults (options, requester)](#apidoc.element.unirest.request.defaults)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>del (uri, options, callback)](#apidoc.element.unirest.request.del)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>delete (uri, options, callback)](#apidoc.element.unirest.request.delete)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>forever (agentOptions, optionsArg)](#apidoc.element.unirest.request.forever)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>get (uri, options, callback)](#apidoc.element.unirest.request.get)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>head (uri, options, callback)](#apidoc.element.unirest.request.head)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>initParams (uri, options, callback)](#apidoc.element.unirest.request.initParams)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>jar (store)](#apidoc.element.unirest.request.jar)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>patch (uri, options, callback)](#apidoc.element.unirest.request.patch)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>post (uri, options, callback)](#apidoc.element.unirest.request.post)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>put (uri, options, callback)](#apidoc.element.unirest.request.put)

#### [module unirest.request.Request](#apidoc.module.unirest.request.Request)
1.  [function <span class="apidocSignatureSpan">unirest.request.</span>Request (options)](#apidoc.element.unirest.request.Request.Request)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.</span>super_ ()](#apidoc.element.unirest.request.Request.super_)
1.  object <span class="apidocSignatureSpan">unirest.request.Request.</span>defaultProxyHeaderExclusiveList
1.  object <span class="apidocSignatureSpan">unirest.request.Request.</span>defaultProxyHeaderWhiteList

#### [module unirest.request.Request.prototype](#apidoc.module.unirest.request.Request.prototype)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>abort ()](#apidoc.element.unirest.request.Request.prototype.abort)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>auth (user, pass, sendImmediately, bearer)](#apidoc.element.unirest.request.Request.prototype.auth)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>aws (opts, now)](#apidoc.element.unirest.request.Request.prototype.aws)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>debug ()](#apidoc.element.unirest.request.Request.prototype.debug)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>destroy ()](#apidoc.element.unirest.request.Request.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>enableUnixSocket ()](#apidoc.element.unirest.request.Request.prototype.enableUnixSocket)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>end (chunk)](#apidoc.element.unirest.request.Request.prototype.end)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>form (form)](#apidoc.element.unirest.request.Request.prototype.form)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>getHeader (name, headers)](#apidoc.element.unirest.request.Request.prototype.getHeader)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>getNewAgent ()](#apidoc.element.unirest.request.Request.prototype.getNewAgent)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>hawk (opts)](#apidoc.element.unirest.request.Request.prototype.hawk)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>httpSignature (opts)](#apidoc.element.unirest.request.Request.prototype.httpSignature)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>init (options)](#apidoc.element.unirest.request.Request.prototype.init)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>jar (jar)](#apidoc.element.unirest.request.Request.prototype.jar)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>json (val)](#apidoc.element.unirest.request.Request.prototype.json)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>multipart (multipart)](#apidoc.element.unirest.request.Request.prototype.multipart)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>oauth (_oauth)](#apidoc.element.unirest.request.Request.prototype.oauth)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>onRequestError (error)](#apidoc.element.unirest.request.Request.prototype.onRequestError)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>onRequestResponse (response)](#apidoc.element.unirest.request.Request.prototype.onRequestResponse)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>pause ()](#apidoc.element.unirest.request.Request.prototype.pause)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>pipe (dest, opts)](#apidoc.element.unirest.request.Request.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>pipeDest (dest)](#apidoc.element.unirest.request.Request.prototype.pipeDest)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>qs (q, clobber)](#apidoc.element.unirest.request.Request.prototype.qs)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>readResponseBody (response)](#apidoc.element.unirest.request.Request.prototype.readResponseBody)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>resume ()](#apidoc.element.unirest.request.Request.prototype.resume)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>start ()](#apidoc.element.unirest.request.Request.prototype.start)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>toJSON ()](#apidoc.element.unirest.request.Request.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>write ()](#apidoc.element.unirest.request.Request.prototype.write)

#### [module unirest.serializers](#apidoc.module.unirest.serializers)
1.  [function <span class="apidocSignatureSpan">unirest.serializers.</span>form (obj)](#apidoc.element.unirest.serializers.form)
1.  [function <span class="apidocSignatureSpan">unirest.serializers.</span>json (obj)](#apidoc.element.unirest.serializers.json)



# <a name="apidoc.module.unirest"></a>[module unirest](#apidoc.module.unirest)

#### <a name="apidoc.element.unirest.cookie"></a>[function <span class="apidocSignatureSpan">unirest.</span>cookie (str)](#apidoc.element.unirest.cookie)
- description and source-code
```javascript
cookie = function (str) {
  return cookies.parse(str)
}
```
- example usage
```shell
...

'''js
var CookieJar = unirest.jar();
CookieJar.add('key=value', '/'); // Cookie string, pathname / url
unirest.get('http://mockbin.com/request').jar(CookieJar);
'''

## unirest.cookie(String)

Creates a cookie, see above for example.

## unirest.request

'mikeal/request' library (the underlying layer of unirest) for direct use.
...
```

#### <a name="apidoc.element.unirest.delete"></a>[function <span class="apidocSignatureSpan">unirest.</span>delete (uri, headers, body, callback)](#apidoc.element.unirest.delete)
- description and source-code
```javascript
delete = function (uri, headers, body, callback) {
  var $this = {
<span class="apidocCodeCommentSpan">    /**
     * Stream Multipart form-data request
     *
     * @type {Boolean}
     */
</span>    _stream: false,

    /**
     * Container to hold multipart form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _multipart: [],

    /**
     * Container to hold form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _form: [],

    /**
     * Request option container for details about the request.
     *
     * @type {Object}
     */
    options: {
      /**
       * Url obtained from request method arguments.
       *
       * @type {String}
       */
      url: uri,

      /**
       * Method obtained from request method arguments.
       *
       * @type {String}
       */
      method: method,

      /**
       * List of headers with case-sensitive fields.
       *
       * @type {Object}
       */
      headers: {}
    },

    hasHeader: function (name) {
      var headers
      var lowercaseHeaders

      name = name.toLowerCase()
      headers = Object.keys($this.options.headers)
      lowercaseHeaders = headers.map(function (header) {
        return header.toLowerCase()
      })

      for (var i = 0; i < lowercaseHeaders.length; i++) {
        if (lowercaseHeaders[i] === name) {
          return headers[i]
        }
      }

      return false
    },

    /**
     * Turn on multipart-form streaming
     *
     * @return {Object}
     */
    stream: function () {
      $this._stream = true
      return this
    },

    /**
     * Attaches a field to the multipart-form request, with pre-processing.
     *
     * @param  {String} name
     * @param  {String} value
     * @return {Object}
     */
    field: function (name, value, options) {
      return handleField(name, value, options)
    },

    /**
     * Attaches a file to the multipart-form request.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @return {Object}
     */
    attach: function (name, path, options) {
      options = options || {}
      options.attachment = true
      return handleField(name, path, options)
    },

    /**
     * Attaches field to the multipart-form request, with no pre-processing.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @param  {Object} options
     * @return {Object}
     */
    rawField: function (name, value, options) {
      $this._multipart.push({
        name: name,
        value: value,
        options: options,
        attachment: options.attachment || false
      })
    },

    /**
     * Basic Header Authentication Method
     *
     * Supports user being an Object to reflect Request
     * Supports user, password to reflect SuperAgent
     *
     * @param  {String|Object} user
     * @param  {String} password
     * @param  {Boolean} sendImmediately
     * @return {Object}
     */
    auth: function (user, password, sendImmediately) {
      $this.options.auth = (is(user).a(Object)) ? user : {
        user: user,
        password: password,
        sendImmediately: sendImmediately
      }

      return $this
    },

    /**
     * Sets header field to value
     *
     * @param  {String} field Header field
     * @param  {String} value Header field value
     * @return {Object}
     */
    header: function (field, value) {
      if (is(field).a(Object)) {
        for (var key in field) {
          if (field.hasOwnProperty(key)) {
            $this.header(key, field[key])
          }
        }

        return $this
      }

      var existingHeaderName = $this.hasHeader(field)
      $this.options.headers[existingHeaderName || field] = value

      return $this
    },

    /**
     * Serialize value as querystring representation, and append or set on 'Request.options.url'
     *
     * @param  {String|Object} value
     * @return {Object}
     */
    query: function (value) {
      if (is(value).a(Object)) value = Unirest.serializers.form(value)
      if (!value.length) return $this
      $this.options.url += (does($this.o ...
```
- example usage
```shell
...
var Request = unirest.patch('http://mockbin.com/request');
'''

### delete
Returns a [Request](#request) object with the 'method' option set to 'DELETE'

'''js
var Request = unirest.delete('http://mockbin.com/request');
'''

## unirest.jar()

Creates a container to store multiple cookies, i.e. a cookie jar.

'''js
...
```

#### <a name="apidoc.element.unirest.firstMatch"></a>[function <span class="apidocSignatureSpan">unirest.</span>firstMatch (string, map)](#apidoc.element.unirest.firstMatch)
- description and source-code
```javascript
function firstMatch(string, map) {
  return Unirest.matches(string, map)[0]
}
```
- example usage
```shell
...
/**
 * Unirest Request Utility Methods
 *
 * @type {Object}
 */
Unirest.Request = {
serialize: function (string, type) {
  var serializer = Unirest.firstMatch(type, Unirest.enum.serialize)
  return serializer ? serializer(string) : string
},

uid: function (len) {
  var output = ''
  var chars = 'abcdefghijklmnopqrstuvwxyz123456789'
  var nchars = chars.length
...
```

#### <a name="apidoc.element.unirest.get"></a>[function <span class="apidocSignatureSpan">unirest.</span>get (uri, headers, body, callback)](#apidoc.element.unirest.get)
- description and source-code
```javascript
get = function (uri, headers, body, callback) {
  var $this = {
<span class="apidocCodeCommentSpan">    /**
     * Stream Multipart form-data request
     *
     * @type {Boolean}
     */
</span>    _stream: false,

    /**
     * Container to hold multipart form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _multipart: [],

    /**
     * Container to hold form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _form: [],

    /**
     * Request option container for details about the request.
     *
     * @type {Object}
     */
    options: {
      /**
       * Url obtained from request method arguments.
       *
       * @type {String}
       */
      url: uri,

      /**
       * Method obtained from request method arguments.
       *
       * @type {String}
       */
      method: method,

      /**
       * List of headers with case-sensitive fields.
       *
       * @type {Object}
       */
      headers: {}
    },

    hasHeader: function (name) {
      var headers
      var lowercaseHeaders

      name = name.toLowerCase()
      headers = Object.keys($this.options.headers)
      lowercaseHeaders = headers.map(function (header) {
        return header.toLowerCase()
      })

      for (var i = 0; i < lowercaseHeaders.length; i++) {
        if (lowercaseHeaders[i] === name) {
          return headers[i]
        }
      }

      return false
    },

    /**
     * Turn on multipart-form streaming
     *
     * @return {Object}
     */
    stream: function () {
      $this._stream = true
      return this
    },

    /**
     * Attaches a field to the multipart-form request, with pre-processing.
     *
     * @param  {String} name
     * @param  {String} value
     * @return {Object}
     */
    field: function (name, value, options) {
      return handleField(name, value, options)
    },

    /**
     * Attaches a file to the multipart-form request.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @return {Object}
     */
    attach: function (name, path, options) {
      options = options || {}
      options.attachment = true
      return handleField(name, path, options)
    },

    /**
     * Attaches field to the multipart-form request, with no pre-processing.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @param  {Object} options
     * @return {Object}
     */
    rawField: function (name, value, options) {
      $this._multipart.push({
        name: name,
        value: value,
        options: options,
        attachment: options.attachment || false
      })
    },

    /**
     * Basic Header Authentication Method
     *
     * Supports user being an Object to reflect Request
     * Supports user, password to reflect SuperAgent
     *
     * @param  {String|Object} user
     * @param  {String} password
     * @param  {Boolean} sendImmediately
     * @return {Object}
     */
    auth: function (user, password, sendImmediately) {
      $this.options.auth = (is(user).a(Object)) ? user : {
        user: user,
        password: password,
        sendImmediately: sendImmediately
      }

      return $this
    },

    /**
     * Sets header field to value
     *
     * @param  {String} field Header field
     * @param  {String} value Header field value
     * @return {Object}
     */
    header: function (field, value) {
      if (is(field).a(Object)) {
        for (var key in field) {
          if (field.hasOwnProperty(key)) {
            $this.header(key, field[key])
          }
        }

        return $this
      }

      var existingHeaderName = $this.hasHeader(field)
      $this.options.headers[existingHeaderName || field] = value

      return $this
    },

    /**
     * Serialize value as querystring representation, and append or set on 'Request.options.url'
     *
     * @param  {String|Object} value
     * @return {Object}
     */
    query: function (value) {
      if (is(value).a(Object)) value = Unirest.serializers.form(value)
      if (!value.length) return $this
      $this.options.url += (does($this.o ...
```
- example usage
```shell
...
When no 'callback' is present, the [Request](#request) object will be returned.

### get

Returns a [Request](#request) object with the 'method' option set to 'GET'

'''js
var Request = unirest.get('http://mockbin.com/request');
'''

### head
Returns a [Request](#request) object with the 'method' option set to 'HEAD'

'''js
var Request = unirest.head('http://mockbin.com/request');
...
```

#### <a name="apidoc.element.unirest.head"></a>[function <span class="apidocSignatureSpan">unirest.</span>head (uri, headers, body, callback)](#apidoc.element.unirest.head)
- description and source-code
```javascript
head = function (uri, headers, body, callback) {
  var $this = {
<span class="apidocCodeCommentSpan">    /**
     * Stream Multipart form-data request
     *
     * @type {Boolean}
     */
</span>    _stream: false,

    /**
     * Container to hold multipart form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _multipart: [],

    /**
     * Container to hold form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _form: [],

    /**
     * Request option container for details about the request.
     *
     * @type {Object}
     */
    options: {
      /**
       * Url obtained from request method arguments.
       *
       * @type {String}
       */
      url: uri,

      /**
       * Method obtained from request method arguments.
       *
       * @type {String}
       */
      method: method,

      /**
       * List of headers with case-sensitive fields.
       *
       * @type {Object}
       */
      headers: {}
    },

    hasHeader: function (name) {
      var headers
      var lowercaseHeaders

      name = name.toLowerCase()
      headers = Object.keys($this.options.headers)
      lowercaseHeaders = headers.map(function (header) {
        return header.toLowerCase()
      })

      for (var i = 0; i < lowercaseHeaders.length; i++) {
        if (lowercaseHeaders[i] === name) {
          return headers[i]
        }
      }

      return false
    },

    /**
     * Turn on multipart-form streaming
     *
     * @return {Object}
     */
    stream: function () {
      $this._stream = true
      return this
    },

    /**
     * Attaches a field to the multipart-form request, with pre-processing.
     *
     * @param  {String} name
     * @param  {String} value
     * @return {Object}
     */
    field: function (name, value, options) {
      return handleField(name, value, options)
    },

    /**
     * Attaches a file to the multipart-form request.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @return {Object}
     */
    attach: function (name, path, options) {
      options = options || {}
      options.attachment = true
      return handleField(name, path, options)
    },

    /**
     * Attaches field to the multipart-form request, with no pre-processing.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @param  {Object} options
     * @return {Object}
     */
    rawField: function (name, value, options) {
      $this._multipart.push({
        name: name,
        value: value,
        options: options,
        attachment: options.attachment || false
      })
    },

    /**
     * Basic Header Authentication Method
     *
     * Supports user being an Object to reflect Request
     * Supports user, password to reflect SuperAgent
     *
     * @param  {String|Object} user
     * @param  {String} password
     * @param  {Boolean} sendImmediately
     * @return {Object}
     */
    auth: function (user, password, sendImmediately) {
      $this.options.auth = (is(user).a(Object)) ? user : {
        user: user,
        password: password,
        sendImmediately: sendImmediately
      }

      return $this
    },

    /**
     * Sets header field to value
     *
     * @param  {String} field Header field
     * @param  {String} value Header field value
     * @return {Object}
     */
    header: function (field, value) {
      if (is(field).a(Object)) {
        for (var key in field) {
          if (field.hasOwnProperty(key)) {
            $this.header(key, field[key])
          }
        }

        return $this
      }

      var existingHeaderName = $this.hasHeader(field)
      $this.options.headers[existingHeaderName || field] = value

      return $this
    },

    /**
     * Serialize value as querystring representation, and append or set on 'Request.options.url'
     *
     * @param  {String|Object} value
     * @return {Object}
     */
    query: function (value) {
      if (is(value).a(Object)) value = Unirest.serializers.form(value)
      if (!value.length) return $this
      $this.options.url += (does($this.o ...
```
- example usage
```shell
...
var Request = unirest.get('http://mockbin.com/request');
'''

### head
Returns a [Request](#request) object with the 'method' option set to 'HEAD'

'''js
var Request = unirest.head('http://mockbin.com/request');
'''

### put
Returns a [Request](#request) object with the 'method' option set to 'PUT'

'''js
var Request = unirest.put('http://mockbin.com/request');
...
```

#### <a name="apidoc.element.unirest.jar"></a>[function <span class="apidocSignatureSpan">unirest.</span>jar (options)](#apidoc.element.unirest.jar)
- description and source-code
```javascript
jar = function (options) {
  var jar = Unirest.request.jar()
  options = options || {}

  // Because Requests aliases toughcookie rather than returning.
  if (options.store) {
    jar._jar.store = options.store
  }

  if (options.rejectPublicSuffixes) {
    jar._jar.rejectPublicSuffixes = options.rejectPublicSuffixes
  }

  // Alias helper methods
  jar.add = jar.setCookie
  jar.toString = jar.getCookieString

  // Export
  return jar
}
```
- example usage
```shell
...
### delete
Returns a [Request](#request) object with the 'method' option set to 'DELETE'

'''js
var Request = unirest.delete('http://mockbin.com/request');
'''

## unirest.jar()

Creates a container to store multiple cookies, i.e. a cookie jar.

'''js
var CookieJar = unirest.jar();
CookieJar.add('key=value', '/'); // Cookie string, pathname / url
unirest.get('http://mockbin.com/request').jar(CookieJar);
...
```

#### <a name="apidoc.element.unirest.matches"></a>[function <span class="apidocSignatureSpan">unirest.</span>matches (string, map)](#apidoc.element.unirest.matches)
- description and source-code
```javascript
function matches(string, map) {
  var results = []

  for (var key in map) {
    if (typeof map.length !== 'undefined') {
      key = map[key]
    }

    if (string.indexOf(key) !== -1) {
      results.push(map[key])
    }
  }

  return results
}
```
- example usage
```shell
...
*
* @see #matches
* @param  {String} string String to be tested
* @param  {Object|Array} map Values / Keys to test against string.
* @return {Mixed} First match value
*/
Unirest.firstMatch = function firstMatch (string, map) {
 return Unirest.matches(string, map)[0]
}

/**
* Generate sugar for request library.
*
* This allows us to mock super-agent chaining style while using request library under the hood.
*/
...
```

#### <a name="apidoc.element.unirest.options"></a>[function <span class="apidocSignatureSpan">unirest.</span>options (uri, headers, body, callback)](#apidoc.element.unirest.options)
- description and source-code
```javascript
options = function (uri, headers, body, callback) {
  var $this = {
<span class="apidocCodeCommentSpan">    /**
     * Stream Multipart form-data request
     *
     * @type {Boolean}
     */
</span>    _stream: false,

    /**
     * Container to hold multipart form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _multipart: [],

    /**
     * Container to hold form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _form: [],

    /**
     * Request option container for details about the request.
     *
     * @type {Object}
     */
    options: {
      /**
       * Url obtained from request method arguments.
       *
       * @type {String}
       */
      url: uri,

      /**
       * Method obtained from request method arguments.
       *
       * @type {String}
       */
      method: method,

      /**
       * List of headers with case-sensitive fields.
       *
       * @type {Object}
       */
      headers: {}
    },

    hasHeader: function (name) {
      var headers
      var lowercaseHeaders

      name = name.toLowerCase()
      headers = Object.keys($this.options.headers)
      lowercaseHeaders = headers.map(function (header) {
        return header.toLowerCase()
      })

      for (var i = 0; i < lowercaseHeaders.length; i++) {
        if (lowercaseHeaders[i] === name) {
          return headers[i]
        }
      }

      return false
    },

    /**
     * Turn on multipart-form streaming
     *
     * @return {Object}
     */
    stream: function () {
      $this._stream = true
      return this
    },

    /**
     * Attaches a field to the multipart-form request, with pre-processing.
     *
     * @param  {String} name
     * @param  {String} value
     * @return {Object}
     */
    field: function (name, value, options) {
      return handleField(name, value, options)
    },

    /**
     * Attaches a file to the multipart-form request.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @return {Object}
     */
    attach: function (name, path, options) {
      options = options || {}
      options.attachment = true
      return handleField(name, path, options)
    },

    /**
     * Attaches field to the multipart-form request, with no pre-processing.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @param  {Object} options
     * @return {Object}
     */
    rawField: function (name, value, options) {
      $this._multipart.push({
        name: name,
        value: value,
        options: options,
        attachment: options.attachment || false
      })
    },

    /**
     * Basic Header Authentication Method
     *
     * Supports user being an Object to reflect Request
     * Supports user, password to reflect SuperAgent
     *
     * @param  {String|Object} user
     * @param  {String} password
     * @param  {Boolean} sendImmediately
     * @return {Object}
     */
    auth: function (user, password, sendImmediately) {
      $this.options.auth = (is(user).a(Object)) ? user : {
        user: user,
        password: password,
        sendImmediately: sendImmediately
      }

      return $this
    },

    /**
     * Sets header field to value
     *
     * @param  {String} field Header field
     * @param  {String} value Header field value
     * @return {Object}
     */
    header: function (field, value) {
      if (is(field).a(Object)) {
        for (var key in field) {
          if (field.hasOwnProperty(key)) {
            $this.header(key, field[key])
          }
        }

        return $this
      }

      var existingHeaderName = $this.hasHeader(field)
      $this.options.headers[existingHeaderName || field] = value

      return $this
    },

    /**
     * Serialize value as querystring representation, and append or set on 'Request.options.url'
     *
     * @param  {String|Object} value
     * @return {Object}
     */
    query: function (value) {
      if (is(value).a(Object)) value = Unirest.serializers.form(value)
      if (!value.length) return $this
      $this.options.url += (does($this.o ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.patch"></a>[function <span class="apidocSignatureSpan">unirest.</span>patch (uri, headers, body, callback)](#apidoc.element.unirest.patch)
- description and source-code
```javascript
patch = function (uri, headers, body, callback) {
  var $this = {
<span class="apidocCodeCommentSpan">    /**
     * Stream Multipart form-data request
     *
     * @type {Boolean}
     */
</span>    _stream: false,

    /**
     * Container to hold multipart form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _multipart: [],

    /**
     * Container to hold form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _form: [],

    /**
     * Request option container for details about the request.
     *
     * @type {Object}
     */
    options: {
      /**
       * Url obtained from request method arguments.
       *
       * @type {String}
       */
      url: uri,

      /**
       * Method obtained from request method arguments.
       *
       * @type {String}
       */
      method: method,

      /**
       * List of headers with case-sensitive fields.
       *
       * @type {Object}
       */
      headers: {}
    },

    hasHeader: function (name) {
      var headers
      var lowercaseHeaders

      name = name.toLowerCase()
      headers = Object.keys($this.options.headers)
      lowercaseHeaders = headers.map(function (header) {
        return header.toLowerCase()
      })

      for (var i = 0; i < lowercaseHeaders.length; i++) {
        if (lowercaseHeaders[i] === name) {
          return headers[i]
        }
      }

      return false
    },

    /**
     * Turn on multipart-form streaming
     *
     * @return {Object}
     */
    stream: function () {
      $this._stream = true
      return this
    },

    /**
     * Attaches a field to the multipart-form request, with pre-processing.
     *
     * @param  {String} name
     * @param  {String} value
     * @return {Object}
     */
    field: function (name, value, options) {
      return handleField(name, value, options)
    },

    /**
     * Attaches a file to the multipart-form request.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @return {Object}
     */
    attach: function (name, path, options) {
      options = options || {}
      options.attachment = true
      return handleField(name, path, options)
    },

    /**
     * Attaches field to the multipart-form request, with no pre-processing.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @param  {Object} options
     * @return {Object}
     */
    rawField: function (name, value, options) {
      $this._multipart.push({
        name: name,
        value: value,
        options: options,
        attachment: options.attachment || false
      })
    },

    /**
     * Basic Header Authentication Method
     *
     * Supports user being an Object to reflect Request
     * Supports user, password to reflect SuperAgent
     *
     * @param  {String|Object} user
     * @param  {String} password
     * @param  {Boolean} sendImmediately
     * @return {Object}
     */
    auth: function (user, password, sendImmediately) {
      $this.options.auth = (is(user).a(Object)) ? user : {
        user: user,
        password: password,
        sendImmediately: sendImmediately
      }

      return $this
    },

    /**
     * Sets header field to value
     *
     * @param  {String} field Header field
     * @param  {String} value Header field value
     * @return {Object}
     */
    header: function (field, value) {
      if (is(field).a(Object)) {
        for (var key in field) {
          if (field.hasOwnProperty(key)) {
            $this.header(key, field[key])
          }
        }

        return $this
      }

      var existingHeaderName = $this.hasHeader(field)
      $this.options.headers[existingHeaderName || field] = value

      return $this
    },

    /**
     * Serialize value as querystring representation, and append or set on 'Request.options.url'
     *
     * @param  {String|Object} value
     * @return {Object}
     */
    query: function (value) {
      if (is(value).a(Object)) value = Unirest.serializers.form(value)
      if (!value.length) return $this
      $this.options.url += (does($this.o ...
```
- example usage
```shell
...
'''

### patch

Returns a [Request](#request) object with the 'method' option set to 'PATCH'

'''js
var Request = unirest.patch('http://mockbin.com/request');
'''

### delete
Returns a [Request](#request) object with the 'method' option set to 'DELETE'

'''js
var Request = unirest.delete('http://mockbin.com/request');
...
```

#### <a name="apidoc.element.unirest.post"></a>[function <span class="apidocSignatureSpan">unirest.</span>post (uri, headers, body, callback)](#apidoc.element.unirest.post)
- description and source-code
```javascript
post = function (uri, headers, body, callback) {
  var $this = {
<span class="apidocCodeCommentSpan">    /**
     * Stream Multipart form-data request
     *
     * @type {Boolean}
     */
</span>    _stream: false,

    /**
     * Container to hold multipart form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _multipart: [],

    /**
     * Container to hold form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _form: [],

    /**
     * Request option container for details about the request.
     *
     * @type {Object}
     */
    options: {
      /**
       * Url obtained from request method arguments.
       *
       * @type {String}
       */
      url: uri,

      /**
       * Method obtained from request method arguments.
       *
       * @type {String}
       */
      method: method,

      /**
       * List of headers with case-sensitive fields.
       *
       * @type {Object}
       */
      headers: {}
    },

    hasHeader: function (name) {
      var headers
      var lowercaseHeaders

      name = name.toLowerCase()
      headers = Object.keys($this.options.headers)
      lowercaseHeaders = headers.map(function (header) {
        return header.toLowerCase()
      })

      for (var i = 0; i < lowercaseHeaders.length; i++) {
        if (lowercaseHeaders[i] === name) {
          return headers[i]
        }
      }

      return false
    },

    /**
     * Turn on multipart-form streaming
     *
     * @return {Object}
     */
    stream: function () {
      $this._stream = true
      return this
    },

    /**
     * Attaches a field to the multipart-form request, with pre-processing.
     *
     * @param  {String} name
     * @param  {String} value
     * @return {Object}
     */
    field: function (name, value, options) {
      return handleField(name, value, options)
    },

    /**
     * Attaches a file to the multipart-form request.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @return {Object}
     */
    attach: function (name, path, options) {
      options = options || {}
      options.attachment = true
      return handleField(name, path, options)
    },

    /**
     * Attaches field to the multipart-form request, with no pre-processing.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @param  {Object} options
     * @return {Object}
     */
    rawField: function (name, value, options) {
      $this._multipart.push({
        name: name,
        value: value,
        options: options,
        attachment: options.attachment || false
      })
    },

    /**
     * Basic Header Authentication Method
     *
     * Supports user being an Object to reflect Request
     * Supports user, password to reflect SuperAgent
     *
     * @param  {String|Object} user
     * @param  {String} password
     * @param  {Boolean} sendImmediately
     * @return {Object}
     */
    auth: function (user, password, sendImmediately) {
      $this.options.auth = (is(user).a(Object)) ? user : {
        user: user,
        password: password,
        sendImmediately: sendImmediately
      }

      return $this
    },

    /**
     * Sets header field to value
     *
     * @param  {String} field Header field
     * @param  {String} value Header field value
     * @return {Object}
     */
    header: function (field, value) {
      if (is(field).a(Object)) {
        for (var key in field) {
          if (field.hasOwnProperty(key)) {
            $this.header(key, field[key])
          }
        }

        return $this
      }

      var existingHeaderName = $this.hasHeader(field)
      $this.options.headers[existingHeaderName || field] = value

      return $this
    },

    /**
     * Serialize value as querystring representation, and append or set on 'Request.options.url'
     *
     * @param  {String|Object} value
     * @return {Object}
     */
    query: function (value) {
      if (is(value).a(Object)) value = Unirest.serializers.form(value)
      if (!value.length) return $this
      $this.options.url += (does($this.o ...
```
- example usage
```shell
...
'''

## Creating Requests

You're probably wondering how by using **Unirest** makes creating requests easier. Besides automatically supporting gzip, and parsing
 responses, lets start with a basic working example:

'''js
unirest.post('http://mockbin.com/request')
.headers({'Accept': 'application/json', 'Content-Type': 'application/json'})
.send({ "parameter": 23, "foo": "bar" })
.end(function (response) {
  console.log(response.body);
});
'''
...
```

#### <a name="apidoc.element.unirest.put"></a>[function <span class="apidocSignatureSpan">unirest.</span>put (uri, headers, body, callback)](#apidoc.element.unirest.put)
- description and source-code
```javascript
put = function (uri, headers, body, callback) {
  var $this = {
<span class="apidocCodeCommentSpan">    /**
     * Stream Multipart form-data request
     *
     * @type {Boolean}
     */
</span>    _stream: false,

    /**
     * Container to hold multipart form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _multipart: [],

    /**
     * Container to hold form data for processing upon request.
     *
     * @type {Array}
     * @private
     */
    _form: [],

    /**
     * Request option container for details about the request.
     *
     * @type {Object}
     */
    options: {
      /**
       * Url obtained from request method arguments.
       *
       * @type {String}
       */
      url: uri,

      /**
       * Method obtained from request method arguments.
       *
       * @type {String}
       */
      method: method,

      /**
       * List of headers with case-sensitive fields.
       *
       * @type {Object}
       */
      headers: {}
    },

    hasHeader: function (name) {
      var headers
      var lowercaseHeaders

      name = name.toLowerCase()
      headers = Object.keys($this.options.headers)
      lowercaseHeaders = headers.map(function (header) {
        return header.toLowerCase()
      })

      for (var i = 0; i < lowercaseHeaders.length; i++) {
        if (lowercaseHeaders[i] === name) {
          return headers[i]
        }
      }

      return false
    },

    /**
     * Turn on multipart-form streaming
     *
     * @return {Object}
     */
    stream: function () {
      $this._stream = true
      return this
    },

    /**
     * Attaches a field to the multipart-form request, with pre-processing.
     *
     * @param  {String} name
     * @param  {String} value
     * @return {Object}
     */
    field: function (name, value, options) {
      return handleField(name, value, options)
    },

    /**
     * Attaches a file to the multipart-form request.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @return {Object}
     */
    attach: function (name, path, options) {
      options = options || {}
      options.attachment = true
      return handleField(name, path, options)
    },

    /**
     * Attaches field to the multipart-form request, with no pre-processing.
     *
     * @param  {String} name
     * @param  {String|Object} path
     * @param  {Object} options
     * @return {Object}
     */
    rawField: function (name, value, options) {
      $this._multipart.push({
        name: name,
        value: value,
        options: options,
        attachment: options.attachment || false
      })
    },

    /**
     * Basic Header Authentication Method
     *
     * Supports user being an Object to reflect Request
     * Supports user, password to reflect SuperAgent
     *
     * @param  {String|Object} user
     * @param  {String} password
     * @param  {Boolean} sendImmediately
     * @return {Object}
     */
    auth: function (user, password, sendImmediately) {
      $this.options.auth = (is(user).a(Object)) ? user : {
        user: user,
        password: password,
        sendImmediately: sendImmediately
      }

      return $this
    },

    /**
     * Sets header field to value
     *
     * @param  {String} field Header field
     * @param  {String} value Header field value
     * @return {Object}
     */
    header: function (field, value) {
      if (is(field).a(Object)) {
        for (var key in field) {
          if (field.hasOwnProperty(key)) {
            $this.header(key, field[key])
          }
        }

        return $this
      }

      var existingHeaderName = $this.hasHeader(field)
      $this.options.headers[existingHeaderName || field] = value

      return $this
    },

    /**
     * Serialize value as querystring representation, and append or set on 'Request.options.url'
     *
     * @param  {String|Object} value
     * @return {Object}
     */
    query: function (value) {
      if (is(value).a(Object)) value = Unirest.serializers.form(value)
      if (!value.length) return $this
      $this.options.url += (does($this.o ...
```
- example usage
```shell
...
var Request = unirest.head('http://mockbin.com/request');
'''

### put
Returns a [Request](#request) object with the 'method' option set to 'PUT'

'''js
var Request = unirest.put('http://mockbin.com/request');
'''

### post
Returns a [Request](#request) object with the 'method' option set to 'POST'

'''js
var Request = unirest.post('http://mockbin.com/request');
...
```

#### <a name="apidoc.element.unirest.request"></a>[function <span class="apidocSignatureSpan">unirest.</span>request (uri, options, callback)](#apidoc.element.unirest.request)
- description and source-code
```javascript
function request(uri, options, callback) {
  if (typeof uri === 'undefined') {
    throw new Error('undefined is not a valid uri or options object.')
  }

  var params = initParams(uri, options, callback)

  if (params.method === 'HEAD' && paramsHaveRequestBody(params)) {
    throw new Error('HTTP HEAD requests MUST NOT include a request body.')
  }

  return new request.Request(params)
}
```
- example usage
```shell
...
.header('Accept', 'application/json')
.field({
  'parameter': 'value'
})
.attach({
  'file': 'dog.png',
  'relative file': fs.createReadStream(path.join(__dirname, 'dog.png')),
  'remote file': unirest.request('http://google.com/doodle.png')
})
.end(function (response) {
  console.log(response.body);
})
'''

**Arguments**
...
```

#### <a name="apidoc.element.unirest.request.Request"></a>[function <span class="apidocSignatureSpan">unirest.</span>request.Request (options)](#apidoc.element.unirest.request.Request)
- description and source-code
```javascript
function Request(options) {
  // if given the method property in options, set property explicitMethod to true

  // extend the Request instance with any non-reserved properties
  // remove any reserved functions from the options object
  // set Request instance to be readable and writable
  // call init

  var self = this

  // start with HAR, then override with additional options
  if (options.har) {
    self._har = new Har(self)
    options = self._har.options(options)
  }

  stream.Stream.call(self)
  var reserved = Object.keys(Request.prototype)
  var nonReserved = filterForNonReserved(reserved, options)

  extend(self, nonReserved)
  options = filterOutReservedFunctions(reserved, options)

  self.readable = true
  self.writable = true
  if (options.method) {
    self.explicitMethod = true
  }
  self._qs = new Querystring(self)
  self._auth = new Auth(self)
  self._oauth = new OAuth(self)
  self._multipart = new Multipart(self)
  self._redirect = new Redirect(self)
  self._tunnel = new Tunnel(self)
  self.init(options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.trim"></a>[function <span class="apidocSignatureSpan">unirest.</span>trim (s)](#apidoc.element.unirest.trim)
- description and source-code
```javascript
trim = function (s) { return s.trim() }
```
- example usage
```shell
...

// Cookie Sugar Method
result.cookie = function (name) {
  return result.cookies[name]
}

function setCookie (cookie) {
  var crumbs = Unirest.trim(cookie).split('=')
  var key = Unirest.trim(crumbs[0])
  var value = Unirest.trim(crumbs.slice(1).join('='))

  if (crumbs[0] && crumbs[0] !== '') {
    result.cookies[key] = value === '' ? true : value
  }
}
...
```

#### <a name="apidoc.element.unirest.type"></a>[function <span class="apidocSignatureSpan">unirest.</span>type (type, parse)](#apidoc.element.unirest.type)
- description and source-code
```javascript
type = function (type, parse) {
  if (typeof type !== 'string') return false
  return parse ? type.split(/ *; */).shift() : (Unirest.types[type] || type)
}
```
- example usage
```shell
...
'''

#### Request.send(Object | String)

Data marshalling for HTTP request body data

Determines whether data mime-type is 'form' or 'json'.
For irregular mime-types the '.type()' method is used to infer the 'content-type' header.

When mime-type is 'application/x-www-form-urlencoded' data is appended rather than overwritten.

**JSON**

'''js
unirest.post('http://mockbin.com/request')
...
```



# <a name="apidoc.module.unirest.Request"></a>[module unirest.Request](#apidoc.module.unirest.Request)

#### <a name="apidoc.element.unirest.Request.serialize"></a>[function <span class="apidocSignatureSpan">unirest.Request.</span>serialize (string, type)](#apidoc.element.unirest.Request.serialize)
- description and source-code
```javascript
serialize = function (string, type) {
  var serializer = Unirest.firstMatch(type, Unirest.enum.serialize)
  return serializer ? serializer(string) : string
}
```
- example usage
```shell
...
          $this.options.body[key] = data[key]
        }
      }
    } else {
      $this.options.body = data
    }
  } else {
    $this.options.body = Unirest.Request.serialize(data, type)
  }
} else if (is(data).a(String)) {
  if (!type) {
    $this.type('form')
    type = $this.options.headers[$this.hasHeader('content-type')]
  }
...
```

#### <a name="apidoc.element.unirest.Request.uid"></a>[function <span class="apidocSignatureSpan">unirest.Request.</span>uid (len)](#apidoc.element.unirest.Request.uid)
- description and source-code
```javascript
uid = function (len) {
  var output = ''
  var chars = 'abcdefghijklmnopqrstuvwxyz123456789'
  var nchars = chars.length
  while (len--) output += chars[Math.random() * nchars | 0]
  return output
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unirest.Response"></a>[module unirest.Response](#apidoc.module.unirest.Response)

#### <a name="apidoc.element.unirest.Response.parse"></a>[function <span class="apidocSignatureSpan">unirest.Response.</span>parse (string, type)](#apidoc.element.unirest.Response.parse)
- description and source-code
```javascript
parse = function (string, type) {
  var parser = Unirest.firstMatch(type, Unirest.enum.parse)
  return parser ? parser(string) : string
}
```
- example usage
```shell
...

The _options_ 'object' is where almost all of the request settings live. Each option method sugars to a field on this object to
allow for chaining and ease of use. If
you have trouble with an option method and wish to directly access the _options_ object
you are free to do so.

This object is modeled after the 'request' libraries options that are passed along through its constructor.

* 'url' ('String' | 'Object') - Url, or object parsed from 'url.parse()'
* 'qs' ('Object') - Object consisting of 'querystring' values to append to 'url' upon request.
* 'method' ('String') - Default 'GET'; HTTP Method.
* 'headers' ('Object') - Default '{}'; HTTP Headers.
* 'body' ('String' | 'Object') - Entity body for certain requests.
* 'form' ('Object') - Form data.
* 'auth' ('Object') - See 'Request.auth()' below.
* 'multipart' ('Object') - _Experimental_; See documentation below.
...
```

#### <a name="apidoc.element.unirest.Response.parseHeader"></a>[function <span class="apidocSignatureSpan">unirest.Response.</span>parseHeader (str)](#apidoc.element.unirest.Response.parseHeader)
- description and source-code
```javascript
parseHeader = function (str) {
  var lines = str.split(/\r?\n/)
  var fields = {}
  var index
  var line
  var field
  var val

  // Trailing CRLF
  lines.pop()

  for (var i = 0, len = lines.length; i < len; ++i) {
    line = lines[i]
    index = line.indexOf(':')
    field = line.slice(0, index).toLowerCase()
    val = Unirest.trim(line.slice(index + 1))
    fields[field] = val
  }

  return fields
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unirest.parsers"></a>[module unirest.parsers](#apidoc.module.unirest.parsers)

#### <a name="apidoc.element.unirest.parsers.json"></a>[function <span class="apidocSignatureSpan">unirest.parsers.</span>json (data)](#apidoc.element.unirest.parsers.json)
- description and source-code
```javascript
json = function (data) {
  try {
    data = JSON.parse(data)
  } catch (e) {}

  return data
}
```
- example usage
```shell
...

if (is(options).a(Object)) {
  if (options['content-type']) {
    var type = Unirest.type(options['content-type'], true)
    if (type) options.body = Unirest.Response.parse(options.body)
  } else {
    if (is(options.body).a(Object)) {
      options.body = Unirest.serializers.json(options.body)
    }
  }

  $this.options.multipart.push(options)
} else {
  $this.options.multipart.push({
    body: options
...
```

#### <a name="apidoc.element.unirest.parsers.string"></a>[function <span class="apidocSignatureSpan">unirest.parsers.</span>string (data)](#apidoc.element.unirest.parsers.string)
- description and source-code
```javascript
string = function (data) {
  var obj = {}
  var pairs = data.split('&')
  var parts
  var pair

  for (var i = 0, len = pairs.length; i < len; ++i) {
    pair = pairs[i]
    parts = pair.split('=')
    obj[decodeURIComponent(parts[0])] = decodeURIComponent(parts[1])
  }

  return obj
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unirest.request"></a>[module unirest.request](#apidoc.module.unirest.request)

#### <a name="apidoc.element.unirest.request.request"></a>[function <span class="apidocSignatureSpan">unirest.</span>request (uri, options, callback)](#apidoc.element.unirest.request.request)
- description and source-code
```javascript
function request(uri, options, callback) {
  if (typeof uri === 'undefined') {
    throw new Error('undefined is not a valid uri or options object.')
  }

  var params = initParams(uri, options, callback)

  if (params.method === 'HEAD' && paramsHaveRequestBody(params)) {
    throw new Error('HTTP HEAD requests MUST NOT include a request body.')
  }

  return new request.Request(params)
}
```
- example usage
```shell
...
.header('Accept', 'application/json')
.field({
  'parameter': 'value'
})
.attach({
  'file': 'dog.png',
  'relative file': fs.createReadStream(path.join(__dirname, 'dog.png')),
  'remote file': unirest.request('http://google.com/doodle.png')
})
.end(function (response) {
  console.log(response.body);
})
'''

**Arguments**
...
```

#### <a name="apidoc.element.unirest.request.Request"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>Request (options)](#apidoc.element.unirest.request.Request)
- description and source-code
```javascript
function Request(options) {
  // if given the method property in options, set property explicitMethod to true

  // extend the Request instance with any non-reserved properties
  // remove any reserved functions from the options object
  // set Request instance to be readable and writable
  // call init

  var self = this

  // start with HAR, then override with additional options
  if (options.har) {
    self._har = new Har(self)
    options = self._har.options(options)
  }

  stream.Stream.call(self)
  var reserved = Object.keys(Request.prototype)
  var nonReserved = filterForNonReserved(reserved, options)

  extend(self, nonReserved)
  options = filterOutReservedFunctions(reserved, options)

  self.readable = true
  self.writable = true
  if (options.method) {
    self.explicitMethod = true
  }
  self._qs = new Querystring(self)
  self._auth = new Auth(self)
  self._oauth = new OAuth(self)
  self._multipart = new Multipart(self)
  self._redirect = new Redirect(self)
  self._tunnel = new Tunnel(self)
  self.init(options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.cookie"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>cookie (str)](#apidoc.element.unirest.request.cookie)
- description and source-code
```javascript
cookie = function (str) {
  return cookies.parse(str)
}
```
- example usage
```shell
...

'''js
var CookieJar = unirest.jar();
CookieJar.add('key=value', '/'); // Cookie string, pathname / url
unirest.get('http://mockbin.com/request').jar(CookieJar);
'''

## unirest.cookie(String)

Creates a cookie, see above for example.

## unirest.request

'mikeal/request' library (the underlying layer of unirest) for direct use.
...
```

#### <a name="apidoc.element.unirest.request.defaults"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>defaults (options, requester)](#apidoc.element.unirest.request.defaults)
- description and source-code
```javascript
defaults = function (options, requester) {
  var self = this

  options = options || {}

  if (typeof options === 'function') {
    requester = options
    options = {}
  }

  var defaults      = wrapRequestMethod(self, options, requester)

  var verbs = ['get', 'head', 'post', 'put', 'patch', 'del', 'delete']
  verbs.forEach(function(verb) {
    defaults[verb]  = wrapRequestMethod(self[verb], options, requester, verb)
  })

  defaults.cookie   = wrapRequestMethod(self.cookie, options, requester)
  defaults.jar      = self.jar
  defaults.defaults = self.defaults
  return defaults
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.del"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>del (uri, options, callback)](#apidoc.element.unirest.request.del)
- description and source-code
```javascript
del = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.delete"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>delete (uri, options, callback)](#apidoc.element.unirest.request.delete)
- description and source-code
```javascript
delete = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...
var Request = unirest.patch('http://mockbin.com/request');
'''

### delete
Returns a [Request](#request) object with the 'method' option set to 'DELETE'

'''js
var Request = unirest.delete('http://mockbin.com/request');
'''

## unirest.jar()

Creates a container to store multiple cookies, i.e. a cookie jar.

'''js
...
```

#### <a name="apidoc.element.unirest.request.forever"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>forever (agentOptions, optionsArg)](#apidoc.element.unirest.request.forever)
- description and source-code
```javascript
forever = function (agentOptions, optionsArg) {
  var options = {}
  if (optionsArg) {
    extend(options, optionsArg)
  }
  if (agentOptions) {
    options.agentOptions = agentOptions
  }

  options.forever = true
  return request.defaults(options)
}
```
- example usage
```shell
...
* 'strictSSL' ('Boolean') - Default 'true'; See 'Request.strictSSL()' below.
* 'secureProtocol' ('String') - See 'Request.secureProtocol()' below.
* 'jar' ('Boolean' | 'Jar') - See 'Request.jar()' below.
* 'aws' ('Object') - See 'Request.aws()' below.
* 'httpSignature' ('Object') - See 'Request.httpSignature()' Below.
* 'localAddress' ('String') - See 'Request.localAddress()' Below.
* 'pool' ('Object') - See 'Request.pool()' Below.
* 'forever' ('Boolean') - Default 'undefined'; See 'Request.forever()' Below

## Request Option Methods

#### Request.url(String)

Sets 'url' location of the current request on 'Request.options' to the given 'String'
...
```

#### <a name="apidoc.element.unirest.request.get"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>get (uri, options, callback)](#apidoc.element.unirest.request.get)
- description and source-code
```javascript
get = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...
When no 'callback' is present, the [Request](#request) object will be returned.

### get

Returns a [Request](#request) object with the 'method' option set to 'GET'

'''js
var Request = unirest.get('http://mockbin.com/request');
'''

### head
Returns a [Request](#request) object with the 'method' option set to 'HEAD'

'''js
var Request = unirest.head('http://mockbin.com/request');
...
```

#### <a name="apidoc.element.unirest.request.head"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>head (uri, options, callback)](#apidoc.element.unirest.request.head)
- description and source-code
```javascript
head = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...
var Request = unirest.get('http://mockbin.com/request');
'''

### head
Returns a [Request](#request) object with the 'method' option set to 'HEAD'

'''js
var Request = unirest.head('http://mockbin.com/request');
'''

### put
Returns a [Request](#request) object with the 'method' option set to 'PUT'

'''js
var Request = unirest.put('http://mockbin.com/request');
...
```

#### <a name="apidoc.element.unirest.request.initParams"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>initParams (uri, options, callback)](#apidoc.element.unirest.request.initParams)
- description and source-code
```javascript
function initParams(uri, options, callback) {
  if (typeof options === 'function') {
    callback = options
  }

  var params = {}
  if (typeof options === 'object') {
    extend(params, options, {uri: uri})
  } else if (typeof uri === 'string') {
    extend(params, {uri: uri})
  } else {
    extend(params, uri)
  }

  params.callback = callback || params.callback
  return params
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.jar"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>jar (store)](#apidoc.element.unirest.request.jar)
- description and source-code
```javascript
jar = function (store) {
  return cookies.jar(store)
}
```
- example usage
```shell
...
### delete
Returns a [Request](#request) object with the 'method' option set to 'DELETE'

'''js
var Request = unirest.delete('http://mockbin.com/request');
'''

## unirest.jar()

Creates a container to store multiple cookies, i.e. a cookie jar.

'''js
var CookieJar = unirest.jar();
CookieJar.add('key=value', '/'); // Cookie string, pathname / url
unirest.get('http://mockbin.com/request').jar(CookieJar);
...
```

#### <a name="apidoc.element.unirest.request.patch"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>patch (uri, options, callback)](#apidoc.element.unirest.request.patch)
- description and source-code
```javascript
patch = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...
'''

### patch

Returns a [Request](#request) object with the 'method' option set to 'PATCH'

'''js
var Request = unirest.patch('http://mockbin.com/request');
'''

### delete
Returns a [Request](#request) object with the 'method' option set to 'DELETE'

'''js
var Request = unirest.delete('http://mockbin.com/request');
...
```

#### <a name="apidoc.element.unirest.request.post"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>post (uri, options, callback)](#apidoc.element.unirest.request.post)
- description and source-code
```javascript
post = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...
'''

## Creating Requests

You're probably wondering how by using **Unirest** makes creating requests easier. Besides automatically supporting gzip, and parsing
 responses, lets start with a basic working example:

'''js
unirest.post('http://mockbin.com/request')
.headers({'Accept': 'application/json', 'Content-Type': 'application/json'})
.send({ "parameter": 23, "foo": "bar" })
.end(function (response) {
  console.log(response.body);
});
'''
...
```

#### <a name="apidoc.element.unirest.request.put"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>put (uri, options, callback)](#apidoc.element.unirest.request.put)
- description and source-code
```javascript
put = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...
var Request = unirest.head('http://mockbin.com/request');
'''

### put
Returns a [Request](#request) object with the 'method' option set to 'PUT'

'''js
var Request = unirest.put('http://mockbin.com/request');
'''

### post
Returns a [Request](#request) object with the 'method' option set to 'POST'

'''js
var Request = unirest.post('http://mockbin.com/request');
...
```



# <a name="apidoc.module.unirest.request.Request"></a>[module unirest.request.Request](#apidoc.module.unirest.request.Request)

#### <a name="apidoc.element.unirest.request.Request.Request"></a>[function <span class="apidocSignatureSpan">unirest.request.</span>Request (options)](#apidoc.element.unirest.request.Request.Request)
- description and source-code
```javascript
function Request(options) {
  // if given the method property in options, set property explicitMethod to true

  // extend the Request instance with any non-reserved properties
  // remove any reserved functions from the options object
  // set Request instance to be readable and writable
  // call init

  var self = this

  // start with HAR, then override with additional options
  if (options.har) {
    self._har = new Har(self)
    options = self._har.options(options)
  }

  stream.Stream.call(self)
  var reserved = Object.keys(Request.prototype)
  var nonReserved = filterForNonReserved(reserved, options)

  extend(self, nonReserved)
  options = filterOutReservedFunctions(reserved, options)

  self.readable = true
  self.writable = true
  if (options.method) {
    self.explicitMethod = true
  }
  self._qs = new Querystring(self)
  self._auth = new Auth(self)
  self._oauth = new OAuth(self)
  self._multipart = new Multipart(self)
  self._redirect = new Redirect(self)
  self._tunnel = new Tunnel(self)
  self.init(options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.super_"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.</span>super_ ()](#apidoc.element.unirest.request.Request.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unirest.request.Request.prototype"></a>[module unirest.request.Request.prototype](#apidoc.module.unirest.request.Request.prototype)

#### <a name="apidoc.element.unirest.request.Request.prototype.abort"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>abort ()](#apidoc.element.unirest.request.Request.prototype.abort)
- description and source-code
```javascript
abort = function () {
  var self = this
  self._aborted = true

  if (self.req) {
    self.req.abort()
  }
  else if (self.response) {
    self.response.destroy()
  }

  self.emit('abort')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.auth"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>auth (user, pass, sendImmediately, bearer)](#apidoc.element.unirest.request.Request.prototype.auth)
- description and source-code
```javascript
auth = function (user, pass, sendImmediately, bearer) {
  var self = this

  self._auth.onRequest(user, pass, sendImmediately, bearer)

  return self
}
```
- example usage
```shell
...
});
'''

## Request Methods

Request Methods differ from Option Methods (See Below) in that these methods transform, or handle the data in a sugared way, where
 as Option Methods require a more _hands on_ approach.

#### Request.auth(Object) or (user, pass, sendImmediately)

Accepts either an 'Object' containing 'user', 'pass', and optionally 'sendImmediately'.

- 'user' ('String') - Authentication Username
- 'pass' ('String') - Authentication Password
- 'sendImmediately' ('String') - _Optional_; Defaults to 'true'; Flag to determine whether Request should send the basic authentication
 header along with the request. Upon being _false_, Request will retry with a _proper_ authentication header after receiving a '
401' response from the server (which must contain a 'WWW-Authenticate' header indicating the required authentication method)
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.aws"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>aws (opts, now)](#apidoc.element.unirest.request.Request.prototype.aws)
- description and source-code
```javascript
aws = function (opts, now) {
  var self = this

  if (!now) {
    self._aws = opts
    return self
  }

  if (opts.sign_version == 4 || opts.sign_version == '4') {
    // use aws4
    var options = {
      host: self.uri.host,
      path: self.uri.path,
      method: self.method,
      headers: {
        'content-type': self.getHeader('content-type') || ''
      },
      body: self.body
    }
    var signRes = aws4.sign(options, {
      accessKeyId: opts.key,
      secretAccessKey: opts.secret
    })
    self.setHeader('authorization', signRes.headers.Authorization)
    self.setHeader('x-amz-date', signRes.headers['X-Amz-Date'])
  }
  else {
    // default: use aws-sign2
    var date = new Date()
    self.setHeader('date', date.toUTCString())
    var auth =
      { key: opts.key
      , secret: opts.secret
      , verb: self.method.toUpperCase()
      , date: date
      , contentType: self.getHeader('content-type') || ''
      , md5: self.getHeader('content-md5') || ''
      , amazonHeaders: aws2.canonicalizeHeaders(self.headers)
      }
    var path = self.uri.path
    if (opts.bucket && path) {
      auth.resource = '/' + opts.bucket + path
    } else if (opts.bucket && !path) {
      auth.resource = '/' + opts.bucket
    } else if (!opts.bucket && path) {
      auth.resource = path
    } else if (!opts.bucket && !path) {
      auth.resource = '/'
    }
    auth.resource = aws2.canonicalizeResource(auth.resource)
    self.setHeader('authorization', aws2.authorization(auth))
  }

  return self
}
```
- example usage
```shell
...
* 'timeout' ('Number') - Number of milliseconds to wait before aborting.
* 'proxy' ('String') - See 'Request.proxy()' below.
* 'oauth' ('Object') - See 'Request.oauth()' below.
* 'hawk' ('Object') - See 'Request.hawk()' below
* 'strictSSL' ('Boolean') - Default 'true'; See 'Request.strictSSL()' below.
* 'secureProtocol' ('String') - See 'Request.secureProtocol()' below.
* 'jar' ('Boolean' | 'Jar') - See 'Request.jar()' below.
* 'aws' ('Object') - See 'Request.aws()' below.
* 'httpSignature' ('Object') - See 'Request.httpSignature()' Below.
* 'localAddress' ('String') - See 'Request.localAddress()' Below.
* 'pool' ('Object') - See 'Request.pool()' Below.
* 'forever' ('Boolean') - Default 'undefined'; See 'Request.forever()' Below

## Request Option Methods
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.debug"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>debug ()](#apidoc.element.unirest.request.Request.prototype.debug)
- description and source-code
```javascript
function debug() {
  if (Request.debug) {
    console.error('REQUEST %s', util.format.apply(util, arguments))
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.destroy"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>destroy ()](#apidoc.element.unirest.request.Request.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  var self = this
  if (!self._ended) {
    self.end()
  } else if (self.response) {
    self.response.destroy()
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.enableUnixSocket"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>enableUnixSocket ()](#apidoc.element.unirest.request.Request.prototype.enableUnixSocket)
- description and source-code
```javascript
enableUnixSocket = function () {
  // Get the socket & request paths from the URL
  var unixParts = this.uri.path.split(':')
    , host = unixParts[0]
    , path = unixParts[1]
  // Apply unix properties to request
  this.socketPath = host
  this.uri.pathname = path
  this.uri.path = path
  this.uri.host = host
  this.uri.hostname = host
  this.uri.isUnix = true
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.end"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>end (chunk)](#apidoc.element.unirest.request.Request.prototype.end)
- description and source-code
```javascript
end = function (chunk) {
  var self = this
  if (self._aborted) {return}

  if (chunk) {
    self.write(chunk)
  }
  if (!self._started) {
    self.start()
  }
  if (self.req) {
    self.req.end()
  }
}
```
- example usage
```shell
...

You're probably wondering how by using **Unirest** makes creating requests easier. Besides automatically supporting gzip, and parsing
 responses, lets start with a basic working example:

'''js
unirest.post('http://mockbin.com/request')
.headers({'Accept': 'application/json', 'Content-Type': 'application/json'})
.send({ "parameter": 23, "foo": "bar" })
.end(function (response) {
  console.log(response.body);
});
'''

## Uploading Files

Transferring file data has been simplified:
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.form"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>form (form)](#apidoc.element.unirest.request.Request.prototype.form)
- description and source-code
```javascript
form = function (form) {
  var self = this
  if (form) {
    if (!/^application\/x-www-form-urlencoded\b/.test(self.getHeader('content-type'))) {
      self.setHeader('content-type', 'application/x-www-form-urlencoded')
    }
    self.body = (typeof form === 'string')
      ? self._qs.rfc3986(form.toString('utf8'))
      : self._qs.stringify(form).toString('utf8')
    return self
  }
  // create form-data object
  self._form = new FormData()
  self._form.on('error', function(err) {
    err.message = 'form-data: ' + err.message
    self.emit('error', err)
    self.abort()
  })
  return self._form
}
```
- example usage
```shell
...

Sets 'method' value on 'Request.options' to the given value.

'''js
Request.method('HEAD');
'''

#### Request.form(Object)

Sets 'form' object on 'Request.options' to the given object.

When used 'body' is set to the object passed as a 'querystring' representation and the 'Content-Type' header to 'application/x-www
-form-urlencoded; charset=utf-8'

'''js
Request.form({
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.getHeader"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>getHeader (name, headers)](#apidoc.element.unirest.request.Request.prototype.getHeader)
- description and source-code
```javascript
getHeader = function (name, headers) {
  var self = this
  var result, re, match
  if (!headers) {
    headers = self.headers
  }
  Object.keys(headers).forEach(function (key) {
    if (key.length !== name.length) {
      return
    }
    re = new RegExp(name, 'i')
    match = key.match(re)
    if (match) {
      result = headers[key]
    }
  })
  return result
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.getNewAgent"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>getNewAgent ()](#apidoc.element.unirest.request.Request.prototype.getNewAgent)
- description and source-code
```javascript
getNewAgent = function () {
  var self = this
  var Agent = self.agentClass
  var options = {}
  if (self.agentOptions) {
    for (var i in self.agentOptions) {
      options[i] = self.agentOptions[i]
    }
  }
  if (self.ca) {
    options.ca = self.ca
  }
  if (self.ciphers) {
    options.ciphers = self.ciphers
  }
  if (self.secureProtocol) {
    options.secureProtocol = self.secureProtocol
  }
  if (self.secureOptions) {
    options.secureOptions = self.secureOptions
  }
  if (typeof self.rejectUnauthorized !== 'undefined') {
    options.rejectUnauthorized = self.rejectUnauthorized
  }

  if (self.cert && self.key) {
    options.key = self.key
    options.cert = self.cert
  }

  if (self.pfx) {
    options.pfx = self.pfx
  }

  if (self.passphrase) {
    options.passphrase = self.passphrase
  }

  var poolKey = ''

  // different types of agents are in different pools
  if (Agent !== self.httpModule.Agent) {
    poolKey += Agent.name
  }

  // ca option is only relevant if proxy or destination are https
  var proxy = self.proxy
  if (typeof proxy === 'string') {
    proxy = url.parse(proxy)
  }
  var isHttps = (proxy && proxy.protocol === 'https:') || this.uri.protocol === 'https:'

  if (isHttps) {
    if (options.ca) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.ca
    }

    if (typeof options.rejectUnauthorized !== 'undefined') {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.rejectUnauthorized
    }

    if (options.cert) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.cert.toString('ascii') + options.key.toString('ascii')
    }

    if (options.pfx) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.pfx.toString('ascii')
    }

    if (options.ciphers) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.ciphers
    }

    if (options.secureProtocol) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.secureProtocol
    }

    if (options.secureOptions) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.secureOptions
    }
  }

  if (self.pool === globalPool && !poolKey && Object.keys(options).length === 0 && self.httpModule.globalAgent) {
    // not doing anything special.  Use the globalAgent
    return self.httpModule.globalAgent
  }

  // we're using a stored agent.  Make sure it's protocol-specific
  poolKey = self.uri.protocol + poolKey

  // generate a new agent for this setting if none yet exists
  if (!self.pool[poolKey]) {
    self.pool[poolKey] = new Agent(options)
    // properly set maxSockets on new agents
    if (self.pool.maxSockets) {
      self.pool[poolKey].maxSockets = self.pool.maxSockets
    }
  }

  return self.pool[poolKey]
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.hawk"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>hawk (opts)](#apidoc.element.unirest.request.Request.prototype.hawk)
- description and source-code
```javascript
hawk = function (opts) {
  var self = this
  self.setHeader('Authorization', hawk.client.header(self.uri, self.method, opts).field)
}
```
- example usage
```shell
...
* 'followRedirect' ('Boolean') - Default 'true'; Follow HTTP '3xx' responses as redirects.
* 'followAllRedirects' ('Boolean') - Default 'false'; Follow **Non**-GET HTTP '3xx' responses as redirects.
* 'maxRedirects' ('Number') - Default '10'; Maximum number of redirects before aborting.
* 'encoding' ('String') - Encoding to be used on 'setEncoding' of response data.
* 'timeout' ('Number') - Number of milliseconds to wait before aborting.
* 'proxy' ('String') - See 'Request.proxy()' below.
* 'oauth' ('Object') - See 'Request.oauth()' below.
* 'hawk' ('Object') - See 'Request.hawk()' below
* 'strictSSL' ('Boolean') - Default 'true'; See 'Request.strictSSL()' below.
* 'secureProtocol' ('String') - See 'Request.secureProtocol()' below.
* 'jar' ('Boolean' | 'Jar') - See 'Request.jar()' below.
* 'aws' ('Object') - See 'Request.aws()' below.
* 'httpSignature' ('Object') - See 'Request.httpSignature()' Below.
* 'localAddress' ('String') - See 'Request.localAddress()' Below.
* 'pool' ('Object') - See 'Request.pool()' Below.
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.httpSignature"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>httpSignature (opts)](#apidoc.element.unirest.request.Request.prototype.httpSignature)
- description and source-code
```javascript
httpSignature = function (opts) {
  var self = this
  httpSignature.signRequest({
    getHeader: function(header) {
      return self.getHeader(header, self.headers)
    },
    setHeader: function(header, value) {
      self.setHeader(header, value)
    },
    method: self.method,
    path: self.path
  }, opts)
  debug('httpSignature authorization', self.getHeader('authorization'))

  return self
}
```
- example usage
```shell
...
* 'proxy' ('String') - See 'Request.proxy()' below.
* 'oauth' ('Object') - See 'Request.oauth()' below.
* 'hawk' ('Object') - See 'Request.hawk()' below
* 'strictSSL' ('Boolean') - Default 'true'; See 'Request.strictSSL()' below.
* 'secureProtocol' ('String') - See 'Request.secureProtocol()' below.
* 'jar' ('Boolean' | 'Jar') - See 'Request.jar()' below.
* 'aws' ('Object') - See 'Request.aws()' below.
* 'httpSignature' ('Object') - See 'Request.httpSignature()' Below.
* 'localAddress' ('String') - See 'Request.localAddress()' Below.
* 'pool' ('Object') - See 'Request.pool()' Below.
* 'forever' ('Boolean') - Default 'undefined'; See 'Request.forever()' Below

## Request Option Methods

#### Request.url(String)
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.init"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>init (options)](#apidoc.element.unirest.request.Request.prototype.init)
- description and source-code
```javascript
init = function (options) {
  // init() contains all the code to setup the request object.
  // the actual outgoing request is not started until start() is called
  // this function is called from both the constructor and on redirect.
  var self = this
  if (!options) {
    options = {}
  }
  self.headers = self.headers ? copy(self.headers) : {}

  // Delete headers with value undefined since they break
  // ClientRequest.OutgoingMessage.setHeader in node 0.12
  for (var headerName in self.headers) {
    if (typeof self.headers[headerName] === 'undefined') {
      delete self.headers[headerName]
    }
  }

  caseless.httpify(self, self.headers)

  if (!self.method) {
    self.method = options.method || 'GET'
  }
  if (!self.localAddress) {
    self.localAddress = options.localAddress
  }

  self._qs.init(options)

  debug(options)
  if (!self.pool && self.pool !== false) {
    self.pool = globalPool
  }
  self.dests = self.dests || []
  self.__isRequestRequest = true

  // Protect against double callback
  if (!self._callback && self.callback) {
    self._callback = self.callback
    self.callback = function () {
      if (self._callbackCalled) {
        return // Print a warning maybe?
      }
      self._callbackCalled = true
      self._callback.apply(self, arguments)
    }
    self.on('error', self.callback.bind())
    self.on('complete', self.callback.bind(self, null))
  }

  // People use this property instead all the time, so support it
  if (!self.uri && self.url) {
    self.uri = self.url
    delete self.url
  }

  // If there's a baseUrl, then use it as the base URL (i.e. uri must be
  // specified as a relative path and is appended to baseUrl).
  if (self.baseUrl) {
    if (typeof self.baseUrl !== 'string') {
      return self.emit('error', new Error('options.baseUrl must be a string'))
    }

    if (typeof self.uri !== 'string') {
      return self.emit('error', new Error('options.uri must be a string when using options.baseUrl'))
    }

    if (self.uri.indexOf('//') === 0 || self.uri.indexOf('://') !== -1) {
      return self.emit('error', new Error('options.uri must be a path when using options.baseUrl'))
    }

    // Handle all cases to make sure that there's only one slash between
    // baseUrl and uri.
    var baseUrlEndsWithSlash = self.baseUrl.lastIndexOf('/') === self.baseUrl.length - 1
    var uriStartsWithSlash = self.uri.indexOf('/') === 0

    if (baseUrlEndsWithSlash && uriStartsWithSlash) {
      self.uri = self.baseUrl + self.uri.slice(1)
    } else if (baseUrlEndsWithSlash || uriStartsWithSlash) {
      self.uri = self.baseUrl + self.uri
    } else if (self.uri === '') {
      self.uri = self.baseUrl
    } else {
      self.uri = self.baseUrl + '/' + self.uri
    }
    delete self.baseUrl
  }

  // A URI is needed by this point, emit error if we haven't been able to get one
  if (!self.uri) {
    return self.emit('error', new Error('options.uri is a required argument'))
  }

  // If a string URI/URL was given, parse it into a URL object
  if (typeof self.uri === 'string') {
    self.uri = url.parse(self.uri)
  }

  // Some URL objects are not from a URL parsed string and need href added
  if (!self.uri.href) {
    self.uri.href = url.format(self.uri)
  }

  // DEPRECATED: Warning for users of the old Unix Sockets URL Scheme
  if (self.uri.protocol === 'unix:') {
    return self.emit('error', new Error(''unix://' URL scheme is no longer supported. Please use the format 'http://unix:SOCKET:
PATH''))
  }

  // Support Unix Sockets
  if (self.uri.host === 'unix') {
    self.enableUnixSocket()
  }

  if (self.strictSSL === false) {
    self.rejectUnauthorized = false
  }

  if (!self.uri.pathname) {self.uri.pathname = '/'}

  if (!(self.uri.host || (self.uri.hostname && self.uri.port)) && !self.uri.isUnix) {
    // Invalid URI: it may generate lot of bad errors, like 'TypeError: Cannot call method 'indexOf' of undefined' in CookieJar
    // Detect and reject it as soon as possible
    var faultyUri = url.format(self.uri)
    var message = 'Invalid URI "' + faultyUri + '"'
    if (Object.keys(options). ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.jar"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>jar (jar)](#apidoc.element.unirest.request.Request.prototype.jar)
- description and source-code
```javascript
jar = function (jar) {
  var self = this
  var cookies

  if (self._redirect.redirectsFollowed === 0) {
    self.originalCookieHeader = self.getHeader('cookie')
  }

  if (!jar) {
    // disable cookies
    cookies = false
    self._disableCookies = true
  } else {
    var targetCookieJar = (jar && jar.getCookieString) ? jar : globalCookieJar
    var urihref = self.uri.href
    //fetch cookie in the Specified host
    if (targetCookieJar) {
      cookies = targetCookieJar.getCookieString(urihref)
    }
  }

  //if need cookie and cookie is not empty
  if (cookies && cookies.length) {
    if (self.originalCookieHeader) {
      // Don't overwrite existing Cookie header
      self.setHeader('cookie', self.originalCookieHeader + '; ' + cookies)
    } else {
      self.setHeader('cookie', cookies)
    }
  }
  self._jar = jar
  return self
}
```
- example usage
```shell
...
### delete
Returns a [Request](#request) object with the 'method' option set to 'DELETE'

'''js
var Request = unirest.delete('http://mockbin.com/request');
'''

## unirest.jar()

Creates a container to store multiple cookies, i.e. a cookie jar.

'''js
var CookieJar = unirest.jar();
CookieJar.add('key=value', '/'); // Cookie string, pathname / url
unirest.get('http://mockbin.com/request').jar(CookieJar);
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.json"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>json (val)](#apidoc.element.unirest.request.Request.prototype.json)
- description and source-code
```javascript
json = function (val) {
  var self = this

  if (!self.hasHeader('accept')) {
    self.setHeader('accept', 'application/json')
  }

  if (typeof self.jsonReplacer === 'function') {
    self._jsonReplacer = self.jsonReplacer
  }

  self._json = true
  if (typeof val === 'boolean') {
    if (self.body !== undefined) {
      if (!/^application\/x-www-form-urlencoded\b/.test(self.getHeader('content-type'))) {
        self.body = safeStringify(self.body, self._jsonReplacer)
      } else {
        self.body = self._qs.rfc3986(self.body)
      }
      if (!self.hasHeader('content-type')) {
        self.setHeader('content-type', 'application/json')
      }
    }
  } else {
    self.body = safeStringify(val, self._jsonReplacer)
    if (!self.hasHeader('content-type')) {
      self.setHeader('content-type', 'application/json')
    }
  }

  if (typeof self.jsonReviver === 'function') {
    self._jsonReviver = self.jsonReviver
  }

  return self
}
```
- example usage
```shell
...

if (is(options).a(Object)) {
  if (options['content-type']) {
    var type = Unirest.type(options['content-type'], true)
    if (type) options.body = Unirest.Response.parse(options.body)
  } else {
    if (is(options.body).a(Object)) {
      options.body = Unirest.serializers.json(options.body)
    }
  }

  $this.options.multipart.push(options)
} else {
  $this.options.multipart.push({
    body: options
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.multipart"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>multipart (multipart)](#apidoc.element.unirest.request.Request.prototype.multipart)
- description and source-code
```javascript
multipart = function (multipart) {
  var self = this

  self._multipart.onRequest(multipart)

  if (!self._multipart.chunked) {
    self.body = self._multipart.body
  }

  return self
}
```
- example usage
```shell
...
Request.header('Accept', 'application/json');
'''

#### Request.part(Object)

**Experimental**

Similiar to 'Request.multipart()' except it only allows one object to be passed at a time and does the pre-processing on necessary
 'body' values for you.

Each object is then appended to the 'Request.options.multipart' array.

'''js
Request.part({
'content-type': 'application/json',
body: { foo: 'bar' }
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.oauth"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>oauth (_oauth)](#apidoc.element.unirest.request.Request.prototype.oauth)
- description and source-code
```javascript
oauth = function (_oauth) {
  var self = this

  self._oauth.onRequest(_oauth)

  return self
}
```
- example usage
```shell
...
* 'multipart' ('Object') - _Experimental_; See documentation below.
* 'followRedirect' ('Boolean') - Default 'true'; Follow HTTP '3xx' responses as redirects.
* 'followAllRedirects' ('Boolean') - Default 'false'; Follow **Non**-GET HTTP '3xx' responses as redirects.
* 'maxRedirects' ('Number') - Default '10'; Maximum number of redirects before aborting.
* 'encoding' ('String') - Encoding to be used on 'setEncoding' of response data.
* 'timeout' ('Number') - Number of milliseconds to wait before aborting.
* 'proxy' ('String') - See 'Request.proxy()' below.
* 'oauth' ('Object') - See 'Request.oauth()' below.
* 'hawk' ('Object') - See 'Request.hawk()' below
* 'strictSSL' ('Boolean') - Default 'true'; See 'Request.strictSSL()' below.
* 'secureProtocol' ('String') - See 'Request.secureProtocol()' below.
* 'jar' ('Boolean' | 'Jar') - See 'Request.jar()' below.
* 'aws' ('Object') - See 'Request.aws()' below.
* 'httpSignature' ('Object') - See 'Request.httpSignature()' Below.
* 'localAddress' ('String') - See 'Request.localAddress()' Below.
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.onRequestError"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>onRequestError (error)](#apidoc.element.unirest.request.Request.prototype.onRequestError)
- description and source-code
```javascript
onRequestError = function (error) {
  var self = this
  if (self._aborted) {
    return
  }
  if (self.req && self.req._reusedSocket && error.code === 'ECONNRESET'
      && self.agent.addRequestNoreuse) {
    self.agent = { addRequest: self.agent.addRequestNoreuse.bind(self.agent) }
    self.start()
    self.req.end()
    return
  }
  if (self.timeout && self.timeoutTimer) {
    clearTimeout(self.timeoutTimer)
    self.timeoutTimer = null
  }
  self.emit('error', error)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.onRequestResponse"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>onRequestResponse (response)](#apidoc.element.unirest.request.Request.prototype.onRequestResponse)
- description and source-code
```javascript
onRequestResponse = function (response) {
  var self = this
  debug('onRequestResponse', self.uri.href, response.statusCode, response.headers)
  response.on('end', function() {
    if (self.timing) {
      self.elapsedTime += (new Date().getTime() - self.startTime)
      debug('elapsed time', self.elapsedTime)
      response.elapsedTime = self.elapsedTime
    }
    debug('response end', self.uri.href, response.statusCode, response.headers)
  })

  if (self._aborted) {
    debug('aborted', self.uri.href)
    response.resume()
    return
  }

  self.response = response
  response.request = self
  response.toJSON = responseToJSON

  // XXX This is different on 0.10, because SSL is strict by default
  if (self.httpModule === https &&
      self.strictSSL && (!response.hasOwnProperty('socket') ||
      !response.socket.authorized)) {
    debug('strict ssl error', self.uri.href)
    var sslErr = response.hasOwnProperty('socket') ? response.socket.authorizationError : self.uri.href + ' does not support SSL
'
    self.emit('error', new Error('SSL Error: ' + sslErr))
    return
  }

  // Save the original host before any redirect (if it changes, we need to
  // remove any authorization headers).  Also remember the case of the header
  // name because lots of broken servers expect Host instead of host and we
  // want the caller to be able to specify this.
  self.originalHost = self.getHeader('host')
  if (!self.originalHostHeaderName) {
    self.originalHostHeaderName = self.hasHeader('host')
  }
  if (self.setHost) {
    self.removeHeader('host')
  }
  if (self.timeout && self.timeoutTimer) {
    clearTimeout(self.timeoutTimer)
    self.timeoutTimer = null
  }

  var targetCookieJar = (self._jar && self._jar.setCookie) ? self._jar : globalCookieJar
  var addCookie = function (cookie) {
    //set the cookie if it's domain in the href's domain.
    try {
      targetCookieJar.setCookie(cookie, self.uri.href, {ignoreError: true})
    } catch (e) {
      self.emit('error', e)
    }
  }

  response.caseless = caseless(response.headers)

  if (response.caseless.has('set-cookie') && (!self._disableCookies)) {
    var headerName = response.caseless.has('set-cookie')
    if (Array.isArray(response.headers[headerName])) {
      response.headers[headerName].forEach(addCookie)
    } else {
      addCookie(response.headers[headerName])
    }
  }

  if (self._redirect.onResponse(response)) {
    return // Ignore the rest of the response
  } else {
    // Be a good stream and emit end when the response is finished.
    // Hack to emit end on close because of a core bug that never fires end
    response.on('close', function () {
      if (!self._ended) {
        self.response.emit('end')
      }
    })

    response.on('end', function () {
      self._ended = true
    })

    var noBody = function (code) {
      return (
        self.method === 'HEAD'
        // Informational
        || (code >= 100 && code < 200)
        // No Content
        || code === 204
        // Not Modified
        || code === 304
      )
    }

    var responseContent
    if (self.gzip && !noBody(response.statusCode)) {
      var contentEncoding = response.headers['content-encoding'] || 'identity'
      contentEncoding = contentEncoding.trim().toLowerCase()

      if (contentEncoding === 'gzip') {
        responseContent = zlib.createGunzip()
        response.pipe(responseContent)
      } else if (contentEncoding === 'deflate') {
        responseContent = zlib.createInflate()
        response.pipe(responseContent)
      } else {
        // Since previous versions didn't check for Content-Encoding header,
        // ignore any invalid values to preserve backwards-compatibility
        if (contentEncoding !== 'identity') {
          debug('ignoring unrecognized Content-Encoding ' + contentEncoding)
        }
        responseContent = response
      }
    } else {
      responseContent = response
    }

    if (self.encoding) {
      if (self.dests.length !== 0) {
        console.error('Ignoring encoding parameter as this stream is being piped to another stream which makes the encoding opti ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.pause"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>pause ()](#apidoc.element.unirest.request.Request.prototype.pause)
- description and source-code
```javascript
pause = function () {
  var self = this
  if (!self.responseContent) {
    self._paused = true
  } else {
    self.responseContent.pause.apply(self.responseContent, arguments)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.pipe"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>pipe (dest, opts)](#apidoc.element.unirest.request.Request.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest, opts) {
  var self = this

  if (self.response) {
    if (self._destdata) {
      self.emit('error', new Error('You cannot pipe after data has been emitted from the response.'))
    } else if (self._ended) {
      self.emit('error', new Error('You cannot pipe after the response has been ended.'))
    } else {
      stream.Stream.prototype.pipe.call(self, dest, opts)
      self.pipeDest(dest)
      return dest
    }
  } else {
    self.dests.push(dest)
    stream.Stream.prototype.pipe.call(self, dest, opts)
    return dest
  }
}
```
- example usage
```shell
...
    return
  }

  stream.emit('error', error)
})

// Start the processing
response.pipe(unzip)

// Ensure encoding is captured
response.setEncoding = function (type) {
  decoder = new StringDecoder(type)
}

// Capture decompression and decode with captured encoding
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.pipeDest"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>pipeDest (dest)](#apidoc.element.unirest.request.Request.prototype.pipeDest)
- description and source-code
```javascript
pipeDest = function (dest) {
  var self = this
  var response = self.response
  // Called after the response is received
  if (dest.headers && !dest.headersSent) {
    if (response.caseless.has('content-type')) {
      var ctname = response.caseless.has('content-type')
      if (dest.setHeader) {
        dest.setHeader(ctname, response.headers[ctname])
      }
      else {
        dest.headers[ctname] = response.headers[ctname]
      }
    }

    if (response.caseless.has('content-length')) {
      var clname = response.caseless.has('content-length')
      if (dest.setHeader) {
        dest.setHeader(clname, response.headers[clname])
      } else {
        dest.headers[clname] = response.headers[clname]
      }
    }
  }
  if (dest.setHeader && !dest.headersSent) {
    for (var i in response.headers) {
      // If the response content is being decoded, the Content-Encoding header
      // of the response doesn't represent the piped content, so don't pass it.
      if (!self.gzip || i !== 'content-encoding') {
        dest.setHeader(i, response.headers[i])
      }
    }
    dest.statusCode = response.statusCode
  }
  if (self.pipefilter) {
    self.pipefilter(response, dest)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.qs"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>qs (q, clobber)](#apidoc.element.unirest.request.Request.prototype.qs)
- description and source-code
```javascript
qs = function (q, clobber) {
  var self = this
  var base
  if (!clobber && self.uri.query) {
    base = self._qs.parse(self.uri.query)
  } else {
    base = {}
  }

  for (var i in q) {
    base[i] = q[i]
  }

  var qs = self._qs.stringify(base)

  if (qs === '') {
    return self
  }

  self.uri = url.parse(self.uri.href.split('?')[0] + '?' + qs)
  self.url = self.uri
  self.path = self.uri.path

  if (self.uri.host === 'unix') {
    self.enableUnixSocket()
  }

  return self
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.readResponseBody"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>readResponseBody (response)](#apidoc.element.unirest.request.Request.prototype.readResponseBody)
- description and source-code
```javascript
readResponseBody = function (response) {
  var self = this
  debug('reading response\'s body')
  var buffer = bl()
    , strings = []

  self.on('data', function (chunk) {
    if (Buffer.isBuffer(chunk)) {
      buffer.append(chunk)
    } else {
      strings.push(chunk)
    }
  })
  self.on('end', function () {
    debug('end event', self.uri.href)
    if (self._aborted) {
      debug('aborted', self.uri.href)
      // 'buffer' is defined in the parent scope and used in a closure it exists for the life of the request.
      // This can lead to leaky behavior if the user retains a reference to the request object.
      buffer.destroy()
      return
    }

    if (buffer.length) {
      debug('has body', self.uri.href, buffer.length)
      if (self.encoding === null) {
        // response.body = buffer
        // can't move to this until https://github.com/rvagg/bl/issues/13
        response.body = buffer.slice()
      } else {
        response.body = buffer.toString(self.encoding)
      }
      // 'buffer' is defined in the parent scope and used in a closure it exists for the life of the Request.
      // This can lead to leaky behavior if the user retains a reference to the request object.
      buffer.destroy()
    } else if (strings.length) {
      // The UTF8 BOM [0xEF,0xBB,0xBF] is converted to [0xFE,0xFF] in the JS UTC16/UCS2 representation.
      // Strip this value out when the encoding is set to 'utf8', as upstream consumers won't expect it and it breaks JSON.parse
().
      if (self.encoding === 'utf8' && strings[0].length > 0 && strings[0][0] === '\uFEFF') {
        strings[0] = strings[0].substring(1)
      }
      response.body = strings.join('')
    }

    if (self._json) {
      try {
        response.body = JSON.parse(response.body, self._jsonReviver)
      } catch (e) {
        debug('invalid JSON received', self.uri.href)
      }
    }
    debug('emitting complete', self.uri.href)
    if (typeof response.body === 'undefined' && !self._json) {
      response.body = self.encoding === null ? new Buffer(0) : ''
    }
    self.emit('complete', response, response.body)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.resume"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>resume ()](#apidoc.element.unirest.request.Request.prototype.resume)
- description and source-code
```javascript
resume = function () {
  var self = this
  if (!self.responseContent) {
    self._paused = false
  } else {
    self.responseContent.resume.apply(self.responseContent, arguments)
  }
}
```
- example usage
```shell
...
}

if (!response.body) {
  response.body = ''
}

// Node 10+
response.resume()

// GZIP, Feel me?
handleGZIPResponse(response)

// Fallback
response.on('data', function (chunk) {
  if (typeof chunk === 'string') response.body += chunk
...
```

#### <a name="apidoc.element.unirest.request.Request.prototype.start"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>start ()](#apidoc.element.unirest.request.Request.prototype.start)
- description and source-code
```javascript
start = function () {
  // start() is called once we are ready to send the outgoing HTTP request.
  // this is usually called on the first write(), end() or on nextTick()
  var self = this

  if (self._aborted) {
    return
  }

  self._started = true
  self.method = self.method || 'GET'
  self.href = self.uri.href

  if (self.src && self.src.stat && self.src.stat.size && !self.hasHeader('content-length')) {
    self.setHeader('content-length', self.src.stat.size)
  }
  if (self._aws) {
    self.aws(self._aws, true)
  }

  // We have a method named auth, which is completely different from the http.request
  // auth option.  If we don't remove it, we're gonna have a bad time.
  var reqOptions = copy(self)
  delete reqOptions.auth

  debug('make request', self.uri.href)

  try {
    self.req = self.httpModule.request(reqOptions)
  } catch (err) {
    self.emit('error', err)
    return
  }

  if (self.timing) {
    self.startTime = new Date().getTime()
  }

  if (self.timeout && !self.timeoutTimer) {
    var timeout = self.timeout < 0 ? 0 : self.timeout
    // Set a timeout in memory - this block will throw if the server takes more
    // than 'timeout' to write the HTTP status and headers (corresponding to
    // the on('response') event on the client). NB: this measures wall-clock
    // time, not the time between bytes sent by the server.
    self.timeoutTimer = setTimeout(function () {
      var connectTimeout = self.req.socket && self.req.socket.readable === false
      self.abort()
      var e = new Error('ETIMEDOUT')
      e.code = 'ETIMEDOUT'
      e.connect = connectTimeout
      self.emit('error', e)
    }, timeout)

    if (self.req.setTimeout) { // only works on node 0.6+
      // Set an additional timeout on the socket, via the 'setsockopt' syscall.
      // This timeout sets the amount of time to wait *between* bytes sent
      // from the server, and may or may not correspond to the wall-clock time
      // elapsed from the start of the request.
      //
      // In particular, it's useful for erroring if the server fails to send
      // data halfway through streaming a response.
      self.req.setTimeout(timeout, function () {
        if (self.req) {
          self.req.abort()
          var e = new Error('ESOCKETTIMEDOUT')
          e.code = 'ESOCKETTIMEDOUT'
          e.connect = false
          self.emit('error', e)
        }
      })
    }
  }

  self.req.on('response', self.onRequestResponse.bind(self))
  self.req.on('error', self.onRequestError.bind(self))
  self.req.on('drain', function() {
    self.emit('drain')
  })
  self.req.on('socket', function(socket) {
    self.emit('socket', socket)
  })

  self.emit('request', self.req)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>toJSON ()](#apidoc.element.unirest.request.Request.prototype.toJSON)
- description and source-code
```javascript
function requestToJSON() {
  var self = this
  return {
    uri: self.uri,
    method: self.method,
    headers: self.headers
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unirest.request.Request.prototype.write"></a>[function <span class="apidocSignatureSpan">unirest.request.Request.prototype.</span>write ()](#apidoc.element.unirest.request.Request.prototype.write)
- description and source-code
```javascript
write = function () {
  var self = this
  if (self._aborted) {return}

  if (!self._started) {
    self.start()
  }
  if (self.req) {
    return self.req.write.apply(self.req, arguments)
  }
}
```
- example usage
```shell
...
response.setEncoding = function (type) {
  decoder = new StringDecoder(type)
}

// Capture decompression and decode with captured encoding
unzip.on('data', function (buffer) {
  if (!decoder) return stream.emit('data', buffer)
  var string = decoder.write(buffer)
  if (string.length) stream.emit('data', string)
})

// Emit yoself
unzip.on('end', function () {
  stream.emit('end')
})
...
```



# <a name="apidoc.module.unirest.serializers"></a>[module unirest.serializers](#apidoc.module.unirest.serializers)

#### <a name="apidoc.element.unirest.serializers.form"></a>[function <span class="apidocSignatureSpan">unirest.serializers.</span>form (obj)](#apidoc.element.unirest.serializers.form)
- description and source-code
```javascript
form = function (obj) {
  return QueryString.stringify(obj)
}
```
- example usage
```shell
...

Sets 'method' value on 'Request.options' to the given value.

'''js
Request.method('HEAD');
'''

#### Request.form(Object)

Sets 'form' object on 'Request.options' to the given object.

When used 'body' is set to the object passed as a 'querystring' representation and the 'Content-Type' header to 'application/x-www
-form-urlencoded; charset=utf-8'

'''js
Request.form({
...
```

#### <a name="apidoc.element.unirest.serializers.json"></a>[function <span class="apidocSignatureSpan">unirest.serializers.</span>json (obj)](#apidoc.element.unirest.serializers.json)
- description and source-code
```javascript
json = function (obj) {
  return JSON.stringify(obj)
}
```
- example usage
```shell
...

if (is(options).a(Object)) {
  if (options['content-type']) {
    var type = Unirest.type(options['content-type'], true)
    if (type) options.body = Unirest.Response.parse(options.body)
  } else {
    if (is(options.body).a(Object)) {
      options.body = Unirest.serializers.json(options.body)
    }
  }

  $this.options.multipart.push(options)
} else {
  $this.options.multipart.push({
    body: options
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
