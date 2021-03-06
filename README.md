# npmdoc-push.js

#### basic api documentation for  [push.js (v0.0.13)](https://github.com/Nickersoft/push.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-push.js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-push.js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-push.js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-push.js)

#### A compact, cross-browser solution for the Javascript Notifications API

[![NPM](https://nodei.co/npm/push.js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/push.js)

- [https://npmdoc.github.io/node-npmdoc-push.js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-push.js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-push.js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-push.js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-push.js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-push.js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tyler Nickerson"
    },
    "bugs": {
        "url": "https://github.com/Nickersoft/push.js/issues"
    },
    "dependencies": {},
    "description": "A compact, cross-browser solution for the Javascript Notifications API",
    "devDependencies": {
        "coveralls": "^2.11.15",
        "jasmine-core": "^2.4.1",
        "karma": "^0.13.22",
        "karma-coverage": "^1.0.0",
        "karma-firefox-launcher": "^0.1.7",
        "karma-jasmine": "^0.3.8",
        "karma-mocha-reporter": "^1.3.0",
        "uglify-js": "^2.6.2"
    },
    "directories": {},
    "dist": {
        "shasum": "05f3bf5c414e386b45f9f61a98f9e3ecc7a5f4b4",
        "tarball": "https://registry.npmjs.org/push.js/-/push.js-0.0.13.tgz"
    },
    "files": [
        "test",
        "*.js",
        "*.html",
        "*.md"
    ],
    "gitHead": "cd7ce07fec031494a0db21b4fb2911863e251c82",
    "homepage": "https://github.com/Nickersoft/push.js",
    "license": "MIT",
    "main": "push.js",
    "maintainers": [
        {
            "name": "nickersoft"
        }
    ],
    "name": "push.js",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Nickersoft/push.js.git"
    },
    "scripts": {
        "build": "uglifyjs push.js -o push.min.js --comments",
        "prepublish": "npm run build",
        "test": "karma start"
    },
    "version": "0.0.13",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
