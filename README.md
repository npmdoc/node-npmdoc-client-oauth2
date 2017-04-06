# api documentation for  [client-oauth2 (v4.0.0)](https://github.com/mulesoft/js-client-oauth2)  [![npm package](https://img.shields.io/npm/v/npmdoc-client-oauth2.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-client-oauth2) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-client-oauth2.svg)](https://travis-ci.org/npmdoc/node-npmdoc-client-oauth2)
#### Straight-forward execution of OAuth 2.0 flows and authenticated API requests

[![NPM](https://nodei.co/npm/client-oauth2.png?downloads=true)](https://www.npmjs.com/package/client-oauth2)

[![apidoc](https://npmdoc.github.io/node-npmdoc-client-oauth2/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-client-oauth2_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-client-oauth2/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-client-oauth2/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-client-oauth2/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "MuleSoft, Inc."
    },
    "browser": {
        "buffer": false,
        "./src/request/index.js": "./src/request/browser.js"
    },
    "bugs": {
        "url": "https://github.com/mulesoft/js-client-oauth2/issues"
    },
    "dependencies": {
        "popsicle": "^9.1.0"
    },
    "description": "Straight-forward execution of OAuth 2.0 flows and authenticated API requests",
    "devDependencies": {
        "body-parser": "^1.15.2",
        "browserify": "^14.1.0",
        "chai": "^3.2.0",
        "cors": "^2.8.1",
        "envify": "^4.0.0",
        "express": "^4.14.0",
        "is-travis": "^1.0.0",
        "karma": "^1.3.0",
        "karma-browserify": "^5.0.2",
        "karma-chai": "^0.1.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-cli": "^1.0.1",
        "karma-coverage": "^1.1.1",
        "karma-firefox-launcher": "^1.0.0",
        "karma-mocha": "^1.1.1",
        "karma-phantomjs-launcher": "^1.0.0",
        "mocha": "^3.0.2",
        "object-assign": "^4.1.1",
        "phantomjs": "^2.1.3",
        "phantomjs-prebuilt": "^2.1.4",
        "standard": "^9.0.2",
        "watchify": "^3.7.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a2eb7e45be0e69e0b1670cac6e16c00d5bc2f8c0",
        "tarball": "https://registry.npmjs.org/client-oauth2/-/client-oauth2-4.0.0.tgz"
    },
    "engines": {
        "node": ">=4.2.0"
    },
    "files": [
        "src/",
        "index.d.ts",
        "LICENSE"
    ],
    "gitHead": "a199dca2f9f59f5de02a6b1b08e3d7404dd7672a",
    "homepage": "https://github.com/mulesoft/js-client-oauth2",
    "keywords": [
        "oauth2",
        "authentication",
        "token"
    ],
    "license": "Apache-2.0",
    "main": "src/client-oauth2.js",
    "maintainers": [
        {
            "name": "blakeembrey",
            "email": "hello@blakeembrey.com"
        },
        {
            "name": "cesaraugustogarcia",
            "email": "cesaraugusto86@hotmail.com"
        },
        {
            "name": "christianvogel",
            "email": "christianvogel84@gmail.com"
        },
        {
            "name": "juan.coen",
            "email": "juan.coen@mulesoft.com"
        },
        {
            "name": "mulesoft-npm",
            "email": "mulesoft-npm@mulesoft.com"
        }
    ],
    "name": "client-oauth2",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/mulesoft/js-client-oauth2.git"
    },
    "scripts": {
        "lint": "standard",
        "test": "npm run lint && npm run test-server-open && npm run test-node && npm run test-browser; npm run test-server-close",
        "test-browser": "PORT=7357 karma start --single-run",
        "test-node": "PORT=7357 mocha -R spec --bail --require test/support/globals.js",
        "test-server-close": "if [ -f server.pid ]; then kill -9 $(cat server.pid); rm server.pid; fi",
        "test-server-open": "PORT=7357 node test/support/server.js & echo $! > server.pid"
    },
    "typings": "index.d.ts",
    "version": "4.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module client-oauth2](#apidoc.module.client-oauth2)
1.  [function <span class="apidocSignatureSpan">client-oauth2.</span>Token (client, data)](#apidoc.element.client-oauth2.Token)
1.  object <span class="apidocSignatureSpan">client-oauth2.</span>Token.prototype

#### [module client-oauth2.Token](#apidoc.module.client-oauth2.Token)
1.  [function <span class="apidocSignatureSpan">client-oauth2.</span>Token (client, data)](#apidoc.element.client-oauth2.Token.Token)

#### [module client-oauth2.Token.prototype](#apidoc.module.client-oauth2.Token.prototype)
1.  [function <span class="apidocSignatureSpan">client-oauth2.Token.prototype.</span>expired ()](#apidoc.element.client-oauth2.Token.prototype.expired)
1.  [function <span class="apidocSignatureSpan">client-oauth2.Token.prototype.</span>expiresIn (duration)](#apidoc.element.client-oauth2.Token.prototype.expiresIn)
1.  [function <span class="apidocSignatureSpan">client-oauth2.Token.prototype.</span>refresh (opts)](#apidoc.element.client-oauth2.Token.prototype.refresh)
1.  [function <span class="apidocSignatureSpan">client-oauth2.Token.prototype.</span>sign (requestObject)](#apidoc.element.client-oauth2.Token.prototype.sign)



# <a name="apidoc.module.client-oauth2"></a>[module client-oauth2](#apidoc.module.client-oauth2)

#### <a name="apidoc.element.client-oauth2.Token"></a>[function <span class="apidocSignatureSpan">client-oauth2.</span>Token (client, data)](#apidoc.element.client-oauth2.Token)
- description and source-code
```javascript
function ClientOAuth2Token(client, data) {
  this.client = client
  this.data = data
  this.tokenType = data.token_type && data.token_type.toLowerCase()
  this.accessToken = data.access_token
  this.refreshToken = data.refresh_token

  this.expiresIn(Number(data.expires_in))
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.client-oauth2.Token"></a>[module client-oauth2.Token](#apidoc.module.client-oauth2.Token)

#### <a name="apidoc.element.client-oauth2.Token.Token"></a>[function <span class="apidocSignatureSpan">client-oauth2.</span>Token (client, data)](#apidoc.element.client-oauth2.Token.Token)
- description and source-code
```javascript
function ClientOAuth2Token(client, data) {
  this.client = client
  this.data = data
  this.tokenType = data.token_type && data.token_type.toLowerCase()
  this.accessToken = data.access_token
  this.refreshToken = data.refresh_token

  this.expiresIn(Number(data.expires_in))
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.client-oauth2.Token.prototype"></a>[module client-oauth2.Token.prototype](#apidoc.module.client-oauth2.Token.prototype)

#### <a name="apidoc.element.client-oauth2.Token.prototype.expired"></a>[function <span class="apidocSignatureSpan">client-oauth2.Token.prototype.</span>expired ()](#apidoc.element.client-oauth2.Token.prototype.expired)
- description and source-code
```javascript
expired = function () {
  return Date.now() > this.expires.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.client-oauth2.Token.prototype.expiresIn"></a>[function <span class="apidocSignatureSpan">client-oauth2.Token.prototype.</span>expiresIn (duration)](#apidoc.element.client-oauth2.Token.prototype.expiresIn)
- description and source-code
```javascript
expiresIn = function (duration) {
  if (typeof duration === 'number') {
    this.expires = new Date()
    this.expires.setSeconds(this.expires.getSeconds() + duration)
  } else if (duration instanceof Date) {
    this.expires = new Date(duration.getTime())
  } else {
    throw new TypeError('Unknown duration: ' + duration)
  }

  return this.expires
}
```
- example usage
```shell
...
To re-create an access token instance and make requests on behalf on the user, you can create an access token instance by using
the 'createToken' method on a client instance.

'''javascript
// Can also just pass the raw 'data' object in place of an argument.
var token = githubAuth.createToken('access token', 'optional refresh token', 'optional token type', { data: 'raw user data' })

// Set the token TTL.
token.expiresIn(1234) // Seconds.
token.expiresIn(new Date('2016-11-08')) // Date.

// Refresh the users credentials and save the new access token and info.
token.refresh().then(storeNewToken)

// Sign a standard HTTP request object, updating the URL with the access token
// or adding authorization headers, depending on token type.
...
```

#### <a name="apidoc.element.client-oauth2.Token.prototype.refresh"></a>[function <span class="apidocSignatureSpan">client-oauth2.Token.prototype.</span>refresh (opts)](#apidoc.element.client-oauth2.Token.prototype.refresh)
- description and source-code
```javascript
refresh = function (opts) {
  var self = this
  var options = Object.assign({}, this.client.options, opts)

  if (!this.refreshToken) {
    return Promise.reject(new Error('No refresh token'))
  }

  return this.client._request(requestOptions({
    url: options.accessTokenUri,
    method: 'POST',
    headers: Object.assign({}, DEFAULT_HEADERS, {
      Authorization: auth(options.clientId, options.clientSecret)
    }),
    body: {
      refresh_token: this.refreshToken,
      grant_type: 'refresh_token'
    }
  }, options))
    .then(function (data) {
      return self.client.createToken(Object.assign({}, self.data, data))
    })
}
```
- example usage
```shell
...
var token = githubAuth.createToken('access token', 'optional refresh token', 'optional token type', { data: 'raw user data' })

// Set the token TTL.
token.expiresIn(1234) // Seconds.
token.expiresIn(new Date('2016-11-08')) // Date.

// Refresh the users credentials and save the new access token and info.
token.refresh().then(storeNewToken)

// Sign a standard HTTP request object, updating the URL with the access token
// or adding authorization headers, depending on token type.
token.sign({
  method: 'get',
  url: 'https://api.github.com/users'
}) //=> { method, url, headers, ... }
...
```

#### <a name="apidoc.element.client-oauth2.Token.prototype.sign"></a>[function <span class="apidocSignatureSpan">client-oauth2.Token.prototype.</span>sign (requestObject)](#apidoc.element.client-oauth2.Token.prototype.sign)
- description and source-code
```javascript
sign = function (requestObject) {
  if (!this.accessToken) {
    throw new Error('Unable to sign without access token')
  }

  requestObject.headers = requestObject.headers || {}

  if (this.tokenType === 'bearer') {
    requestObject.headers.Authorization = 'Bearer ' + this.accessToken
  } else {
    var parts = requestObject.url.split('#')
    var token = 'access_token=' + this.accessToken
    var url = parts[0].replace(/[?&]access_token=[^&#]/, '')
    var fragment = parts[1] ? '#' + parts[1] : ''

    // Prepend the correct query string parameter to the url.
    requestObject.url = url + (url.indexOf('?') > -1 ? '&' : '?') + token + fragment

    // Attempt to avoid storing the url in proxies, since the access token
    // is exposed in the query parameters.
    requestObject.headers.Pragma = 'no-store'
    requestObject.headers['Cache-Control'] = 'no-store'
  }

  return requestObject
}
```
- example usage
```shell
...
token.expiresIn(new Date('2016-11-08')) // Date.

// Refresh the users credentials and save the new access token and info.
token.refresh().then(storeNewToken)

// Sign a standard HTTP request object, updating the URL with the access token
// or adding authorization headers, depending on token type.
token.sign({
  method: 'get',
  url: 'https://api.github.com/users'
}) //=> { method, url, headers, ... }
'''

**P.S.** All authorization methods accept 'options' as the last argument, useful for overriding the global configuration on a per
-request basis.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
