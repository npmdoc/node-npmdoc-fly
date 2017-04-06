# api documentation for  [fly (v2.0.5)](https://github.com/flyjs/fly)  [![npm package](https://img.shields.io/npm/v/npmdoc-fly.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fly) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fly.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fly)
#### Generator & Coroutine-based build system. Fasten your seatbelt.

[![NPM](https://nodei.co/npm/fly.png?downloads=true)](https://www.npmjs.com/package/fly)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fly/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-fly_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fly/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fly/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fly/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jorge Bucaran",
        "email": "jbucaran@gmail.com",
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
            "email": "luke@lukeed.com",
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
            "name": "jbucaran",
            "email": "jbucaran@gmail.com"
        },
        {
            "name": "lukeed",
            "email": "luke@lukeed.com"
        }
    ],
    "name": "fly",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module fly](#apidoc.module.fly)
1.  [function <span class="apidocSignatureSpan">fly.</span>task (fly)](#apidoc.element.fly.task)
1.  object <span class="apidocSignatureSpan">fly.</span>fmt
1.  object <span class="apidocSignatureSpan">fly.</span>fn
1.  object <span class="apidocSignatureSpan">fly.</span>plugins
1.  object <span class="apidocSignatureSpan">fly.</span>task.prototype

#### [module fly.fmt](#apidoc.module.fly.fmt)
1.  [function <span class="apidocSignatureSpan">fly.fmt.</span>complete {{signature}}](#apidoc.element.fly.fmt.complete)
1.  [function <span class="apidocSignatureSpan">fly.fmt.</span>error {{signature}}](#apidoc.element.fly.fmt.error)
1.  [function <span class="apidocSignatureSpan">fly.fmt.</span>path {{signature}}](#apidoc.element.fly.fmt.path)
1.  [function <span class="apidocSignatureSpan">fly.fmt.</span>text {{signature}}](#apidoc.element.fly.fmt.text)
1.  [function <span class="apidocSignatureSpan">fly.fmt.</span>time {{signature}}](#apidoc.element.fly.fmt.time)
1.  [function <span class="apidocSignatureSpan">fly.fmt.</span>title {{signature}}](#apidoc.element.fly.fmt.title)
1.  [function <span class="apidocSignatureSpan">fly.fmt.</span>warn {{signature}}](#apidoc.element.fly.fmt.warn)

#### [module fly.fn](#apidoc.module.fly.fn)
1.  [function <span class="apidocSignatureSpan">fly.fn.</span>flatten (arr, [])](#apidoc.element.fly.fn.flatten)
1.  [function <span class="apidocSignatureSpan">fly.fn.</span>formatTime (arr[1] / 1000000)](#apidoc.element.fly.fn.formatTime)
1.  [function <span class="apidocSignatureSpan">fly.fn.</span>getTime ()](#apidoc.element.fly.fn.getTime)
1.  [function <span class="apidocSignatureSpan">fly.fn.</span>getUniques (; i < len; i++)](#apidoc.element.fly.fn.getUniques)
1.  [function <span class="apidocSignatureSpan">fly.fn.</span>isEmptyObj (val)](#apidoc.element.fly.fn.isEmptyObj)
1.  [function <span class="apidocSignatureSpan">fly.fn.</span>isObject (val)](#apidoc.element.fly.fn.isObject)
1.  [function <span class="apidocSignatureSpan">fly.fn.</span>toArray (val === null || val === undefined)](#apidoc.element.fly.fn.toArray)
1.  [function <span class="apidocSignatureSpan">fly.fn.</span>valUniq (val, arr)](#apidoc.element.fly.fn.valUniq)

#### [module fly.plugins](#apidoc.module.fly.plugins)
1.  [function <span class="apidocSignatureSpan">fly.plugins.</span>getDependencies (pkg)](#apidoc.element.fly.plugins.getDependencies)
1.  [function <span class="apidocSignatureSpan">fly.plugins.</span>getPackage ()](#apidoc.element.fly.plugins.getPackage)
1.  [function <span class="apidocSignatureSpan">fly.plugins.</span>load ()](#apidoc.element.fly.plugins.load)

#### [module fly.task](#apidoc.module.fly.task)
1.  [function <span class="apidocSignatureSpan">fly.</span>task (fly)](#apidoc.element.fly.task.task)

#### [module fly.task.prototype](#apidoc.module.fly.task.prototype)
1.  [function <span class="apidocSignatureSpan">fly.task.prototype.</span>exec (fn, opts, data)](#apidoc.element.fly.task.prototype.exec)
1.  [function <span class="apidocSignatureSpan">fly.task.prototype.</span>run ()](#apidoc.element.fly.task.prototype.run)
1.  [function <span class="apidocSignatureSpan">fly.task.prototype.</span>source ()](#apidoc.element.fly.task.prototype.source)
1.  [function <span class="apidocSignatureSpan">fly.task.prototype.</span>target ()](#apidoc.element.fly.task.prototype.target)



# <a name="apidoc.module.fly"></a>[module fly](#apidoc.module.fly)

#### <a name="apidoc.element.fly.task"></a>[function <span class="apidocSignatureSpan">fly.</span>task (fly)](#apidoc.element.fly.task)
- description and source-code
```javascript
function Task(fly) {
	// construct shape
	this.$ = util
	this.root = fly.root
	this._ = {files: [], globs: [], prevs: []}
	// attach parent fns to Task
	this.parallel = fly.parallel.bind(fly)
	this.serial = fly.serial.bind(fly)
	this.start = fly.start.bind(fly)
	this.emit = fly.emit.bind(fly)
	// attach 'fly.plugins' to prototype
	for (const k in fly.plugins) {
		this[k] = fly.plugins[k].bind(this)
	}
	// return chained methods + shared
	return boot(this)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fly.fmt"></a>[module fly.fmt](#apidoc.module.fly.fmt)

#### <a name="apidoc.element.fly.fmt.complete"></a>[function <span class="apidocSignatureSpan">fly.fmt.</span>complete {{signature}}](#apidoc.element.fly.fmt.complete)
- description and source-code
```javascript
[34m[1m[22m
```
- example usage
```shell
...

		.on("task_start", str => {
			$.log('Starting ${fmt.title(str)}')
		})

		.on("task_complete", (str, time) => {
			const t = formatTime(time)
			$.log('Finished ${fmt.complete(str)} in ${fmt.time(t)}')
		})

		.on("task_not_found", str => {
			$.log('${fmt.error(str)} not found in Flyfile.')
			process.exit(1)
		})
...
```

#### <a name="apidoc.element.fly.fmt.error"></a>[function <span class="apidocSignatureSpan">fly.fmt.</span>error {{signature}}](#apidoc.element.fly.fmt.error)
- description and source-code
```javascript
[1m[31m[39m
```
- example usage
```shell
...
 */
function getDependencies(pkg) {
	if (!pkg) {
		return []
	}

	if (!isObject(pkg)) {
		$.error("Content from 'package.json' must be an 'Object'!")
		return []
	}

	// get all possible dependencies
	const deps = ["dependencies", "devDependencies", "peerDependencies"]
		.filter(key => key in pkg).map(dep => Object.keys(pkg[dep]))
...
```

#### <a name="apidoc.element.fly.fmt.path"></a>[function <span class="apidocSignatureSpan">fly.fmt.</span>path {{signature}}](#apidoc.element.fly.fmt.path)
- description and source-code
```javascript
[4m[36m[39m
```
- example usage
```shell
...
const fmt = require("./fmt")
const $ = require("./utils/logging")
const formatTime = require("./fn").formatTime

module.exports = function () {
	return this
		.on("fly_run", file => {
			$.log('Flying with ${fmt.path(file)}')
		})

		.on("flyfile_not_found", () => {
			$.log("Flyfile not found!")
			process.exit(1)
		})
...
```

#### <a name="apidoc.element.fly.fmt.text"></a>[function <span class="apidocSignatureSpan">fly.fmt.</span>text {{signature}}](#apidoc.element.fly.fmt.text)
- description and source-code
```javascript
[1m[37m[39m
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fly.fmt.time"></a>[function <span class="apidocSignatureSpan">fly.fmt.</span>time {{signature}}](#apidoc.element.fly.fmt.time)
- description and source-code
```javascript
[32m[39m
```
- example usage
```shell
...

		.on("task_start", str => {
			$.log('Starting ${fmt.title(str)}')
		})

		.on("task_complete", (str, time) => {
			const t = formatTime(time)
			$.log('Finished ${fmt.complete(str)} in ${fmt.time(t)}')
		})

		.on("task_not_found", str => {
			$.log('${fmt.error(str)} not found in Flyfile.')
			process.exit(1)
		})
...
```

#### <a name="apidoc.element.fly.fmt.title"></a>[function <span class="apidocSignatureSpan">fly.fmt.</span>title {{signature}}](#apidoc.element.fly.fmt.title)
- description and source-code
```javascript
[1m[33m[39m
```
- example usage
```shell
...
			let str = '${fmt.warn("Warning:")} Source did not match any files!'
			str += '\n\t  Patterns:   ${JSON.stringify(globs)}'
			opts && (str += '\n\t  Options:    ${JSON.stringify(opts)}')
			$.log(str)
		})

		.on("plugin_load", obj => {
			$.log('Loading plugin ${fmt.title(obj.plugin)}')
		})

		.on("plugin_load_error", str => {
			$.log('Problem loading plugin: ${fmt.title(str)}')
		})

		.on("plugin_rename", (old, nxt) => {
...
```

#### <a name="apidoc.element.fly.fmt.warn"></a>[function <span class="apidocSignatureSpan">fly.fmt.</span>warn {{signature}}](#apidoc.element.fly.fmt.warn)
- description and source-code
```javascript
[1m[35m[39m
```
- example usage
```shell
...

		.on("flyfile_not_found", () => {
			$.log("Flyfile not found!")
			process.exit(1)
		})

		.on("fly_watch", () => {
			$.log('${fmt.warn("Watching files...")}')
		})

		.on("fly_watch_event", obj => {
			$.log('File ${obj.action}: ${fmt.warn(obj.file)}')
		})

		.on("globs_no_match", (globs, opts) => {
...
```



# <a name="apidoc.module.fly.fn"></a>[module fly.fn](#apidoc.module.fly.fn)

#### <a name="apidoc.element.fly.fn.flatten"></a>[function <span class="apidocSignatureSpan">fly.fn.</span>flatten (arr, [])](#apidoc.element.fly.fn.flatten)
- description and source-code
```javascript
arr => flat(arr, [])
```
- example usage
```shell
...
}

Task.prototype.run = co(function * (opts, func) {
	return yield wrapp(opts, func).call(this)
})

Task.prototype.source = co(function * (globs, opts) {
	globs = $.flatten($.toArray(globs))
	const files = yield this.$.expand(globs, opts)

	if (globs.length && !files.length) {
		this.emit("globs_no_match", globs, opts)
	}

	// pre-fetch each file"s content
...
```

#### <a name="apidoc.element.fly.fn.formatTime"></a>[function <span class="apidocSignatureSpan">fly.fn.</span>formatTime (arr[1] / 1000000)](#apidoc.element.fly.fn.formatTime)
- description and source-code
```javascript
arr => {
	let unit = "ms"
	let num = Math.round(arr[1] / 1000000)
	if (arr[0] > 0) {
		unit = "s"
		num = (arr[0] + num / 1000).toFixed(2)
	}
	return '${num}${unit}'
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fly.fn.getTime"></a>[function <span class="apidocSignatureSpan">fly.fn.</span>getTime ()](#apidoc.element.fly.fn.getTime)
- description and source-code
```javascript
() => new Date().toTimeString("UTC").match(/[^\s]+/)[0]
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fly.fn.getUniques"></a>[function <span class="apidocSignatureSpan">fly.fn.</span>getUniques (; i < len; i++)](#apidoc.element.fly.fn.getUniques)
- description and source-code
```javascript
arr => {
	const len = arr.length
	const res = []
	let i = 0

	for (; i < len; i++) {
		const curr = arr[i]
		if (res.indexOf(curr) === -1) {
			res.push(curr)
		}
	}

	return res
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fly.fn.isEmptyObj"></a>[function <span class="apidocSignatureSpan">fly.fn.</span>isEmptyObj (val)](#apidoc.element.fly.fn.isEmptyObj)
- description and source-code
```javascript
val => $.isObject(val) && !Object.keys(val).length
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fly.fn.isObject"></a>[function <span class="apidocSignatureSpan">fly.fn.</span>isObject (val)](#apidoc.element.fly.fn.isObject)
- description and source-code
```javascript
val => Boolean(val) && (val.constructor === Object)
```
- example usage
```shell
...
"use strict"

const $ = exports

// @see http://stackoverflow.com/a/16608074
$.isObject = val => Boolean(val) && (val.constructor === Object)

$.isEmptyObj = val => $.isObject(val) && !Object.keys(val).length

$.toArray = val => (val === null || val === undefined) ? [] : Array.isArray(val) ? val : [val]

/**
* Format a task's duration.
* @param  {Array} arr  Output from 'process.hrtime'
* @return {String}
...
```

#### <a name="apidoc.element.fly.fn.toArray"></a>[function <span class="apidocSignatureSpan">fly.fn.</span>toArray (val === null || val === undefined)](#apidoc.element.fly.fn.toArray)
- description and source-code
```javascript
val => (val === null || val === undefined) ? [] : Array.isArray(val) ? val : [val]
```
- example usage
```shell
...
}

Task.prototype.run = co(function * (opts, func) {
	return yield wrapp(opts, func).call(this)
})

Task.prototype.source = co(function * (globs, opts) {
	globs = $.flatten($.toArray(globs))
	const files = yield this.$.expand(globs, opts)

	if (globs.length && !files.length) {
		this.emit("globs_no_match", globs, opts)
	}

	// pre-fetch each file"s content
...
```

#### <a name="apidoc.element.fly.fn.valUniq"></a>[function <span class="apidocSignatureSpan">fly.fn.</span>valUniq (val, arr)](#apidoc.element.fly.fn.valUniq)
- description and source-code
```javascript
(val, arr) => {
	let n = 0
	let v = val
	while (arr.indexOf(v) !== -1) {
		n++
		v = val.concat(n)
	}
	return v
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fly.plugins"></a>[module fly.plugins](#apidoc.module.fly.plugins)

#### <a name="apidoc.element.fly.plugins.getDependencies"></a>[function <span class="apidocSignatureSpan">fly.plugins.</span>getDependencies (pkg)](#apidoc.element.fly.plugins.getDependencies)
- description and source-code
```javascript
function getDependencies(pkg) {
	if (!pkg) {
		return []
	}

	if (!isObject(pkg)) {
		$.error("Content from 'package.json' must be an 'Object'!")
		return []
	}

	// get all possible dependencies
	const deps = ["dependencies", "devDependencies", "peerDependencies"]
		.filter(key => key in pkg).map(dep => Object.keys(pkg[dep]))

	return flatten(deps)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fly.plugins.getPackage"></a>[function <span class="apidocSignatureSpan">fly.plugins.</span>getPackage ()](#apidoc.element.fly.plugins.getPackage)
- description and source-code
```javascript
getPackage = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    var ret = spawn.promise();
    spawn._generator = generator;
    spawn._promiseFulfilled(undefined);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fly.plugins.load"></a>[function <span class="apidocSignatureSpan">fly.plugins.</span>load ()](#apidoc.element.fly.plugins.load)
- description and source-code
```javascript
load = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    var ret = spawn.promise();
    spawn._generator = generator;
    spawn._promiseFulfilled(undefined);
    return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fly.task"></a>[module fly.task](#apidoc.module.fly.task)

#### <a name="apidoc.element.fly.task.task"></a>[function <span class="apidocSignatureSpan">fly.</span>task (fly)](#apidoc.element.fly.task.task)
- description and source-code
```javascript
function Task(fly) {
	// construct shape
	this.$ = util
	this.root = fly.root
	this._ = {files: [], globs: [], prevs: []}
	// attach parent fns to Task
	this.parallel = fly.parallel.bind(fly)
	this.serial = fly.serial.bind(fly)
	this.start = fly.start.bind(fly)
	this.emit = fly.emit.bind(fly)
	// attach 'fly.plugins' to prototype
	for (const k in fly.plugins) {
		this[k] = fly.plugins[k].bind(this)
	}
	// return chained methods + shared
	return boot(this)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fly.task.prototype"></a>[module fly.task.prototype](#apidoc.module.fly.task.prototype)

#### <a name="apidoc.element.fly.task.prototype.exec"></a>[function <span class="apidocSignatureSpan">fly.task.prototype.</span>exec (fn, opts, data)](#apidoc.element.fly.task.prototype.exec)
- description and source-code
```javascript
exec = function (fn, opts, data) {
	// cache ref to 'fly.tasks[].data' values
	this._ = data
	return fn.call(this, this, opts)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fly.task.prototype.run"></a>[function <span class="apidocSignatureSpan">fly.task.prototype.</span>run ()](#apidoc.element.fly.task.prototype.run)
- description and source-code
```javascript
run = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    var ret = spawn.promise();
    spawn._generator = generator;
    spawn._promiseFulfilled(undefined);
    return ret;
}
```
- example usage
```shell
...

> **Note:** Inline plugins have no need for a second argument in their generator function; you are the "user" here.

See ['task.run'](#taskrunoptions-generator) for a simple example. The same inline example may be written purely as an object:

'''js
exports.foo = function * (fly) {
  yield fly.source("src/*.js").run({
    every: false,
    *func(files) {
      Array.isArray(files) //=> true
      yield Promise.resolve("this will run once.")
    }
  }).target("dist")
}
...
```

#### <a name="apidoc.element.fly.task.prototype.source"></a>[function <span class="apidocSignatureSpan">fly.task.prototype.</span>source ()](#apidoc.element.fly.task.prototype.source)
- description and source-code
```javascript
source = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    var ret = spawn.promise();
    spawn._generator = generator;
    spawn._promiseFulfilled(undefined);
    return ret;
}
```
- example usage
```shell
...
'''js
const sass = "src/{admin,client}/*.sass"
const js = "src/{admin,client}/*.js"
const dist = "build"

module.exports = {
*lint(fly) {
  yield fly.source(js).xo({ esnext: true })
},
*scripts(fly) {
  yield fly.source(js).babel({ presets: ["es2015"] }).target('${dist}/js')
},
*styles(fly) {
  yield fly.source(sass).sass({ outputStyle: "compressed" }).autoprefixer().target('${dist}/css')
},
...
```

#### <a name="apidoc.element.fly.task.prototype.target"></a>[function <span class="apidocSignatureSpan">fly.task.prototype.</span>target ()](#apidoc.element.fly.task.prototype.target)
- description and source-code
```javascript
target = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    var ret = spawn.promise();
    spawn._generator = generator;
    spawn._promiseFulfilled(undefined);
    return ret;
}
```
- example usage
```shell
...
const dist = "build"

module.exports = {
*lint(fly) {
  yield fly.source(js).xo({ esnext: true })
},
*scripts(fly) {
  yield fly.source(js).babel({ presets: ["es2015"] }).target('${dist}/js')
},
*styles(fly) {
  yield fly.source(sass).sass({ outputStyle: "compressed" }).autoprefixer().target('${dist}/css')
},
*build(fly) {
  yield fly.parallel(["lint", "scripts", "styles"])
}
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
