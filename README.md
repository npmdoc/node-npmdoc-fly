# npmdoc-fly

#### api documentation for  [fly (v2.0.5)](https://github.com/flyjs/fly)  [![npm package](https://img.shields.io/npm/v/npmdoc-fly.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fly) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fly.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fly)

#### Generator & Coroutine-based build system. Fasten your seatbelt.

[![NPM](https://nodei.co/npm/fly.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/fly)

- [https://npmdoc.github.io/node-npmdoc-fly/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-fly/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fly/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fly/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fly/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fly/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jorge Bucaran",
        "url": "https://github.com/jbucaran"
    },
    "bin": {
        "fly": "cli.js"
    },
    "bugs": {
        "url": "https://github.com/flyjs/fly/issues"
    },
    "contributors": [
        {
            "name": "Luke Edwards",
            "url": "https://lukeed.com"
        }
    ],
    "dependencies": {
        "bluebird": "^3.4.7",
        "clor": "^5.0.1",
        "glob": "^7.1.1",
        "minimist": "^1.2.0",
        "mkdirp": "^0.5.1"
    },
    "description": "Generator & Coroutine-based build system. Fasten your seatbelt.",
    "devDependencies": {
        "rimraf": "^2.5.4",
        "tap-spec": "^4.1.1",
        "tape": "^4.6.3"
    },
    "directories": {},
    "dist": {
        "shasum": "5c204bc1740d677eb231feeffc3313d7f5e86961",
        "tarball": "https://registry.npmjs.org/fly/-/fly-2.0.5.tgz"
    },
    "engines": {
        "node": ">= 4.6"
    },
    "files": [
        "lib",
        "cli.js"
    ],
    "gitHead": "802c0e2ab229f2486eb174113123f722fcb32c07",
    "homepage": "https://github.com/flyjs/fly",
    "keywords": [
        "cli",
        "task",
        "build",
        "async",
        "await",
        "minify",
        "uglify",
        "promise",
        "pipeline",
        "generator",
        "coroutine",
        "automation",
        "task runner",
        "build system"
    ],
    "license": "MIT",
    "main": "lib/fly.js",
    "maintainers": [
        {
            "name": "jbucaran"
        },
        {
            "name": "lukeed"
        }
    ],
    "name": "fly",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/flyjs/fly.git"
    },
    "scripts": {
        "test": "tape test/*.js | tap-spec"
    },
    "version": "2.0.5"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
