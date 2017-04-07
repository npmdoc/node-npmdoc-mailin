# api documentation for  [mailin (v3.0.4)](https://github.com/Flolagale/mailin)  [![npm package](https://img.shields.io/npm/v/npmdoc-mailin.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mailin) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mailin.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mailin)
#### Artisanal inbound emails for every web app

[![NPM](https://nodei.co/npm/mailin.png?downloads=true)](https://www.npmjs.com/package/mailin)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mailin/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mailin_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mailin/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mailin/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mailin/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Florent Galland"
    },
    "bin": {
        "mailin": "./run-cli.js"
    },
    "bugs": {
        "url": "https://github.com/Flolagale/mailin/issues"
    },
    "dependencies": {
        "bluebird": "^2.9.30",
        "commander": "^2.8.1",
        "extend": "^2.0.1",
        "forever-monitor": "^1.5.2",
        "html-to-text": "^1.3.1",
        "languagedetect": "^1.1.1",
        "lodash": "^3.9.3",
        "mailparser": "^0.5.1",
        "node-uuid": "^1.4.3",
        "semver": "^5.0.1",
        "shelljs": "^0.5.1",
        "smtp-server": "^1.4.0",
        "spamc": "0.0.5",
        "superagent": "^1.2.0",
        "winston": "^1.0.0"
    },
    "description": "Artisanal inbound emails for every web app",
    "devDependencies": {
        "async": "^1.5.0",
        "chai": "^3.0.0",
        "chai-as-promised": "^5.1.0",
        "express": "^4.13.0",
        "grunt": "^0.4.5",
        "grunt-contrib-jshint": "^0.11.2",
        "grunt-jsbeautifier": "~0.2.10",
        "grunt-mocha-test": "^0.12.7",
        "mocha": "^1.20.0",
        "multiparty": "^4.1.2",
        "should": "^7.0.1",
        "smtp-connection": "^1.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "47a381c1f94b5ecb4dc3808459afbe474f27aa8c",
        "tarball": "https://registry.npmjs.org/mailin/-/mailin-3.0.4.tgz"
    },
    "engine": "node ~0.12.4",
    "gitHead": "6fd516b4c69cf4f42745b03730a4dfabb5af39ad",
    "homepage": "https://github.com/Flolagale/mailin",
    "keywords": [
        "incoming",
        "inbound",
        "email",
        "parse",
        "smtp",
        "easy",
        "webhook",
        "post"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "flolagale",
            "email": "flolagale@gmail.com"
        }
    ],
    "name": "mailin",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Flolagale/mailin.git"
    },
    "scripts": {
        "start": "./run-cli.js",
        "test": "node -e \"require('grunt').tasks(['mochaTest']);\""
    },
    "version": "3.0.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mailin](#apidoc.module.mailin)
1.  number <span class="apidocSignatureSpan">mailin.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">mailin.</span>_events
1.  object <span class="apidocSignatureSpan">mailin.</span>_smtp
1.  object <span class="apidocSignatureSpan">mailin.</span>configuration
1.  object <span class="apidocSignatureSpan">mailin.</span>domain
1.  object <span class="apidocSignatureSpan">mailin.</span>logger
1.  object <span class="apidocSignatureSpan">mailin.</span>mailUtilities

