# npmdoc-client-oauth2

#### api documentation for  [client-oauth2 (v4.0.0)](https://github.com/mulesoft/js-client-oauth2)  [![npm package](https://img.shields.io/npm/v/npmdoc-client-oauth2.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-client-oauth2) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-client-oauth2.svg)](https://travis-ci.org/npmdoc/node-npmdoc-client-oauth2)

#### Straight-forward execution of OAuth 2.0 flows and authenticated API requests

[![NPM](https://nodei.co/npm/client-oauth2.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/client-oauth2)

- [https://npmdoc.github.io/node-npmdoc-client-oauth2/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-client-oauth2/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-client-oauth2/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-client-oauth2/build/apidoc.html)

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
            "name": "blakeembrey"
        },
        {
            "name": "cesaraugustogarcia"
        },
        {
            "name": "christianvogel"
        },
        {
            "name": "juan.coen"
        },
        {
            "name": "mulesoft-npm"
        }
    ],
    "name": "client-oauth2",
    "optionalDependencies": {},
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



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
