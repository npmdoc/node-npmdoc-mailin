# npmdoc-mailin

#### api documentation for  [mailin (v3.0.4)](https://github.com/Flolagale/mailin)  [![npm package](https://img.shields.io/npm/v/npmdoc-mailin.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mailin) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mailin.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mailin)

#### Artisanal inbound emails for every web app

[![NPM](https://nodei.co/npm/mailin.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/mailin)

- [https://npmdoc.github.io/node-npmdoc-mailin/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-mailin/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mailin/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mailin/build/apidoc.html)

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
            "name": "flolagale"
        }
    ],
    "name": "mailin",
    "optionalDependencies": {},
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



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