#### [module mailin.logger](#apidoc.module.mailin.logger)
1.  boolean <span class="apidocSignatureSpan">mailin.logger.</span>emitErrs
1.  boolean <span class="apidocSignatureSpan">mailin.logger.</span>exitOnError
1.  boolean <span class="apidocSignatureSpan">mailin.logger.</span>padLevels
1.  boolean <span class="apidocSignatureSpan">mailin.logger.</span>stripColors
1.  [function <span class="apidocSignatureSpan">mailin.logger.</span>_error (msg)](#apidoc.element.mailin.logger._error)
1.  [function <span class="apidocSignatureSpan">mailin.logger.</span>debug (msg)](#apidoc.element.mailin.logger.debug)
1.  [function <span class="apidocSignatureSpan">mailin.logger.</span>error (err)](#apidoc.element.mailin.logger.error)
1.  [function <span class="apidocSignatureSpan">mailin.logger.</span>info (msg)](#apidoc.element.mailin.logger.info)
1.  [function <span class="apidocSignatureSpan">mailin.logger.</span>setLevel (level)](#apidoc.element.mailin.logger.setLevel)
1.  [function <span class="apidocSignatureSpan">mailin.logger.</span>setLogFile (logFilePath)](#apidoc.element.mailin.logger.setLogFile)
1.  [function <span class="apidocSignatureSpan">mailin.logger.</span>silly (msg)](#apidoc.element.mailin.logger.silly)
1.  [function <span class="apidocSignatureSpan">mailin.logger.</span>verbose (msg)](#apidoc.element.mailin.logger.verbose)
1.  [function <span class="apidocSignatureSpan">mailin.logger.</span>warn (msg)](#apidoc.element.mailin.logger.warn)
1.  number <span class="apidocSignatureSpan">mailin.logger.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">mailin.logger.</span>_events
1.  object <span class="apidocSignatureSpan">mailin.logger.</span>_hnames
1.  object <span class="apidocSignatureSpan">mailin.logger.</span>_names
1.  object <span class="apidocSignatureSpan">mailin.logger.</span>domain
1.  object <span class="apidocSignatureSpan">mailin.logger.</span>exceptionHandlers
1.  object <span class="apidocSignatureSpan">mailin.logger.</span>filters
1.  object <span class="apidocSignatureSpan">mailin.logger.</span>levels
1.  object <span class="apidocSignatureSpan">mailin.logger.</span>profilers
1.  object <span class="apidocSignatureSpan">mailin.logger.</span>rewriters
1.  object <span class="apidocSignatureSpan">mailin.logger.</span>transports
1.  string <span class="apidocSignatureSpan">mailin.logger.</span>level

#### [module mailin.mailUtilities](#apidoc.module.mailin.mailUtilities)
1.  [function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>computeSpamScore (rawEmail, callback)](#apidoc.element.mailin.mailUtilities.computeSpamScore)
1.  [function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>computeSpamScoreAsync (_arg0, _arg1, _arg2)](#apidoc.element.mailin.mailUtilities.computeSpamScoreAsync)
1.  [function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>validateDkim (rawEmail, callback)](#apidoc.element.mailin.mailUtilities.validateDkim)
1.  [function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>validateDkimAsync (_arg0, _arg1, _arg2)](#apidoc.element.mailin.mailUtilities.validateDkimAsync)
1.  [function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>validateSpf (ip, address, host, callback)](#apidoc.element.mailin.mailUtilities.validateSpf)
1.  [function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>validateSpfAsync (_arg0, _arg1, _arg2)](#apidoc.element.mailin.mailUtilities.validateSpfAsync)



# <a name="apidoc.module.mailin"></a>[module mailin](#apidoc.module.mailin)



# <a name="apidoc.module.mailin.logger"></a>[module mailin.logger](#apidoc.module.mailin.logger)

#### <a name="apidoc.element.mailin.logger._error"></a>[function <span class="apidocSignatureSpan">mailin.logger.</span>_error (msg)](#apidoc.element.mailin.logger._error)
- description and source-code
```javascript
_error = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
    if (logger.transports.file) logger.transports.file.level = level;
}
};

logger._error = logger.error;
logger.error = function (err) {
if (err.stack) {
    this._error(err.stack);
} else if (!_.isString(err)) {
    this._error(util.inspect(err, {
        depth: 5
    }));
} else {
    this._error.apply(this, arguments);
}
...
```

#### <a name="apidoc.element.mailin.logger.debug"></a>[function <span class="apidocSignatureSpan">mailin.logger.</span>debug (msg)](#apidoc.element.mailin.logger.debug)
- description and source-code
```javascript
debug = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mailin.logger.error"></a>[function <span class="apidocSignatureSpan">mailin.logger.</span>error (err)](#apidoc.element.mailin.logger.error)
- description and source-code
```javascript
error = function (err) {
    if (err.stack) {
        this._error(err.stack);
    } else if (!_.isString(err)) {
        this._error(util.inspect(err, {
            depth: 5
        }));
    } else {
        this._error.apply(this, arguments);
    }
}
```
- example usage
```shell
...
});
};

/* Parameter level is one of 'silly', 'verbose', 'debug', 'info', 'warn',
 * 'error'. */
logger.setLevel = function (level) {
if (['silly', 'verbose', 'debug', 'info', 'warn', 'error'].indexOf(level) === -1) {
    logger.error('Unable to set logging level to unknown level "' + level + '".');
} else {
    /* Verbose and debug have not exactly the same semantic in Mailin and
     * Winston, so handle that. */
    if (logger.transports.console.level === 'verbose' &&
        level === 'debug') {
        return;
    }
...
```

#### <a name="apidoc.element.mailin.logger.info"></a>[function <span class="apidocSignatureSpan">mailin.logger.</span>info (msg)](#apidoc.element.mailin.logger.info)
- description and source-code
```javascript
info = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mailin.logger.setLevel"></a>[function <span class="apidocSignatureSpan">mailin.logger.</span>setLevel (level)](#apidoc.element.mailin.logger.setLevel)
- description and source-code
```javascript
setLevel = function (level) {
    if (['silly', 'verbose', 'debug', 'info', 'warn', 'error'].indexOf(level) === -1) {
        logger.error('Unable to set logging level to unknown level "' + level + '".');
    } else {
<span class="apidocCodeCommentSpan">        /* Verbose and debug have not exactly the same semantic in Mailin and
         * Winston, so handle that. */
</span>        if (logger.transports.console.level === 'verbose' &&
            level === 'debug') {
            return;
        }

        logger.transports.console.level = level;

        if (logger.transports.file) logger.transports.file.level = level;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mailin.logger.setLogFile"></a>[function <span class="apidocSignatureSpan">mailin.logger.</span>setLogFile (logFilePath)](#apidoc.element.mailin.logger.setLogFile)
- description and source-code
```javascript
setLogFile = function (logFilePath) {
    this.add(winston.transports.File, {
        filename: logFilePath,
        json: false,
        maxsize: 20000000,
        timestamp: true
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mailin.logger.silly"></a>[function <span class="apidocSignatureSpan">mailin.logger.</span>silly (msg)](#apidoc.element.mailin.logger.silly)
- description and source-code
```javascript
silly = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mailin.logger.verbose"></a>[function <span class="apidocSignatureSpan">mailin.logger.</span>verbose (msg)](#apidoc.element.mailin.logger.verbose)
- description and source-code
```javascript
verbose = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
    return callback(null, false);
}

var verifyDkimPath = path.join(__dirname, '../python/verifydkim.py');
var verifyDkim = child_process.spawn('python', [verifyDkimPath]);

verifyDkim.stdout.on('data', function (data) {
    logger.verbose(data.toString());
});

verifyDkim.on('close', function (code) {
    logger.verbose('closed with return code ' + code);
    /* Convert return code to appropriate boolean. */
    return callback(null, !!!code);
});
...
```

#### <a name="apidoc.element.mailin.logger.warn"></a>[function <span class="apidocSignatureSpan">mailin.logger.</span>warn (msg)](#apidoc.element.mailin.logger.warn)
- description and source-code
```javascript
warn = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
var path = require('path');
var Spamc = require('spamc');
var spamc = new Spamc();

/* Verify Python availability. */
var isPythonAvailable = shell.which('python');
if (!isPythonAvailable) {
logger.warn('Python is not available. Dkim and spf checking is disabled.');
}

/* Verify spamc/spamassassin availability. */
var isSpamcAvailable = true;
if (!shell.which('spamassassin') || !shell.which('spamc')) {
logger.warn('Either spamassassin or spamc are not available. Spam score computation is disabled.');
isSpamcAvailable = false;
...
```



# <a name="apidoc.module.mailin.mailUtilities"></a>[module mailin.mailUtilities](#apidoc.module.mailin.mailUtilities)

#### <a name="apidoc.element.mailin.mailUtilities.computeSpamScore"></a>[function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>computeSpamScore (rawEmail, callback)](#apidoc.element.mailin.mailUtilities.computeSpamScore)
- description and source-code
```javascript
computeSpamScore = function (rawEmail, callback) {
    if (!isSpamcAvailable) {
        return callback(null, 0.0);
    }

    spamc.report(rawEmail, function (err, result) {
        logger.verbose(result);
        if (err) logger.error(err);
        if (err) return callback(new Error('Unable to compute spam score.'));
        callback(null, result.spamScore);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mailin.mailUtilities.computeSpamScoreAsync"></a>[function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>computeSpamScoreAsync (_arg0, _arg1, _arg2)](#apidoc.element.mailin.mailUtilities.computeSpamScoreAsync)
- description and source-code
```javascript
computeSpamScoreAsync = function (_arg0, _arg1, _arg2) {
    'use strict';
    var len = arguments.length;
    var promise = new Promise(INTERNAL);
    promise._captureStackTrace();
    var nodeback = nodebackForPromise(promise);
    var ret;
    var callback = tryCatch(this != null ? this['computeSpamScore'] : fn);
    switch(len) {
        case 1:ret = callback.call(this, _arg0, nodeback); break;
case 0:ret = callback.call(this, nodeback); break;
case 2:ret = callback.call(this, _arg0, _arg1, nodeback); break;
case 3:ret = callback.call(this, _arg0, _arg1, _arg2, nodeback); break;

default:
    var args = new Array(len + 1);
    var i = 0;
    for (var i = 0; i < len; ++i) {
       args[i] = arguments[i];
    }
    args[i] = nodeback;
    ret = callback.apply(this, args);

    break;

    }
    if (ret === errorObj) {
        promise._rejectCallback(maybeWrapAsError(ret.e), true, true);
    }
    return promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mailin.mailUtilities.validateDkim"></a>[function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>validateDkim (rawEmail, callback)](#apidoc.element.mailin.mailUtilities.validateDkim)
- description and source-code
```javascript
validateDkim = function (rawEmail, callback) {
    if (!isPythonAvailable) {
        return callback(null, false);
    }

    var verifyDkimPath = path.join(__dirname, '../python/verifydkim.py');
    var verifyDkim = child_process.spawn('python', [verifyDkimPath]);

    verifyDkim.stdout.on('data', function (data) {
        logger.verbose(data.toString());
    });

    verifyDkim.on('close', function (code) {
        logger.verbose('closed with return code ' + code);
<span class="apidocCodeCommentSpan">        /* Convert return code to appropriate boolean. */
</span>        return callback(null, !!!code);
    });

    verifyDkim.stdin.write(rawEmail);
    verifyDkim.stdin.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mailin.mailUtilities.validateDkimAsync"></a>[function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>validateDkimAsync (_arg0, _arg1, _arg2)](#apidoc.element.mailin.mailUtilities.validateDkimAsync)
- description and source-code
```javascript
validateDkimAsync = function (_arg0, _arg1, _arg2) {
    'use strict';
    var len = arguments.length;
    var promise = new Promise(INTERNAL);
    promise._captureStackTrace();
    var nodeback = nodebackForPromise(promise);
    var ret;
    var callback = tryCatch(this != null ? this['validateDkim'] : fn);
    switch(len) {
        case 1:ret = callback.call(this, _arg0, nodeback); break;
case 0:ret = callback.call(this, nodeback); break;
case 2:ret = callback.call(this, _arg0, _arg1, nodeback); break;
case 3:ret = callback.call(this, _arg0, _arg1, _arg2, nodeback); break;

default:
    var args = new Array(len + 1);
    var i = 0;
    for (var i = 0; i < len; ++i) {
       args[i] = arguments[i];
    }
    args[i] = nodeback;
    ret = callback.apply(this, args);

    break;

    }
    if (ret === errorObj) {
        promise._rejectCallback(maybeWrapAsError(ret.e), true, true);
    }
    return promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mailin.mailUtilities.validateSpf"></a>[function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>validateSpf (ip, address, host, callback)](#apidoc.element.mailin.mailUtilities.validateSpf)
- description and source-code
```javascript
validateSpf = function (ip, address, host, callback) {
    if (!isPythonAvailable) {
        return callback(null, false);
    }

    var verifySpfPath = path.join(__dirname, '../python/verifyspf.py');
    var cmd = 'python ' + verifySpfPath + ' ' + ip + ' ' + address + ' ' + host;
    child_process.exec(cmd, function (err, stdout) {
        logger.verbose(stdout);
        var code = 0;
        if (err) {
            code = err.code;
        }

        logger.verbose('closed with return code ' + code);

<span class="apidocCodeCommentSpan">        /* Convert return code to appropriate boolean. */
</span>        return callback(null, !!!code);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mailin.mailUtilities.validateSpfAsync"></a>[function <span class="apidocSignatureSpan">mailin.mailUtilities.</span>validateSpfAsync (_arg0, _arg1, _arg2)](#apidoc.element.mailin.mailUtilities.validateSpfAsync)
- description and source-code
```javascript
validateSpfAsync = function (_arg0, _arg1, _arg2) {
    'use strict';
    var len = arguments.length;
    var promise = new Promise(INTERNAL);
    promise._captureStackTrace();
    var nodeback = nodebackForPromise(promise);
    var ret;
    var callback = tryCatch(this != null ? this['validateSpf'] : fn);
    switch(len) {
        case 3:ret = callback.call(this, _arg0, _arg1, _arg2, nodeback); break;
case 2:ret = callback.call(this, _arg0, _arg1, nodeback); break;
case 1:ret = callback.call(this, _arg0, nodeback); break;
case 0:ret = callback.call(this, nodeback); break;

default:
    var args = new Array(len + 1);
    var i = 0;
    for (var i = 0; i < len; ++i) {
       args[i] = arguments[i];
    }
    args[i] = nodeback;
    ret = callback.apply(this, args);

    break;

    }
    if (ret === errorObj) {
        promise._rejectCallback(maybeWrapAsError(ret.e), true, true);
    }
    return promise;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
