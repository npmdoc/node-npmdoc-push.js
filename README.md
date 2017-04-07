# api documentation for  [push.js (v0.0.13)](https://github.com/Nickersoft/push.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-push.js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-push.js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-push.js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-push.js)
#### A compact, cross-browser solution for the Javascript Notifications API

[![NPM](https://nodei.co/npm/push.js.png?downloads=true)](https://www.npmjs.com/package/push.js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-push.js/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-push.js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-push.js/build/apidoc.html)

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
            "name": "nickersoft",
            "email": "nickersoft@gmail.com"
        }
    ],
    "name": "push.js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Nickersoft/push.js.git"
    },
    "scripts": {
        "build": "uglifyjs push.js -o push.min.js --comments",
        "prepublish": "npm run build",
        "test": "karma start"
    },
    "version": "0.0.13"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module push.js](#apidoc.module.push.js)
1.  boolean <span class="apidocSignatureSpan">push.js.</span>isSupported
1.  [function <span class="apidocSignatureSpan">push.js.</span>__lastWorkerPath ()](#apidoc.element.push.js.__lastWorkerPath)
1.  [function <span class="apidocSignatureSpan">push.js.</span>clear ()](#apidoc.element.push.js.clear)
1.  [function <span class="apidocSignatureSpan">push.js.</span>close (tag)](#apidoc.element.push.js.close)
1.  [function <span class="apidocSignatureSpan">push.js.</span>count ()](#apidoc.element.push.js.count)
1.  [function <span class="apidocSignatureSpan">push.js.</span>create (title, options)](#apidoc.element.push.js.create)
1.  object <span class="apidocSignatureSpan">push.js.</span>Permission
1.  object <span class="apidocSignatureSpan">push.js.</span>js.Permission

#### [module push.js.Permission](#apidoc.module.push.js.Permission)
1.  [function <span class="apidocSignatureSpan">push.js.Permission.</span>get ()](#apidoc.element.push.js.Permission.get)
1.  [function <span class="apidocSignatureSpan">push.js.Permission.</span>has ()](#apidoc.element.push.js.Permission.has)
1.  [function <span class="apidocSignatureSpan">push.js.Permission.</span>request (onGranted, onDenied)](#apidoc.element.push.js.Permission.request)
1.  string <span class="apidocSignatureSpan">push.js.Permission.</span>DEFAULT
1.  string <span class="apidocSignatureSpan">push.js.Permission.</span>DENIED
1.  string <span class="apidocSignatureSpan">push.js.Permission.</span>GRANTED



# <a name="apidoc.module.push.js"></a>[module push.js](#apidoc.module.push.js)

#### <a name="apidoc.element.push.js.__lastWorkerPath"></a>[function <span class="apidocSignatureSpan">push.js.</span>__lastWorkerPath ()](#apidoc.element.push.js.__lastWorkerPath)
- description and source-code
```javascript
__lastWorkerPath = function () {
    return self.lastWorkerPath;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.push.js.clear"></a>[function <span class="apidocSignatureSpan">push.js.</span>clear ()](#apidoc.element.push.js.clear)
- description and source-code
```javascript
clear = function () {
    var success = true;

    for (key in notifications)
        success = success && closeNotification(key);

    return success;
}
```
- example usage
```shell
...
    notification.close();
});
'''

When it comes to clearing all open notifications, that's just as easy as well:

'''javascript
Push.clear();
'''

**Important:** Although Javascript promises are [decently supported](http://caniuse.com/#search=promises) across
browsers, there are still some browsers that lack support. If you find that you are trying to support a browser that
doesn't support promises, chances are it won't support notifications either. However, if you are really determined, I
encourage you to checkout the lightweight [promise-polyfill](https://github.com/taylorhakes/promise-polyfill) library
by Taylor Hakes (or something similar). This library used to be bundled with Push, until it was decided that it'd be
...
```

#### <a name="apidoc.element.push.js.close"></a>[function <span class="apidocSignatureSpan">push.js.</span>close (tag)](#apidoc.element.push.js.close)
- description and source-code
```javascript
close = function (tag) {
    var key;
    for (key in notifications) {
        notification = notifications[key];
<span class="apidocCodeCommentSpan">        /* Run only if the tags match */
</span>        if (notification.tag === tag) {
            /* Call the notification's close() method */
            return closeNotification(key);
        }
    }
}
```
- example usage
```shell
...
'''javascript
Push.create('Hello World!', {
    tag: 'foo'
});

// Somewhere later in your code...

Push.close('foo');
'''

Alternatively, you can assign the notification promise returned by Push to a variable and close it directly using the
promise's then() method:

'''javascript
var promise = Push.create('Hello World!');
...
```

#### <a name="apidoc.element.push.js.count"></a>[function <span class="apidocSignatureSpan">push.js.</span>count ()](#apidoc.element.push.js.count)
- description and source-code
```javascript
count = function () {
    var count = 0,
        key;

    for (key in notifications)
        count++;

    return count;
}
```
- example usage
```shell
...
});
'''

If the browser does not have permission to send push notifications, Push will automatically request permission as soon
as create() is called. Simple as that. If you wish to know how many notifications are currently open, simply call:

'''javascript
Push.count();
'''

#### Closing Notifications ####
When it comes to closing notifications, you have a few options. You can either set a timeout (see "Options"), call
Push's close() method, or pass around the notification's promise object and then call close() directly. Push's close()
method will only work with newer browsers, taking in a notification's unique tag name and closing the first notification
it finds with that tag:
...
```

#### <a name="apidoc.element.push.js.create"></a>[function <span class="apidocSignatureSpan">push.js.</span>create (title, options)](#apidoc.element.push.js.create)
- description and source-code
```javascript
create = function (title, options) {
    var promiseCallback;

<span class="apidocCodeCommentSpan">    /* Fail if the browser is not supported */
</span>    if (!self.isSupported) {
        throw new Error(incompatibilityErrorMessage);
    }

    /* Fail if no or an invalid title is provided */
    if (!isString(title)) {
        throw new Error('PushError: Title of notification must be a string');
    }

    /* Request permission if it isn't granted */
    if (!self.Permission.has()) {
        promiseCallback = function(resolve, reject) {
            self.Permission.request(function() {
                try {
                    createCallback(title, options, resolve);
                } catch (e) {
                    reject(e);
                }
            }, function() {
                reject("Permission request declined");
            });
        };
    } else {
        promiseCallback = function(resolve, reject) {
            try {
                createCallback(title, options, resolve);
            } catch (e) {
                reject(e);
            }
        };
    }

    return new Promise(promiseCallback);
}
```
- example usage
```shell
...

For more information regarding the Push NPM package, [see here](https://www.npmjs.com/package/push.js).

#### Creating Notifications ####
So just how easy is it to create a notification using Push? We can do it in just one line, actually:

'''javascript
Push.create('Hello World!')
'''

No constructors, just a universal API you can access from anywhere. Push is even compatible with AMD as well:

'''javascript
define(['pushjs'], function (Push) {
Push.create('Hello World!');
...
```



# <a name="apidoc.module.push.js.Permission"></a>[module push.js.Permission](#apidoc.module.push.js.Permission)

#### <a name="apidoc.element.push.js.Permission.get"></a>[function <span class="apidocSignatureSpan">push.js.Permission.</span>get ()](#apidoc.element.push.js.Permission.get)
- description and source-code
```javascript
get = function () {

    var permission;

<span class="apidocCodeCommentSpan">    /* Return if Push not supported */
</span>    if (!self.isSupported) { throw new Error(incompatibilityErrorMessage); }

    /* Safari 6+, Chrome 23+ */
    if (w.Notification && w.Notification.permissionLevel) {
        permission = w.Notification.permissionLevel;

    /* Legacy webkit browsers */
    } else if (w.webkitNotifications && w.webkitNotifications.checkPermission) {
        permission = Permissions[w.webkitNotifications.checkPermission()];

    /* Firefox 23+ */
    } else if (w.Notification && w.Notification.permission) {
        permission = w.Notification.permission;

    /* Firefox Mobile */
    } else if (navigator.mozNotification) {
        permission = Permission.GRANTED;

    /* IE9+ */
    } else if (w.external && w.external.msIsSiteMode() !== undefined) {
        permission = w.external.msIsSiteMode() ? Permission.GRANTED : Permission.DEFAULT;
    } else {
        throw new Error(incompatibilityErrorMessage);
    }

    return permission;

}
```
- example usage
```shell
...

#### Native Permission Levels ####

If you feel like being *really* geeky, you can get the raw permission level from native API itself (scary stuff, I know)
using:

'''javascript
Push.Permission.get();
'''

This returns a string value which may or may not coincidentally be represented by Push's constants. Use this info as you
please.

### Options ###
...
```

#### <a name="apidoc.element.push.js.Permission.has"></a>[function <span class="apidocSignatureSpan">push.js.Permission.</span>has ()](#apidoc.element.push.js.Permission.has)
- description and source-code
```javascript
has = function () {
    return Permission.get() === Permission.GRANTED;
}
```
- example usage
```shell
...
guessed it, the permission is denied. Note that if 'Permission.DEFAULT' is returned, no callback is executed.

#### Reading Permission ####

To find out whether or not Push has permission to show notifications, just call:

'''javascript
Push.Permission.has();
'''

which will return a boolean value denoting permission.

#### Native Permission Levels ####

If you feel like being *really* geeky, you can get the raw permission level from native API itself (scary stuff, I know)
...
```

#### <a name="apidoc.element.push.js.Permission.request"></a>[function <span class="apidocSignatureSpan">push.js.Permission.</span>request (onGranted, onDenied)](#apidoc.element.push.js.Permission.request)
- description and source-code
```javascript
request = function (onGranted, onDenied) {
    var existing = self.Permission.get();

<span class="apidocCodeCommentSpan">    /* Return if Push not supported */
</span>    if (!self.isSupported) {
        throw new Error(incompatibilityErrorMessage);
    }

    /* Default callback */
    callback = function (result) {
        switch (result) {

            case self.Permission.GRANTED:
                if (onGranted) onGranted();
                break;

            case self.Permission.DENIED:
                if (onDenied) onDenied();
                break;

        }

    };

    /* Permissions already set */
    if (existing !== self.Permission.DEFAULT) {
        callback(existing);
    }
    /* Safari 6+, Chrome 23+ */
    else if (w.Notification && w.Notification.requestPermission) {
        Notification.requestPermission(callback);
    }
    /* Legacy webkit browsers */
    else if (w.webkitNotifications && w.webkitNotifications.checkPermission) {
        w.webkitNotifications.requestPermission(callback);
    } else {
        throw new Error(incompatibilityErrorMessage);
    }
}
```
- example usage
```shell
...
'''

#### Requesting Permission ####

To manually request notification permission, simply call:

'''javascript
Push.Permission.request(onGranted, onDenied);
'''

where 'onGranted' is a callback function for if permision is granted, and 'onDenied' is a callback function for if, you
guessed it, the permission is denied. Note that if 'Permission.DEFAULT' is returned, no callback is executed.

#### Reading Permission ####
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
