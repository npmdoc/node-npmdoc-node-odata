# api documentation for  [node-odata (v0.7.15)](https://github.com/TossShinHwa/node-odata#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-odata.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-odata) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-odata.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-odata)
#### A module for easily create a REST API based on oData protocol

[![NPM](https://nodei.co/npm/node-odata.png?downloads=true)](https://www.npmjs.com/package/node-odata)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-odata/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-odata_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-odata/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-odata/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-odata/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Zack",
        "email": "zackyang@outlook.com"
    },
    "bugs": {
        "url": "https://github.com/TossShinHwa/node-odata/issues"
    },
    "dependencies": {
        "body-parser": "1.15.2",
        "cors": "2.7.1",
        "express": "4.14.0",
        "method-override": "2.3.6",
        "mongoose": "4.5.9",
        "node-uuid": "1.4.7"
    },
    "description": "A module for easily create a REST API based on oData protocol",
    "devDependencies": {
        "babel": "6.5.2",
        "babel-cli": "6.11.4",
        "babel-core": "6.13.2",
        "babel-eslint": "6.1.2",
        "babel-helpers": "6.8.0",
        "babel-loader": "6.2.4",
        "babel-plugin-transform-decorators-legacy": "1.3.4",
        "babel-polyfill": "6.13.0",
        "babel-preset-es2015": "6.13.2",
        "babel-preset-stage-0": "6.5.0",
        "babel-register": "6.11.6",
        "babel-runtime": "6.11.6",
        "eslint": "3.3.1",
        "eslint-config-airbnb": "10.0.1",
        "eslint-plugin-babel": "3.3.0",
        "istanbul": "1.0.0-alpha.2",
        "mocha": "3.0.2",
        "should": "11.1.0",
        "should-sinon": "0.0.5",
        "sinon": "1.17.5",
        "supertest": "2.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "04b06d897598a571d39de5f9e3d4996de602d50a",
        "tarball": "https://registry.npmjs.org/node-odata/-/node-odata-0.7.15.tgz"
    },
    "engines": {
        "node": ">=0.12"
    },
    "gitHead": "e3af9d5c17353b9d7985ae55ec2aa7b4b2f89ebf",
    "homepage": "https://github.com/TossShinHwa/node-odata#readme",
    "keywords": [
        "OData",
        "REST",
        "RESTful"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "zackyang",
            "email": "zackyang@outlook.com"
        }
    ],
    "name": "node-odata",
    "optionalDependencies": {},
    "private": false,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/TossShinHwa/node-odata.git"
    },
    "scripts": {
        "prepublish": "make",
        "test": "make"
    },
    "version": "0.7.15"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-odata](#apidoc.module.node-odata)
1.  [function <span class="apidocSignatureSpan">node-odata.</span>Function ()](#apidoc.element.node-odata.Function)
1.  [function <span class="apidocSignatureSpan">node-odata.</span>Resource (name, model)](#apidoc.element.node-odata.Resource)
1.  [function <span class="apidocSignatureSpan">node-odata.</span>_express ()](#apidoc.element.node-odata._express)
1.  [function <span class="apidocSignatureSpan">node-odata.</span>_express.Route (path)](#apidoc.element.node-odata._express.Route)
1.  [function <span class="apidocSignatureSpan">node-odata.</span>_express.Router (options)](#apidoc.element.node-odata._express.Router)
1.  object <span class="apidocSignatureSpan">node-odata.</span>ODataFunction
1.  object <span class="apidocSignatureSpan">node-odata.</span>ODataResource
1.  object <span class="apidocSignatureSpan">node-odata.</span>_express.Route.prototype
1.  object <span class="apidocSignatureSpan">node-odata.</span>_express.application
1.  object <span class="apidocSignatureSpan">node-odata.</span>_express.request
1.  object <span class="apidocSignatureSpan">node-odata.</span>_express.response
1.  object <span class="apidocSignatureSpan">node-odata.</span>express
1.  object <span class="apidocSignatureSpan">node-odata.</span>server
1.  object <span class="apidocSignatureSpan">node-odata.</span>utils

#### [module node-odata.ODataFunction](#apidoc.module.node-odata.ODataFunction)
1.  [function <span class="apidocSignatureSpan">node-odata.ODataFunction.</span>default ()](#apidoc.element.node-odata.ODataFunction.default)

#### [module node-odata.ODataResource](#apidoc.module.node-odata.ODataResource)
1.  [function <span class="apidocSignatureSpan">node-odata.ODataResource.</span>default (name, userModel)](#apidoc.element.node-odata.ODataResource.default)

#### [module node-odata._express](#apidoc.module.node-odata._express)
1.  [function <span class="apidocSignatureSpan">node-odata.</span>_express ()](#apidoc.element.node-odata._express._express)
1.  [function <span class="apidocSignatureSpan">node-odata._express.</span>Route (path)](#apidoc.element.node-odata._express.Route)
1.  [function <span class="apidocSignatureSpan">node-odata._express.</span>Router (options)](#apidoc.element.node-odata._express.Router)
1.  [function <span class="apidocSignatureSpan">node-odata._express.</span>query (options)](#apidoc.element.node-odata._express.query)
1.  [function <span class="apidocSignatureSpan">node-odata._express.</span>static (root, options)](#apidoc.element.node-odata._express.static)
1.  object <span class="apidocSignatureSpan">node-odata._express.</span>application
1.  object <span class="apidocSignatureSpan">node-odata._express.</span>request
1.  object <span class="apidocSignatureSpan">node-odata._express.</span>response

#### [module node-odata._express.Route](#apidoc.module.node-odata._express.Route)
1.  [function <span class="apidocSignatureSpan">node-odata._express.</span>Route (path)](#apidoc.element.node-odata._express.Route.Route)

#### [module node-odata._express.Route.prototype](#apidoc.module.node-odata._express.Route.prototype)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>_handles_method (method)](#apidoc.element.node-odata._express.Route.prototype._handles_method)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>_options ()](#apidoc.element.node-odata._express.Route.prototype._options)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>acl ()](#apidoc.element.node-odata._express.Route.prototype.acl)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>all ()](#apidoc.element.node-odata._express.Route.prototype.all)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>bind ()](#apidoc.element.node-odata._express.Route.prototype.bind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>checkout ()](#apidoc.element.node-odata._express.Route.prototype.checkout)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>connect ()](#apidoc.element.node-odata._express.Route.prototype.connect)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>copy ()](#apidoc.element.node-odata._express.Route.prototype.copy)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>delete ()](#apidoc.element.node-odata._express.Route.prototype.delete)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>dispatch (req, res, done)](#apidoc.element.node-odata._express.Route.prototype.dispatch)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>get ()](#apidoc.element.node-odata._express.Route.prototype.get)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>head ()](#apidoc.element.node-odata._express.Route.prototype.head)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>link ()](#apidoc.element.node-odata._express.Route.prototype.link)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>lock ()](#apidoc.element.node-odata._express.Route.prototype.lock)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>m-search ()](#apidoc.element.node-odata._express.Route.prototype.m-search)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>merge ()](#apidoc.element.node-odata._express.Route.prototype.merge)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>mkactivity ()](#apidoc.element.node-odata._express.Route.prototype.mkactivity)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>mkcalendar ()](#apidoc.element.node-odata._express.Route.prototype.mkcalendar)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>mkcol ()](#apidoc.element.node-odata._express.Route.prototype.mkcol)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>move ()](#apidoc.element.node-odata._express.Route.prototype.move)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>notify ()](#apidoc.element.node-odata._express.Route.prototype.notify)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>options ()](#apidoc.element.node-odata._express.Route.prototype.options)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>patch ()](#apidoc.element.node-odata._express.Route.prototype.patch)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>post ()](#apidoc.element.node-odata._express.Route.prototype.post)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>propfind ()](#apidoc.element.node-odata._express.Route.prototype.propfind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>proppatch ()](#apidoc.element.node-odata._express.Route.prototype.proppatch)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>purge ()](#apidoc.element.node-odata._express.Route.prototype.purge)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>put ()](#apidoc.element.node-odata._express.Route.prototype.put)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>rebind ()](#apidoc.element.node-odata._express.Route.prototype.rebind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>report ()](#apidoc.element.node-odata._express.Route.prototype.report)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>search ()](#apidoc.element.node-odata._express.Route.prototype.search)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>subscribe ()](#apidoc.element.node-odata._express.Route.prototype.subscribe)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>trace ()](#apidoc.element.node-odata._express.Route.prototype.trace)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>unbind ()](#apidoc.element.node-odata._express.Route.prototype.unbind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>unlink ()](#apidoc.element.node-odata._express.Route.prototype.unlink)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>unlock ()](#apidoc.element.node-odata._express.Route.prototype.unlock)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>unsubscribe ()](#apidoc.element.node-odata._express.Route.prototype.unsubscribe)

#### [module node-odata._express.Router](#apidoc.module.node-odata._express.Router)
1.  [function <span class="apidocSignatureSpan">node-odata._express.</span>Router (options)](#apidoc.element.node-odata._express.Router.Router)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>acl (path)](#apidoc.element.node-odata._express.Router.acl)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>all (path)](#apidoc.element.node-odata._express.Router.all)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>bind (path)](#apidoc.element.node-odata._express.Router.bind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>checkout (path)](#apidoc.element.node-odata._express.Router.checkout)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>connect (path)](#apidoc.element.node-odata._express.Router.connect)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>copy (path)](#apidoc.element.node-odata._express.Router.copy)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>delete (path)](#apidoc.element.node-odata._express.Router.delete)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>get (path)](#apidoc.element.node-odata._express.Router.get)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>handle (req, res, out)](#apidoc.element.node-odata._express.Router.handle)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>head (path)](#apidoc.element.node-odata._express.Router.head)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>link (path)](#apidoc.element.node-odata._express.Router.link)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>lock (path)](#apidoc.element.node-odata._express.Router.lock)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>m-search (path)](#apidoc.element.node-odata._express.Router.m-search)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>merge (path)](#apidoc.element.node-odata._express.Router.merge)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>mkactivity (path)](#apidoc.element.node-odata._express.Router.mkactivity)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>mkcalendar (path)](#apidoc.element.node-odata._express.Router.mkcalendar)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>mkcol (path)](#apidoc.element.node-odata._express.Router.mkcol)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>move (path)](#apidoc.element.node-odata._express.Router.move)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>notify (path)](#apidoc.element.node-odata._express.Router.notify)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>options (path)](#apidoc.element.node-odata._express.Router.options)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>param (name, fn)](#apidoc.element.node-odata._express.Router.param)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>patch (path)](#apidoc.element.node-odata._express.Router.patch)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>post (path)](#apidoc.element.node-odata._express.Router.post)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>process_params (layer, called, req, res, done)](#apidoc.element.node-odata._express.Router.process_params)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>propfind (path)](#apidoc.element.node-odata._express.Router.propfind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>proppatch (path)](#apidoc.element.node-odata._express.Router.proppatch)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>purge (path)](#apidoc.element.node-odata._express.Router.purge)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>put (path)](#apidoc.element.node-odata._express.Router.put)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>rebind (path)](#apidoc.element.node-odata._express.Router.rebind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>report (path)](#apidoc.element.node-odata._express.Router.report)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>route (path)](#apidoc.element.node-odata._express.Router.route)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>search (path)](#apidoc.element.node-odata._express.Router.search)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>subscribe (path)](#apidoc.element.node-odata._express.Router.subscribe)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>trace (path)](#apidoc.element.node-odata._express.Router.trace)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>unbind (path)](#apidoc.element.node-odata._express.Router.unbind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>unlink (path)](#apidoc.element.node-odata._express.Router.unlink)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>unlock (path)](#apidoc.element.node-odata._express.Router.unlock)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>unsubscribe (path)](#apidoc.element.node-odata._express.Router.unsubscribe)
1.  [function <span class="apidocSignatureSpan">node-odata._express.Router.</span>use (fn)](#apidoc.element.node-odata._express.Router.use)

#### [module node-odata._express.application](#apidoc.module.node-odata._express.application)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>acl (path)](#apidoc.element.node-odata._express.application.acl)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>all (path)](#apidoc.element.node-odata._express.application.all)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>bind (path)](#apidoc.element.node-odata._express.application.bind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>checkout (path)](#apidoc.element.node-odata._express.application.checkout)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>connect (path)](#apidoc.element.node-odata._express.application.connect)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>copy (path)](#apidoc.element.node-odata._express.application.copy)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>defaultConfiguration ()](#apidoc.element.node-odata._express.application.defaultConfiguration)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>del (arg0)](#apidoc.element.node-odata._express.application.del)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>delete (path)](#apidoc.element.node-odata._express.application.delete)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>disable (setting)](#apidoc.element.node-odata._express.application.disable)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>disabled (setting)](#apidoc.element.node-odata._express.application.disabled)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>enable (setting)](#apidoc.element.node-odata._express.application.enable)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>enabled (setting)](#apidoc.element.node-odata._express.application.enabled)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>engine (ext, fn)](#apidoc.element.node-odata._express.application.engine)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>get (path)](#apidoc.element.node-odata._express.application.get)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>handle (req, res, callback)](#apidoc.element.node-odata._express.application.handle)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>head (path)](#apidoc.element.node-odata._express.application.head)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>init ()](#apidoc.element.node-odata._express.application.init)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>lazyrouter ()](#apidoc.element.node-odata._express.application.lazyrouter)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>link (path)](#apidoc.element.node-odata._express.application.link)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>listen ()](#apidoc.element.node-odata._express.application.listen)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>lock (path)](#apidoc.element.node-odata._express.application.lock)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>m-search (path)](#apidoc.element.node-odata._express.application.m-search)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>merge (path)](#apidoc.element.node-odata._express.application.merge)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>mkactivity (path)](#apidoc.element.node-odata._express.application.mkactivity)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>mkcalendar (path)](#apidoc.element.node-odata._express.application.mkcalendar)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>mkcol (path)](#apidoc.element.node-odata._express.application.mkcol)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>move (path)](#apidoc.element.node-odata._express.application.move)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>notify (path)](#apidoc.element.node-odata._express.application.notify)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>options (path)](#apidoc.element.node-odata._express.application.options)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>param (name, fn)](#apidoc.element.node-odata._express.application.param)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>patch (path)](#apidoc.element.node-odata._express.application.patch)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>path ()](#apidoc.element.node-odata._express.application.path)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>post (path)](#apidoc.element.node-odata._express.application.post)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>propfind (path)](#apidoc.element.node-odata._express.application.propfind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>proppatch (path)](#apidoc.element.node-odata._express.application.proppatch)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>purge (path)](#apidoc.element.node-odata._express.application.purge)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>put (path)](#apidoc.element.node-odata._express.application.put)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>rebind (path)](#apidoc.element.node-odata._express.application.rebind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>render (name, options, callback)](#apidoc.element.node-odata._express.application.render)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>report (path)](#apidoc.element.node-odata._express.application.report)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>route (path)](#apidoc.element.node-odata._express.application.route)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>search (path)](#apidoc.element.node-odata._express.application.search)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>set (setting, val)](#apidoc.element.node-odata._express.application.set)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>subscribe (path)](#apidoc.element.node-odata._express.application.subscribe)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>trace (path)](#apidoc.element.node-odata._express.application.trace)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>unbind (path)](#apidoc.element.node-odata._express.application.unbind)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>unlink (path)](#apidoc.element.node-odata._express.application.unlink)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>unlock (path)](#apidoc.element.node-odata._express.application.unlock)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>unsubscribe (path)](#apidoc.element.node-odata._express.application.unsubscribe)
1.  [function <span class="apidocSignatureSpan">node-odata._express.application.</span>use (fn)](#apidoc.element.node-odata._express.application.use)

#### [module node-odata._express.request](#apidoc.module.node-odata._express.request)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>accepts ()](#apidoc.element.node-odata._express.request.accepts)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsCharset ()](#apidoc.element.node-odata._express.request.acceptsCharset)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsCharsets ()](#apidoc.element.node-odata._express.request.acceptsCharsets)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsEncoding ()](#apidoc.element.node-odata._express.request.acceptsEncoding)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsEncodings ()](#apidoc.element.node-odata._express.request.acceptsEncodings)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsLanguage ()](#apidoc.element.node-odata._express.request.acceptsLanguage)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsLanguages ()](#apidoc.element.node-odata._express.request.acceptsLanguages)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>get (name)](#apidoc.element.node-odata._express.request.get)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>header (name)](#apidoc.element.node-odata._express.request.header)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>is (types)](#apidoc.element.node-odata._express.request.is)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>param (name, defaultValue)](#apidoc.element.node-odata._express.request.param)
1.  [function <span class="apidocSignatureSpan">node-odata._express.request.</span>range (size, options)](#apidoc.element.node-odata._express.request.range)

#### [module node-odata._express.response](#apidoc.module.node-odata._express.response)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>append (field, val)](#apidoc.element.node-odata._express.response.append)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>attachment (filename)](#apidoc.element.node-odata._express.response.attachment)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>clearCookie (name, options)](#apidoc.element.node-odata._express.response.clearCookie)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>contentType (type)](#apidoc.element.node-odata._express.response.contentType)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>cookie (name, value, options)](#apidoc.element.node-odata._express.response.cookie)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>download (path, filename, callback)](#apidoc.element.node-odata._express.response.download)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>format (obj)](#apidoc.element.node-odata._express.response.format)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>get (field)](#apidoc.element.node-odata._express.response.get)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>header (field, val)](#apidoc.element.node-odata._express.response.header)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>json (obj)](#apidoc.element.node-odata._express.response.json)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>jsonp (obj)](#apidoc.element.node-odata._express.response.jsonp)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>links (links)](#apidoc.element.node-odata._express.response.links)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>location (url)](#apidoc.element.node-odata._express.response.location)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>redirect (url)](#apidoc.element.node-odata._express.response.redirect)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>render (view, options, callback)](#apidoc.element.node-odata._express.response.render)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>send (body)](#apidoc.element.node-odata._express.response.send)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>sendFile (path, options, callback)](#apidoc.element.node-odata._express.response.sendFile)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>sendStatus (statusCode)](#apidoc.element.node-odata._express.response.sendStatus)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>sendfile (arg0, arg1, arg2)](#apidoc.element.node-odata._express.response.sendfile)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>set (field, val)](#apidoc.element.node-odata._express.response.set)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>status (code)](#apidoc.element.node-odata._express.response.status)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>type (type)](#apidoc.element.node-odata._express.response.type)
1.  [function <span class="apidocSignatureSpan">node-odata._express.response.</span>vary (field)](#apidoc.element.node-odata._express.response.vary)

#### [module node-odata.express](#apidoc.module.node-odata.express)
1.  [function <span class="apidocSignatureSpan">node-odata.express.</span>default ()](#apidoc.element.node-odata.express.default)

#### [module node-odata.server](#apidoc.module.node-odata.server)
1.  [function <span class="apidocSignatureSpan">node-odata.server.</span>default (db, prefix)](#apidoc.element.node-odata.server.default)

#### [module node-odata.utils](#apidoc.module.node-odata.utils)
1.  [function <span class="apidocSignatureSpan">node-odata.utils.</span>min (arr)](#apidoc.element.node-odata.utils.min)
1.  [function <span class="apidocSignatureSpan">node-odata.utils.</span>split (sentence)](#apidoc.element.node-odata.utils.split)



# <a name="apidoc.module.node-odata"></a>[module node-odata](#apidoc.module.node-odata)

#### <a name="apidoc.element.node-odata.Function"></a>[function <span class="apidocSignatureSpan">node-odata.</span>Function ()](#apidoc.element.node-odata.Function)
- description and source-code
```javascript
function createFunction() {
  return new _ODataFunction2.default();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata.Resource"></a>[function <span class="apidocSignatureSpan">node-odata.</span>Resource (name, model)](#apidoc.element.node-odata.Resource)
- description and source-code
```javascript
function createResouce(name, model) {
  return new _ODataResource2.default(name, model);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express"></a>[function <span class="apidocSignatureSpan">node-odata.</span>_express ()](#apidoc.element.node-odata._express)
- description and source-code
```javascript
function createApplication() {
  var app = function(req, res, next) {
    app.handle(req, res, next);
  };

  mixin(app, EventEmitter.prototype, false);
  mixin(app, proto, false);

  app.request = { __proto__: req, app: app };
  app.response = { __proto__: res, app: app };
  app.init();
  return app;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route"></a>[function <span class="apidocSignatureSpan">node-odata.</span>_express.Route (path)](#apidoc.element.node-odata._express.Route)
- description and source-code
```javascript
function Route(path) {
  this.path = path;
  this.stack = [];

  debug('new %s', path);

  // route handlers for various http methods
  this.methods = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router"></a>[function <span class="apidocSignatureSpan">node-odata.</span>_express.Router (options)](#apidoc.element.node-odata._express.Router)
- description and source-code
```javascript
_express.Router = function (options) {
  var opts = options || {};

  function router(req, res, next) {
    router.handle(req, res, next);
  }

  // mixin Router class functions
  router.__proto__ = proto;

  router.params = {};
  router._params = [];
  router.caseSensitive = opts.caseSensitive;
  router.mergeParams = opts.mergeParams;
  router.strict = opts.strict;
  router.stack = [];

  return router;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-odata.ODataFunction"></a>[module node-odata.ODataFunction](#apidoc.module.node-odata.ODataFunction)

#### <a name="apidoc.element.node-odata.ODataFunction.default"></a>[function <span class="apidocSignatureSpan">node-odata.ODataFunction.</span>default ()](#apidoc.element.node-odata.ODataFunction.default)
- description and source-code
```javascript
function _default() {
  _classCallCheck(this, _default);

<span class="apidocCodeCommentSpan">  /*eslint-disable */
</span>  return _express2.default.Router();
  /*eslint-enable */
}
```
- example usage
```shell
...
  }
}, {
  key: 'resource',
  value: function resource(name, model) {
    if (model === undefined) {
      return this._resources.name;
    }
    var resource = new _ODataResource2.default(name, model);
    this._resources.push(resource);
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
...
```



# <a name="apidoc.module.node-odata.ODataResource"></a>[module node-odata.ODataResource](#apidoc.module.node-odata.ODataResource)

#### <a name="apidoc.element.node-odata.ODataResource.default"></a>[function <span class="apidocSignatureSpan">node-odata.ODataResource.</span>default (name, userModel)](#apidoc.element.node-odata.ODataResource.default)
- description and source-code
```javascript
function _default(name, userModel) {
  _classCallCheck(this, _default);

  this._name = name;
  this._url = name;
  this._model = userModel;
  this._hooks = {
    list: {},
    get: {},
    post: {},
    put: {},
    delete: {},
    patch: {}
  };
  this._actions = {};
  this._options = {
    maxTop: 10000,
    maxSkip: 10000,
    orderby: undefined
  };
}
```
- example usage
```shell
...
  }
}, {
  key: 'resource',
  value: function resource(name, model) {
    if (model === undefined) {
      return this._resources.name;
    }
    var resource = new _ODataResource2.default(name, model);
    this._resources.push(resource);
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
...
```



# <a name="apidoc.module.node-odata._express"></a>[module node-odata._express](#apidoc.module.node-odata._express)

#### <a name="apidoc.element.node-odata._express._express"></a>[function <span class="apidocSignatureSpan">node-odata.</span>_express ()](#apidoc.element.node-odata._express._express)
- description and source-code
```javascript
function createApplication() {
  var app = function(req, res, next) {
    app.handle(req, res, next);
  };

  mixin(app, EventEmitter.prototype, false);
  mixin(app, proto, false);

  app.request = { __proto__: req, app: app };
  app.response = { __proto__: res, app: app };
  app.init();
  return app;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route"></a>[function <span class="apidocSignatureSpan">node-odata._express.</span>Route (path)](#apidoc.element.node-odata._express.Route)
- description and source-code
```javascript
function Route(path) {
  this.path = path;
  this.stack = [];

  debug('new %s', path);

  // route handlers for various http methods
  this.methods = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router"></a>[function <span class="apidocSignatureSpan">node-odata._express.</span>Router (options)](#apidoc.element.node-odata._express.Router)
- description and source-code
```javascript
Router = function (options) {
  var opts = options || {};

  function router(req, res, next) {
    router.handle(req, res, next);
  }

  // mixin Router class functions
  router.__proto__ = proto;

  router.params = {};
  router._params = [];
  router.caseSensitive = opts.caseSensitive;
  router.mergeParams = opts.mergeParams;
  router.strict = opts.strict;
  router.stack = [];

  return router;
}
```
- example usage
```shell
...

function _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError("Cannot call a class
 as a function"); } }

var _default = function _default() {
  _classCallCheck(this, _default);

  /*eslint-disable */
  return _express2.default.Router();
  /*eslint-enable */
};

exports.default = _default;
...
```

#### <a name="apidoc.element.node-odata._express.query"></a>[function <span class="apidocSignatureSpan">node-odata._express.</span>query (options)](#apidoc.element.node-odata._express.query)
- description and source-code
```javascript
function query(options) {
  var opts = Object.create(options || null);
  var queryparse = qs.parse;

  if (typeof options === 'function') {
    queryparse = options;
    opts = undefined;
  }

  if (opts !== undefined && opts.allowPrototypes === undefined) {
    // back-compat for qs module
    opts.allowPrototypes = true;
  }

  return function query(req, res, next){
    if (!req.query) {
      var val = parseUrl(req).query;
      req.query = queryparse(val, opts);
    }

    next();
  };
}
```
- example usage
```shell
...
});

exports.default = function () {
  var app = (0, _express2.default)();
  app.use(_bodyParser2.default.urlencoded({ extended: true }));
  app.use(_bodyParser2.default.json());
  app.use((0, _methodOverride2.default)());
  app.use(_express2.default.query());
  app.use((0, _cors2.default)());
  app.disable('x-powered-by');
  return app;
};

var _express = require('express');
...
```

#### <a name="apidoc.element.node-odata._express.static"></a>[function <span class="apidocSignatureSpan">node-odata._express.</span>static (root, options)](#apidoc.element.node-odata._express.static)
- description and source-code
```javascript
function serveStatic(root, options) {
  if (!root) {
    throw new TypeError('root path required')
  }

  if (typeof root !== 'string') {
    throw new TypeError('root path must be a string')
  }

  // copy options object
  var opts = Object.create(options || null)

  // fall-though
  var fallthrough = opts.fallthrough !== false

  // default redirect
  var redirect = opts.redirect !== false

  // headers listener
  var setHeaders = opts.setHeaders

  if (setHeaders && typeof setHeaders !== 'function') {
    throw new TypeError('option setHeaders must be function')
  }

  // setup options for send
  opts.maxage = opts.maxage || opts.maxAge || 0
  opts.root = resolve(root)

  // construct directory listener
  var onDirectory = redirect
    ? createRedirectDirectoryListener()
    : createNotFoundDirectoryListener()

  return function serveStatic (req, res, next) {
    if (req.method !== 'GET' && req.method !== 'HEAD') {
      if (fallthrough) {
        return next()
      }

      // method not allowed
      res.statusCode = 405
      res.setHeader('Allow', 'GET, HEAD')
      res.setHeader('Content-Length', '0')
      res.end()
      return
    }

    var forwardError = !fallthrough
    var originalUrl = parseUrl.original(req)
    var path = parseUrl(req).pathname

    // make sure redirect occurs at mount
    if (path === '/' && originalUrl.pathname.substr(-1) !== '/') {
      path = ''
    }

    // create send stream
    var stream = send(req, path, opts)

    // add directory handler
    stream.on('directory', onDirectory)

    // add headers listener
    if (setHeaders) {
      stream.on('headers', setHeaders)
    }

    // add file listener for fallthrough
    if (fallthrough) {
      stream.on('file', function onFile () {
        // once file is determined, always forward error
        forwardError = true
      })
    }

    // forward errors
    stream.on('error', function error (err) {
      if (forwardError || !(err.statusCode < 500)) {
        next(err)
        return
      }

      next()
    })

    // pipe
    stream.pipe(res)
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-odata._express.Route"></a>[module node-odata._express.Route](#apidoc.module.node-odata._express.Route)

#### <a name="apidoc.element.node-odata._express.Route.Route"></a>[function <span class="apidocSignatureSpan">node-odata._express.</span>Route (path)](#apidoc.element.node-odata._express.Route.Route)
- description and source-code
```javascript
function Route(path) {
  this.path = path;
  this.stack = [];

  debug('new %s', path);

  // route handlers for various http methods
  this.methods = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-odata._express.Route.prototype"></a>[module node-odata._express.Route.prototype](#apidoc.module.node-odata._express.Route.prototype)

#### <a name="apidoc.element.node-odata._express.Route.prototype._handles_method"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>_handles_method (method)](#apidoc.element.node-odata._express.Route.prototype._handles_method)
- description and source-code
```javascript
function _handles_method(method) {
  if (this.methods._all) {
    return true;
  }

  var name = method.toLowerCase();

  if (name === 'head' && !this.methods['head']) {
    name = 'get';
  }

  return Boolean(this.methods[name]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype._options"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>_options ()](#apidoc.element.node-odata._express.Route.prototype._options)
- description and source-code
```javascript
function _options() {
  var methods = Object.keys(this.methods);

  // append automatic head
  if (this.methods.get && !this.methods.head) {
    methods.push('head');
  }

  for (var i = 0; i < methods.length; i++) {
    // make upper case
    methods[i] = methods[i].toUpperCase();
  }

  return methods;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.acl"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>acl ()](#apidoc.element.node-odata._express.Route.prototype.acl)
- description and source-code
```javascript
acl = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.all"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>all ()](#apidoc.element.node-odata._express.Route.prototype.all)
- description and source-code
```javascript
function all() {
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.all() requires callback functions but got a ' + type;
      throw new TypeError(msg);
    }

    var layer = Layer('/', {}, handle);
    layer.method = undefined;

    this.methods._all = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.bind"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>bind ()](#apidoc.element.node-odata._express.Route.prototype.bind)
- description and source-code
```javascript
bind = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.checkout"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>checkout ()](#apidoc.element.node-odata._express.Route.prototype.checkout)
- description and source-code
```javascript
checkout = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.connect"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>connect ()](#apidoc.element.node-odata._express.Route.prototype.connect)
- description and source-code
```javascript
connect = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.copy"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>copy ()](#apidoc.element.node-odata._express.Route.prototype.copy)
- description and source-code
```javascript
copy = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.delete"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>delete ()](#apidoc.element.node-odata._express.Route.prototype.delete)
- description and source-code
```javascript
delete = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
...
    });
  }
}, {
  key: 'delete',
  value: function _delete(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.delete('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>dispatch (req, res, done)](#apidoc.element.node-odata._express.Route.prototype.dispatch)
- description and source-code
```javascript
function dispatch(req, res, done) {
  var idx = 0;
  var stack = this.stack;
  if (stack.length === 0) {
    return done();
  }

  var method = req.method.toLowerCase();
  if (method === 'head' && !this.methods['head']) {
    method = 'get';
  }

  req.route = this;

  next();

  function next(err) {
    if (err && err === 'route') {
      return done();
    }

    var layer = stack[idx++];
    if (!layer) {
      return done(err);
    }

    if (layer.method && layer.method !== method) {
      return next(err);
    }

    if (err) {
      layer.handle_error(err, req, res, next);
    } else {
      layer.handle_request(req, res, next);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.get"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>get ()](#apidoc.element.node-odata._express.Route.prototype.get)
- description and source-code
```javascript
get = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
...
    var resource = new _ODataResource2.default(name, model);
    this._resources.push(resource);
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.post('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
...
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.head"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>head ()](#apidoc.element.node-odata._express.Route.prototype.head)
- description and source-code
```javascript
head = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.link"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>link ()](#apidoc.element.node-odata._express.Route.prototype.link)
- description and source-code
```javascript
link = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.lock"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>lock ()](#apidoc.element.node-odata._express.Route.prototype.lock)
- description and source-code
```javascript
lock = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.m-search"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>m-search ()](#apidoc.element.node-odata._express.Route.prototype.m-search)
- description and source-code
```javascript
m-search = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.merge"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>merge ()](#apidoc.element.node-odata._express.Route.prototype.merge)
- description and source-code
```javascript
merge = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.mkactivity"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>mkactivity ()](#apidoc.element.node-odata._express.Route.prototype.mkactivity)
- description and source-code
```javascript
mkactivity = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.mkcalendar"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>mkcalendar ()](#apidoc.element.node-odata._express.Route.prototype.mkcalendar)
- description and source-code
```javascript
mkcalendar = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.mkcol"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>mkcol ()](#apidoc.element.node-odata._express.Route.prototype.mkcol)
- description and source-code
```javascript
mkcol = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.move"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>move ()](#apidoc.element.node-odata._express.Route.prototype.move)
- description and source-code
```javascript
move = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.notify"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>notify ()](#apidoc.element.node-odata._express.Route.prototype.notify)
- description and source-code
```javascript
notify = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.options"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>options ()](#apidoc.element.node-odata._express.Route.prototype.options)
- description and source-code
```javascript
options = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.patch"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>patch ()](#apidoc.element.node-odata._express.Route.prototype.patch)
- description and source-code
```javascript
patch = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
...
    });
  }
}, {
  key: 'patch',
  value: function patch(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.patch('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.post"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>post ()](#apidoc.element.node-odata._express.Route.prototype.post)
- description and source-code
```javascript
post = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
...
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.post('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.propfind"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>propfind ()](#apidoc.element.node-odata._express.Route.prototype.propfind)
- description and source-code
```javascript
propfind = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.proppatch"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>proppatch ()](#apidoc.element.node-odata._express.Route.prototype.proppatch)
- description and source-code
```javascript
proppatch = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.purge"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>purge ()](#apidoc.element.node-odata._express.Route.prototype.purge)
- description and source-code
```javascript
purge = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.put"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>put ()](#apidoc.element.node-odata._express.Route.prototype.put)
- description and source-code
```javascript
put = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
...
    });
  }
}, {
  key: 'put',
  value: function put(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.put('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.rebind"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>rebind ()](#apidoc.element.node-odata._express.Route.prototype.rebind)
- description and source-code
```javascript
rebind = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.report"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>report ()](#apidoc.element.node-odata._express.Route.prototype.report)
- description and source-code
```javascript
report = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.search"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>search ()](#apidoc.element.node-odata._express.Route.prototype.search)
- description and source-code
```javascript
search = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.subscribe"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>subscribe ()](#apidoc.element.node-odata._express.Route.prototype.subscribe)
- description and source-code
```javascript
subscribe = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.trace"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>trace ()](#apidoc.element.node-odata._express.Route.prototype.trace)
- description and source-code
```javascript
trace = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.unbind"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>unbind ()](#apidoc.element.node-odata._express.Route.prototype.unbind)
- description and source-code
```javascript
unbind = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.unlink"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>unlink ()](#apidoc.element.node-odata._express.Route.prototype.unlink)
- description and source-code
```javascript
unlink = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.unlock"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>unlock ()](#apidoc.element.node-odata._express.Route.prototype.unlock)
- description and source-code
```javascript
unlock = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Route.prototype.unsubscribe"></a>[function <span class="apidocSignatureSpan">node-odata._express.Route.prototype.</span>unsubscribe ()](#apidoc.element.node-odata._express.Route.prototype.unsubscribe)
- description and source-code
```javascript
unsubscribe = function (){
  var handles = flatten(slice.call(arguments));

  for (var i = 0; i < handles.length; i++) {
    var handle = handles[i];

    if (typeof handle !== 'function') {
      var type = toString.call(handle);
      var msg = 'Route.' + method + '() requires callback functions but got a ' + type;
      throw new Error(msg);
    }

    debug('%s %s', method, this.path);

    var layer = Layer('/', {}, handle);
    layer.method = method;

    this.methods[method] = true;
    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-odata._express.Router"></a>[module node-odata._express.Router](#apidoc.module.node-odata._express.Router)

#### <a name="apidoc.element.node-odata._express.Router.Router"></a>[function <span class="apidocSignatureSpan">node-odata._express.</span>Router (options)](#apidoc.element.node-odata._express.Router.Router)
- description and source-code
```javascript
Router = function (options) {
  var opts = options || {};

  function router(req, res, next) {
    router.handle(req, res, next);
  }

  // mixin Router class functions
  router.__proto__ = proto;

  router.params = {};
  router._params = [];
  router.caseSensitive = opts.caseSensitive;
  router.mergeParams = opts.mergeParams;
  router.strict = opts.strict;
  router.stack = [];

  return router;
}
```
- example usage
```shell
...

function _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError("Cannot call a class
 as a function"); } }

var _default = function _default() {
  _classCallCheck(this, _default);

  /*eslint-disable */
  return _express2.default.Router();
  /*eslint-enable */
};

exports.default = _default;
...
```

#### <a name="apidoc.element.node-odata._express.Router.acl"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>acl (path)](#apidoc.element.node-odata._express.Router.acl)
- description and source-code
```javascript
acl = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.all"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>all (path)](#apidoc.element.node-odata._express.Router.all)
- description and source-code
```javascript
all = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.bind"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>bind (path)](#apidoc.element.node-odata._express.Router.bind)
- description and source-code
```javascript
bind = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.checkout"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>checkout (path)](#apidoc.element.node-odata._express.Router.checkout)
- description and source-code
```javascript
checkout = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.connect"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>connect (path)](#apidoc.element.node-odata._express.Router.connect)
- description and source-code
```javascript
connect = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.copy"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>copy (path)](#apidoc.element.node-odata._express.Router.copy)
- description and source-code
```javascript
copy = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.delete"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>delete (path)](#apidoc.element.node-odata._express.Router.delete)
- description and source-code
```javascript
delete = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
...
    });
  }
}, {
  key: 'delete',
  value: function _delete(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.delete('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.Router.get"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>get (path)](#apidoc.element.node-odata._express.Router.get)
- description and source-code
```javascript
get = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
...
    var resource = new _ODataResource2.default(name, model);
    this._resources.push(resource);
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.post('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
...
```

#### <a name="apidoc.element.node-odata._express.Router.handle"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>handle (req, res, out)](#apidoc.element.node-odata._express.Router.handle)
- description and source-code
```javascript
function handle(req, res, out) {
  var self = this;

  debug('dispatching %s %s', req.method, req.url);

  var search = 1 + req.url.indexOf('?');
  var pathlength = search ? search - 1 : req.url.length;
  var fqdn = req.url[0] !== '/' && 1 + req.url.substr(0, pathlength).indexOf('://');
  var protohost = fqdn ? req.url.substr(0, req.url.indexOf('/', 2 + fqdn)) : '';
  var idx = 0;
  var removed = '';
  var slashAdded = false;
  var paramcalled = {};

  // store options for OPTIONS request
  // only used if OPTIONS request
  var options = [];

  // middleware and routes
  var stack = self.stack;

  // manage inter-router variables
  var parentParams = req.params;
  var parentUrl = req.baseUrl || '';
  var done = restore(out, req, 'baseUrl', 'next', 'params');

  // setup next layer
  req.next = next;

  // for options requests, respond with a default if nothing else responds
  if (req.method === 'OPTIONS') {
    done = wrap(done, function(old, err) {
      if (err || options.length === 0) return old(err);
      sendOptionsResponse(res, options, old);
    });
  }

  // setup basic req values
  req.baseUrl = parentUrl;
  req.originalUrl = req.originalUrl || req.url;

  next();

  function next(err) {
    var layerError = err === 'route'
      ? null
      : err;

    // remove added slash
    if (slashAdded) {
      req.url = req.url.substr(1);
      slashAdded = false;
    }

    // restore altered req.url
    if (removed.length !== 0) {
      req.baseUrl = parentUrl;
      req.url = protohost + removed + req.url.substr(protohost.length);
      removed = '';
    }

    // no more matching layers
    if (idx >= stack.length) {
      setImmediate(done, layerError);
      return;
    }

    // get pathname of request
    var path = getPathname(req);

    if (path == null) {
      return done(layerError);
    }

    // find next matching layer
    var layer;
    var match;
    var route;

    while (match !== true && idx < stack.length) {
      layer = stack[idx++];
      match = matchLayer(layer, path);
      route = layer.route;

      if (typeof match !== 'boolean') {
        // hold on to layerError
        layerError = layerError || match;
      }

      if (match !== true) {
        continue;
      }

      if (!route) {
        // process non-route handlers normally
        continue;
      }

      if (layerError) {
        // routes do not match with a pending error
        match = false;
        continue;
      }

      var method = req.method;
      var has_method = route._handles_method(method);

      // build up automatic options response
      if (!has_method && method === 'OPTIONS') {
        appendMethods(options, route._options());
      }

      // don't even bother matching route
      if (!has_method && method !== 'HEAD') {
        match = false;
        continue;
      }
    }

    // no match
    if (match !== true) {
      return done(layerError);
    }

    // store route for dispatch on change
    if (route) {
      req.route = route;
    }

    // Capture one-time layer values
    req.params = self.mergeParams
      ? mergeParams(layer.params, parentParams)
      : layer.params;
    var layerPath = layer.path;

    // this should be done for the layer
    self.process_params(layer, paramcalled, req, res, function (err) {
      if (err) {
        return next(layerError || err);
      }

      if (route) {
        return layer.handle_request(req, res, next);
      }

      trim_prefix(layer, layerError, layerPath, path);
    });
  }

  function trim_prefix(layer, layerError, layerPath, path) {
    var c = path[layerPath.length];
    if (c && '/' !== c && '.' !== c) return next(layerError);

     // Trim off the part of the url that matches the route
     // middleware (.use stuff) needs to have the path stripped
    if (layerPath.length !== 0) {
      debug('trim prefix (%s) from url %s', layerPath, req.url);
      removed = layerPath;
      req.url = protohost + req.url.substr(protohost.length + removed.length);

      // Ensure leading slash
      if (!fqdn && req.url[0] !== '/') {
        req.url = ' ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.head"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>head (path)](#apidoc.element.node-odata._express.Router.head)
- description and source-code
```javascript
head = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.link"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>link (path)](#apidoc.element.node-odata._express.Router.link)
- description and source-code
```javascript
link = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.lock"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>lock (path)](#apidoc.element.node-odata._express.Router.lock)
- description and source-code
```javascript
lock = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.m-search"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>m-search (path)](#apidoc.element.node-odata._express.Router.m-search)
- description and source-code
```javascript
m-search = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.merge"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>merge (path)](#apidoc.element.node-odata._express.Router.merge)
- description and source-code
```javascript
merge = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.mkactivity"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>mkactivity (path)](#apidoc.element.node-odata._express.Router.mkactivity)
- description and source-code
```javascript
mkactivity = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.mkcalendar"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>mkcalendar (path)](#apidoc.element.node-odata._express.Router.mkcalendar)
- description and source-code
```javascript
mkcalendar = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.mkcol"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>mkcol (path)](#apidoc.element.node-odata._express.Router.mkcol)
- description and source-code
```javascript
mkcol = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.move"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>move (path)](#apidoc.element.node-odata._express.Router.move)
- description and source-code
```javascript
move = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.notify"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>notify (path)](#apidoc.element.node-odata._express.Router.notify)
- description and source-code
```javascript
notify = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.options"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>options (path)](#apidoc.element.node-odata._express.Router.options)
- description and source-code
```javascript
options = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.param"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>param (name, fn)](#apidoc.element.node-odata._express.Router.param)
- description and source-code
```javascript
function param(name, fn) {
  // param logic
  if (typeof name === 'function') {
    deprecate('router.param(fn): Refactor to use path params');
    this._params.push(name);
    return;
  }

  // apply param functions
  var params = this._params;
  var len = params.length;
  var ret;

  if (name[0] === ':') {
    deprecate('router.param(' + JSON.stringify(name) + ', fn): Use router.param(' + JSON.stringify(name.substr(1)) + ', fn) instead
');
    name = name.substr(1);
  }

  for (var i = 0; i < len; ++i) {
    if (ret = params[i](name, fn)) {
      fn = ret;
    }
  }

  // ensure we end up with a
  // middleware function
  if ('function' !== typeof fn) {
    throw new Error('invalid param() call for ' + name + ', got ' + fn);
  }

  (this.params[name] = this.params[name] || []).push(fn);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.patch"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>patch (path)](#apidoc.element.node-odata._express.Router.patch)
- description and source-code
```javascript
patch = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
...
    });
  }
}, {
  key: 'patch',
  value: function patch(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.patch('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.Router.post"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>post (path)](#apidoc.element.node-odata._express.Router.post)
- description and source-code
```javascript
post = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
...
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.post('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.Router.process_params"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>process_params (layer, called, req, res, done)](#apidoc.element.node-odata._express.Router.process_params)
- description and source-code
```javascript
function process_params(layer, called, req, res, done) {
  var params = this.params;

  // captured parameters from the layer, keys and values
  var keys = layer.keys;

  // fast track
  if (!keys || keys.length === 0) {
    return done();
  }

  var i = 0;
  var name;
  var paramIndex = 0;
  var key;
  var paramVal;
  var paramCallbacks;
  var paramCalled;

  // process params in order
  // param callbacks can be async
  function param(err) {
    if (err) {
      return done(err);
    }

    if (i >= keys.length ) {
      return done();
    }

    paramIndex = 0;
    key = keys[i++];

    if (!key) {
      return done();
    }

    name = key.name;
    paramVal = req.params[name];
    paramCallbacks = params[name];
    paramCalled = called[name];

    if (paramVal === undefined || !paramCallbacks) {
      return param();
    }

    // param previously called with same value or error occurred
    if (paramCalled && (paramCalled.match === paramVal
      || (paramCalled.error && paramCalled.error !== 'route'))) {
      // restore value
      req.params[name] = paramCalled.value;

      // next param
      return param(paramCalled.error);
    }

    called[name] = paramCalled = {
      error: null,
      match: paramVal,
      value: paramVal
    };

    paramCallback();
  }

  // single param callbacks
  function paramCallback(err) {
    var fn = paramCallbacks[paramIndex++];

    // store updated value
    paramCalled.value = req.params[key.name];

    if (err) {
      // store error
      paramCalled.error = err;
      param(err);
      return;
    }

    if (!fn) return param();

    try {
      fn(req, res, paramCallback, paramVal, key.name);
    } catch (e) {
      paramCallback(e);
    }
  }

  param();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.propfind"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>propfind (path)](#apidoc.element.node-odata._express.Router.propfind)
- description and source-code
```javascript
propfind = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.proppatch"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>proppatch (path)](#apidoc.element.node-odata._express.Router.proppatch)
- description and source-code
```javascript
proppatch = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.purge"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>purge (path)](#apidoc.element.node-odata._express.Router.purge)
- description and source-code
```javascript
purge = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.put"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>put (path)](#apidoc.element.node-odata._express.Router.put)
- description and source-code
```javascript
put = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
...
    });
  }
}, {
  key: 'put',
  value: function put(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.put('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.Router.rebind"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>rebind (path)](#apidoc.element.node-odata._express.Router.rebind)
- description and source-code
```javascript
rebind = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.report"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>report (path)](#apidoc.element.node-odata._express.Router.report)
- description and source-code
```javascript
report = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.route"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>route (path)](#apidoc.element.node-odata._express.Router.route)
- description and source-code
```javascript
function route(path) {
  var route = new Route(path);

  var layer = new Layer(path, {
    sensitive: this.caseSensitive,
    strict: this.strict,
    end: true
  }, route.dispatch.bind(route));

  layer.route = route;

  this.stack.push(layer);
  return route;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.search"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>search (path)](#apidoc.element.node-odata._express.Router.search)
- description and source-code
```javascript
search = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.subscribe"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>subscribe (path)](#apidoc.element.node-odata._express.Router.subscribe)
- description and source-code
```javascript
subscribe = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.trace"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>trace (path)](#apidoc.element.node-odata._express.Router.trace)
- description and source-code
```javascript
trace = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.unbind"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>unbind (path)](#apidoc.element.node-odata._express.Router.unbind)
- description and source-code
```javascript
unbind = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.unlink"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>unlink (path)](#apidoc.element.node-odata._express.Router.unlink)
- description and source-code
```javascript
unlink = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.unlock"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>unlock (path)](#apidoc.element.node-odata._express.Router.unlock)
- description and source-code
```javascript
unlock = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.unsubscribe"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>unsubscribe (path)](#apidoc.element.node-odata._express.Router.unsubscribe)
- description and source-code
```javascript
unsubscribe = function (path){
  var route = this.route(path)
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.Router.use"></a>[function <span class="apidocSignatureSpan">node-odata._express.Router.</span>use (fn)](#apidoc.element.node-odata._express.Router.use)
- description and source-code
```javascript
function use(fn) {
  var offset = 0;
  var path = '/';

  // default path to '/'
  // disambiguate router.use([fn])
  if (typeof fn !== 'function') {
    var arg = fn;

    while (Array.isArray(arg) && arg.length !== 0) {
      arg = arg[0];
    }

    // first arg is the path
    if (typeof arg !== 'function') {
      offset = 1;
      path = fn;
    }
  }

  var callbacks = flatten(slice.call(arguments, offset));

  if (callbacks.length === 0) {
    throw new TypeError('Router.use() requires middleware functions');
  }

  for (var i = 0; i < callbacks.length; i++) {
    var fn = callbacks[i];

    if (typeof fn !== 'function') {
      throw new TypeError('Router.use() requires middleware function but got a ' + gettype(fn));
    }

    // add the middleware
    debug('use %s %s', path, fn.name || '<anonymous>');

    var layer = new Layer(path, {
      sensitive: this.caseSensitive,
      strict: false,
      end: false
    }, fn);

    layer.route = undefined;

    this.stack.push(layer);
  }

  return this;
}
```
- example usage
```shell
...

Object.defineProperty(exports, "__esModule", {
  value: true
});

exports.default = function () {
  var app = (0, _express2.default)();
  app.use(_bodyParser2.default.urlencoded({ extended: true }));
  app.use(_bodyParser2.default.json());
  app.use((0, _methodOverride2.default)());
  app.use(_express2.default.query());
  app.use((0, _cors2.default)());
  app.disable('x-powered-by');
  return app;
};
...
```



# <a name="apidoc.module.node-odata._express.application"></a>[module node-odata._express.application](#apidoc.module.node-odata._express.application)

#### <a name="apidoc.element.node-odata._express.application.acl"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>acl (path)](#apidoc.element.node-odata._express.application.acl)
- description and source-code
```javascript
acl = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.all"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>all (path)](#apidoc.element.node-odata._express.application.all)
- description and source-code
```javascript
function all(path) {
  this.lazyrouter();

  var route = this._router.route(path);
  var args = slice.call(arguments, 1);

  for (var i = 0; i < methods.length; i++) {
    route[methods[i]].apply(route, args);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.bind"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>bind (path)](#apidoc.element.node-odata._express.application.bind)
- description and source-code
```javascript
bind = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.checkout"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>checkout (path)](#apidoc.element.node-odata._express.application.checkout)
- description and source-code
```javascript
checkout = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.connect"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>connect (path)](#apidoc.element.node-odata._express.application.connect)
- description and source-code
```javascript
connect = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.copy"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>copy (path)](#apidoc.element.node-odata._express.application.copy)
- description and source-code
```javascript
copy = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.defaultConfiguration"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>defaultConfiguration ()](#apidoc.element.node-odata._express.application.defaultConfiguration)
- description and source-code
```javascript
function defaultConfiguration() {
  var env = process.env.NODE_ENV || 'development';

  // default settings
  this.enable('x-powered-by');
  this.set('etag', 'weak');
  this.set('env', env);
  this.set('query parser', 'extended');
  this.set('subdomain offset', 2);
  this.set('trust proxy', false);

  // trust proxy inherit back-compat
  Object.defineProperty(this.settings, trustProxyDefaultSymbol, {
    configurable: true,
    value: true
  });

  debug('booting in %s mode', env);

  this.on('mount', function onmount(parent) {
    // inherit trust proxy
    if (this.settings[trustProxyDefaultSymbol] === true
      && typeof parent.settings['trust proxy fn'] === 'function') {
      delete this.settings['trust proxy'];
      delete this.settings['trust proxy fn'];
    }

    // inherit protos
    this.request.__proto__ = parent.request;
    this.response.__proto__ = parent.response;
    this.engines.__proto__ = parent.engines;
    this.settings.__proto__ = parent.settings;
  });

  // setup locals
  this.locals = Object.create(null);

  // top-most app is mounted at /
  this.mountpath = '/';

  // default locals
  this.locals.settings = this.settings;

  // default configuration
  this.set('view', View);
  this.set('views', resolve('views'));
  this.set('jsonp callback name', 'callback');

  if (env === 'production') {
    this.enable('view cache');
  }

  Object.defineProperty(this, 'router', {
    get: function() {
      throw new Error('\'app.router\' is deprecated!\nPlease see the 3.x to 4.x migration guide for details on how to update your
 app.');
    }
  });
}
```
- example usage
```shell
...
this._app = (0, _express2.default)();
this._mongoose = _mongoose2.default;
this._settings = {
  maxTop: 10000,
  maxSkip: 10000,
  orderby: undefined
};
this.defaultConfiguration(db, prefix);

// TODO: Infact, resources is a mongooseModel instance, origin name is repositories.
// Should mix _resources object and resources object: _resources + resource = resources.
// Encapsulation to a object, separate mognoose, try to use *repository pattern*.
// 这里也许应该让 resources 支持 odata 查询的, 以方便直接在代码中使用 OData 查询方式来进行数据筛选, 达到隔离 mongo 的效果.
this._resources = [];
this.resources = {};
...
```

#### <a name="apidoc.element.node-odata._express.application.del"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>del (arg0)](#apidoc.element.node-odata._express.application.del)
- description and source-code
```javascript
del = function (arg0) {
"use strict"
log.call(deprecate, message, site)
return fn.apply(this, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.delete"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>delete (path)](#apidoc.element.node-odata._express.application.delete)
- description and source-code
```javascript
delete = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
...
    });
  }
}, {
  key: 'delete',
  value: function _delete(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.delete('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.application.disable"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>disable (setting)](#apidoc.element.node-odata._express.application.disable)
- description and source-code
```javascript
function disable(setting) {
  return this.set(setting, false);
}
```
- example usage
```shell
...
exports.default = function () {
  var app = (0, _express2.default)();
  app.use(_bodyParser2.default.urlencoded({ extended: true }));
  app.use(_bodyParser2.default.json());
  app.use((0, _methodOverride2.default)());
  app.use(_express2.default.query());
  app.use((0, _cors2.default)());
  app.disable('x-powered-by');
  return app;
};

var _express = require('express');

var _express2 = _interopRequireDefault(_express);
...
```

#### <a name="apidoc.element.node-odata._express.application.disabled"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>disabled (setting)](#apidoc.element.node-odata._express.application.disabled)
- description and source-code
```javascript
function disabled(setting) {
  return !this.set(setting);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.enable"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>enable (setting)](#apidoc.element.node-odata._express.application.enable)
- description and source-code
```javascript
function enable(setting) {
  return this.set(setting, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.enabled"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>enabled (setting)](#apidoc.element.node-odata._express.application.enabled)
- description and source-code
```javascript
function enabled(setting) {
  return Boolean(this.set(setting));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.engine"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>engine (ext, fn)](#apidoc.element.node-odata._express.application.engine)
- description and source-code
```javascript
function engine(ext, fn) {
  if (typeof fn !== 'function') {
    throw new Error('callback function required');
  }

  // get file extension
  var extension = ext[0] !== '.'
    ? '.' + ext
    : ext;

  // store engine
  this.engines[extension] = fn;

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.get"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>get (path)](#apidoc.element.node-odata._express.application.get)
- description and source-code
```javascript
get = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
...
    var resource = new _ODataResource2.default(name, model);
    this._resources.push(resource);
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.post('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
...
```

#### <a name="apidoc.element.node-odata._express.application.handle"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>handle (req, res, callback)](#apidoc.element.node-odata._express.application.handle)
- description and source-code
```javascript
function handle(req, res, callback) {
  var router = this._router;

  // final handler
  var done = callback || finalhandler(req, res, {
    env: this.get('env'),
    onerror: logerror.bind(this)
  });

  // no routes
  if (!router) {
    debug('no routes defined on app');
    done();
    return;
  }

  router.handle(req, res, done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.head"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>head (path)](#apidoc.element.node-odata._express.application.head)
- description and source-code
```javascript
head = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.init"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>init ()](#apidoc.element.node-odata._express.application.init)
- description and source-code
```javascript
function init() {
  this.cache = {};
  this.engines = {};
  this.settings = {};

  this.defaultConfiguration();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.lazyrouter"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>lazyrouter ()](#apidoc.element.node-odata._express.application.lazyrouter)
- description and source-code
```javascript
function lazyrouter() {
  if (!this._router) {
    this._router = new Router({
      caseSensitive: this.enabled('case sensitive routing'),
      strict: this.enabled('strict routing')
    });

    this._router.use(query(this.get('query parser fn')));
    this._router.use(middleware.init(this));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.link"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>link (path)](#apidoc.element.node-odata._express.application.link)
- description and source-code
```javascript
link = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.listen"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>listen ()](#apidoc.element.node-odata._express.application.listen)
- description and source-code
```javascript
function listen() {
  var server = http.createServer(this);
  return server.listen.apply(server, arguments);
}
```
- example usage
```shell
...
var server = odata('mongodb://localhost/my-app');

server.resource('books', {
  title: String,
  price: Number
});

server.listen(3000);
'''

Registers the following routes:

'''
GET    /books
GET    /books(:id)
...
```

#### <a name="apidoc.element.node-odata._express.application.lock"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>lock (path)](#apidoc.element.node-odata._express.application.lock)
- description and source-code
```javascript
lock = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.m-search"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>m-search (path)](#apidoc.element.node-odata._express.application.m-search)
- description and source-code
```javascript
m-search = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.merge"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>merge (path)](#apidoc.element.node-odata._express.application.merge)
- description and source-code
```javascript
merge = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.mkactivity"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>mkactivity (path)](#apidoc.element.node-odata._express.application.mkactivity)
- description and source-code
```javascript
mkactivity = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.mkcalendar"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>mkcalendar (path)](#apidoc.element.node-odata._express.application.mkcalendar)
- description and source-code
```javascript
mkcalendar = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.mkcol"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>mkcol (path)](#apidoc.element.node-odata._express.application.mkcol)
- description and source-code
```javascript
mkcol = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.move"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>move (path)](#apidoc.element.node-odata._express.application.move)
- description and source-code
```javascript
move = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.notify"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>notify (path)](#apidoc.element.node-odata._express.application.notify)
- description and source-code
```javascript
notify = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.options"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>options (path)](#apidoc.element.node-odata._express.application.options)
- description and source-code
```javascript
options = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.param"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>param (name, fn)](#apidoc.element.node-odata._express.application.param)
- description and source-code
```javascript
function param(name, fn) {
  this.lazyrouter();

  if (Array.isArray(name)) {
    for (var i = 0; i < name.length; i++) {
      this.param(name[i], fn);
    }

    return this;
  }

  this._router.param(name, fn);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.patch"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>patch (path)](#apidoc.element.node-odata._express.application.patch)
- description and source-code
```javascript
patch = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
...
    });
  }
}, {
  key: 'patch',
  value: function patch(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.patch('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.application.path"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>path ()](#apidoc.element.node-odata._express.application.path)
- description and source-code
```javascript
function path() {
  return this.parent
    ? this.parent.path() + this.mountpath
    : '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.post"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>post (path)](#apidoc.element.node-odata._express.application.post)
- description and source-code
```javascript
post = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
...
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.post('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.application.propfind"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>propfind (path)](#apidoc.element.node-odata._express.application.propfind)
- description and source-code
```javascript
propfind = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.proppatch"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>proppatch (path)](#apidoc.element.node-odata._express.application.proppatch)
- description and source-code
```javascript
proppatch = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.purge"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>purge (path)](#apidoc.element.node-odata._express.application.purge)
- description and source-code
```javascript
purge = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.put"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>put (path)](#apidoc.element.node-odata._express.application.put)
- description and source-code
```javascript
put = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
...
    });
  }
}, {
  key: 'put',
  value: function put(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.put('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
...
```

#### <a name="apidoc.element.node-odata._express.application.rebind"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>rebind (path)](#apidoc.element.node-odata._express.application.rebind)
- description and source-code
```javascript
rebind = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.render"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>render (name, options, callback)](#apidoc.element.node-odata._express.application.render)
- description and source-code
```javascript
function render(name, options, callback) {
  var cache = this.cache;
  var done = callback;
  var engines = this.engines;
  var opts = options;
  var renderOptions = {};
  var view;

  // support callback function as second arg
  if (typeof options === 'function') {
    done = options;
    opts = {};
  }

  // merge app.locals
  merge(renderOptions, this.locals);

  // merge options._locals
  if (opts._locals) {
    merge(renderOptions, opts._locals);
  }

  // merge options
  merge(renderOptions, opts);

  // set .cache unless explicitly provided
  if (renderOptions.cache == null) {
    renderOptions.cache = this.enabled('view cache');
  }

  // primed cache
  if (renderOptions.cache) {
    view = cache[name];
  }

  // view
  if (!view) {
    var View = this.get('view');

    view = new View(name, {
      defaultEngine: this.get('view engine'),
      root: this.get('views'),
      engines: engines
    });

    if (!view.path) {
      var dirs = Array.isArray(view.root) && view.root.length > 1
        ? 'directories "' + view.root.slice(0, -1).join('", "') + '" or "' + view.root[view.root.length - 1] + '"'
        : 'directory "' + view.root + '"'
      var err = new Error('Failed to lookup view "' + name + '" in views ' + dirs);
      err.view = view;
      return done(err);
    }

    // prime the cache
    if (renderOptions.cache) {
      cache[name] = view;
    }
  }

  // render
  tryRender(view, renderOptions, done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.report"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>report (path)](#apidoc.element.node-odata._express.application.report)
- description and source-code
```javascript
report = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.route"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>route (path)](#apidoc.element.node-odata._express.application.route)
- description and source-code
```javascript
function route(path) {
  this.lazyrouter();
  return this._router.route(path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.search"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>search (path)](#apidoc.element.node-odata._express.application.search)
- description and source-code
```javascript
search = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.set"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>set (setting, val)](#apidoc.element.node-odata._express.application.set)
- description and source-code
```javascript
function set(setting, val) {
  if (arguments.length === 1) {
    // app.get(setting)
    return this.settings[setting];
  }

  debug('set "%s" to %o', setting, val);

  // set value
  this.settings[setting] = val;

  // trigger matched settings
  switch (setting) {
    case 'etag':
      this.set('etag fn', compileETag(val));
      break;
    case 'query parser':
      this.set('query parser fn', compileQueryParser(val));
      break;
    case 'trust proxy':
      this.set('trust proxy fn', compileTrust(val));

      // trust proxy inherit back-compat
      Object.defineProperty(this.settings, trustProxyDefaultSymbol, {
        configurable: true,
        value: false
      });

      break;
  }

  return this;
}
```
- example usage
```shell
...
}

_createClass(Server, [{
  key: 'defaultConfiguration',
  value: function defaultConfiguration(db) {
    var prefix = arguments.length <= 1 || arguments[1] === undefined ? '' : arguments[1];

    this.set('app', this._app);
    this.set('db', db);
    this.set('prefix', prefix);
  }
}, {
  key: 'resource',
  value: function resource(name, model) {
    if (model === undefined) {
...
```

#### <a name="apidoc.element.node-odata._express.application.subscribe"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>subscribe (path)](#apidoc.element.node-odata._express.application.subscribe)
- description and source-code
```javascript
subscribe = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.trace"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>trace (path)](#apidoc.element.node-odata._express.application.trace)
- description and source-code
```javascript
trace = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.unbind"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>unbind (path)](#apidoc.element.node-odata._express.application.unbind)
- description and source-code
```javascript
unbind = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.unlink"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>unlink (path)](#apidoc.element.node-odata._express.application.unlink)
- description and source-code
```javascript
unlink = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.unlock"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>unlock (path)](#apidoc.element.node-odata._express.application.unlock)
- description and source-code
```javascript
unlock = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.unsubscribe"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>unsubscribe (path)](#apidoc.element.node-odata._express.application.unsubscribe)
- description and source-code
```javascript
unsubscribe = function (path){
  if (method === 'get' && arguments.length === 1) {
    // app.get(setting)
    return this.set(path);
  }

  this.lazyrouter();

  var route = this._router.route(path);
  route[method].apply(route, slice.call(arguments, 1));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.application.use"></a>[function <span class="apidocSignatureSpan">node-odata._express.application.</span>use (fn)](#apidoc.element.node-odata._express.application.use)
- description and source-code
```javascript
function use(fn) {
  var offset = 0;
  var path = '/';

  // default path to '/'
  // disambiguate app.use([fn])
  if (typeof fn !== 'function') {
    var arg = fn;

    while (Array.isArray(arg) && arg.length !== 0) {
      arg = arg[0];
    }

    // first arg is the path
    if (typeof arg !== 'function') {
      offset = 1;
      path = fn;
    }
  }

  var fns = flatten(slice.call(arguments, offset));

  if (fns.length === 0) {
    throw new TypeError('app.use() requires middleware functions');
  }

  // setup router
  this.lazyrouter();
  var router = this._router;

  fns.forEach(function (fn) {
    // non-express app
    if (!fn || !fn.handle || !fn.set) {
      return router.use(path, fn);
    }

    debug('.use app under %s', path);
    fn.mountpath = path;
    fn.parent = this;

    // restore .app property on req and res
    router.use(path, function mounted_app(req, res, next) {
      var orig = req.app;
      fn.handle(req, res, function (err) {
        req.__proto__ = orig.request;
        res.__proto__ = orig.response;
        next(err);
      });
    });

    // mounted an app
    fn.emit('mount', this);
  }, this);

  return this;
}
```
- example usage
```shell
...

Object.defineProperty(exports, "__esModule", {
  value: true
});

exports.default = function () {
  var app = (0, _express2.default)();
  app.use(_bodyParser2.default.urlencoded({ extended: true }));
  app.use(_bodyParser2.default.json());
  app.use((0, _methodOverride2.default)());
  app.use(_express2.default.query());
  app.use((0, _cors2.default)());
  app.disable('x-powered-by');
  return app;
};
...
```



# <a name="apidoc.module.node-odata._express.request"></a>[module node-odata._express.request](#apidoc.module.node-odata._express.request)

#### <a name="apidoc.element.node-odata._express.request.accepts"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>accepts ()](#apidoc.element.node-odata._express.request.accepts)
- description and source-code
```javascript
accepts = function (){
  var accept = accepts(this);
  return accept.types.apply(accept, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.request.acceptsCharset"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsCharset ()](#apidoc.element.node-odata._express.request.acceptsCharset)
- description and source-code
```javascript
acceptsCharset = function () {
"use strict"
log.call(deprecate, message, site)
return fn.apply(this, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.request.acceptsCharsets"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsCharsets ()](#apidoc.element.node-odata._express.request.acceptsCharsets)
- description and source-code
```javascript
acceptsCharsets = function (){
  var accept = accepts(this);
  return accept.charsets.apply(accept, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.request.acceptsEncoding"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsEncoding ()](#apidoc.element.node-odata._express.request.acceptsEncoding)
- description and source-code
```javascript
acceptsEncoding = function () {
"use strict"
log.call(deprecate, message, site)
return fn.apply(this, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.request.acceptsEncodings"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsEncodings ()](#apidoc.element.node-odata._express.request.acceptsEncodings)
- description and source-code
```javascript
acceptsEncodings = function (){
  var accept = accepts(this);
  return accept.encodings.apply(accept, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.request.acceptsLanguage"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsLanguage ()](#apidoc.element.node-odata._express.request.acceptsLanguage)
- description and source-code
```javascript
acceptsLanguage = function () {
"use strict"
log.call(deprecate, message, site)
return fn.apply(this, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.request.acceptsLanguages"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>acceptsLanguages ()](#apidoc.element.node-odata._express.request.acceptsLanguages)
- description and source-code
```javascript
acceptsLanguages = function (){
  var accept = accepts(this);
  return accept.languages.apply(accept, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.request.get"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>get (name)](#apidoc.element.node-odata._express.request.get)
- description and source-code
```javascript
function header(name) {
  if (!name) {
    throw new TypeError('name argument is required to req.get');
  }

  if (typeof name !== 'string') {
    throw new TypeError('name must be a string to req.get');
  }

  var lc = name.toLowerCase();

  switch (lc) {
    case 'referer':
    case 'referrer':
      return this.headers.referrer
        || this.headers.referer;
    default:
      return this.headers[lc];
  }
}
```
- example usage
```shell
...
    var resource = new _ODataResource2.default(name, model);
    this._resources.push(resource);
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.post('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
...
```

#### <a name="apidoc.element.node-odata._express.request.header"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>header (name)](#apidoc.element.node-odata._express.request.header)
- description and source-code
```javascript
function header(name) {
  if (!name) {
    throw new TypeError('name argument is required to req.get');
  }

  if (typeof name !== 'string') {
    throw new TypeError('name must be a string to req.get');
  }

  var lc = name.toLowerCase();

  switch (lc) {
    case 'referer':
    case 'referrer':
      return this.headers.referrer
        || this.headers.referer;
    default:
      return this.headers[lc];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.request.is"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>is (types)](#apidoc.element.node-odata._express.request.is)
- description and source-code
```javascript
function is(types) {
  var arr = types;

  // support flattened arguments
  if (!Array.isArray(types)) {
    arr = new Array(arguments.length);
    for (var i = 0; i < arr.length; i++) {
      arr[i] = arguments[i];
    }
  }

  return typeis(this, arr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.request.param"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>param (name, defaultValue)](#apidoc.element.node-odata._express.request.param)
- description and source-code
```javascript
function param(name, defaultValue) {
  var params = this.params || {};
  var body = this.body || {};
  var query = this.query || {};

  var args = arguments.length === 1
    ? 'name'
    : 'name, default';
  deprecate('req.param(' + args + '): Use req.params, req.body, or req.query instead');

  if (null != params[name] && params.hasOwnProperty(name)) return params[name];
  if (null != body[name]) return body[name];
  if (null != query[name]) return query[name];

  return defaultValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.request.range"></a>[function <span class="apidocSignatureSpan">node-odata._express.request.</span>range (size, options)](#apidoc.element.node-odata._express.request.range)
- description and source-code
```javascript
function range(size, options) {
  var range = this.get('Range');
  if (!range) return;
  return parseRange(size, range, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-odata._express.response"></a>[module node-odata._express.response](#apidoc.module.node-odata._express.response)

#### <a name="apidoc.element.node-odata._express.response.append"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>append (field, val)](#apidoc.element.node-odata._express.response.append)
- description and source-code
```javascript
function append(field, val) {
  var prev = this.get(field);
  var value = val;

  if (prev) {
    // concat the new and prev vals
    value = Array.isArray(prev) ? prev.concat(val)
      : Array.isArray(val) ? [prev].concat(val)
      : [prev, val];
  }

  return this.set(field, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.attachment"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>attachment (filename)](#apidoc.element.node-odata._express.response.attachment)
- description and source-code
```javascript
function attachment(filename) {
  if (filename) {
    this.type(extname(filename));
  }

  this.set('Content-Disposition', contentDisposition(filename));

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.clearCookie"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>clearCookie (name, options)](#apidoc.element.node-odata._express.response.clearCookie)
- description and source-code
```javascript
function clearCookie(name, options) {
  var opts = merge({ expires: new Date(1), path: '/' }, options);

  return this.cookie(name, '', opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.contentType"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>contentType (type)](#apidoc.element.node-odata._express.response.contentType)
- description and source-code
```javascript
function contentType(type) {
  var ct = type.indexOf('/') === -1
    ? mime.lookup(type)
    : type;

  return this.set('Content-Type', ct);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.cookie"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>cookie (name, value, options)](#apidoc.element.node-odata._express.response.cookie)
- description and source-code
```javascript
cookie = function (name, value, options) {
  var opts = merge({}, options);
  var secret = this.req.secret;
  var signed = opts.signed;

  if (signed && !secret) {
    throw new Error('cookieParser("secret") required for signed cookies');
  }

  var val = typeof value === 'object'
    ? 'j:' + JSON.stringify(value)
    : String(value);

  if (signed) {
    val = 's:' + sign(val, secret);
  }

  if ('maxAge' in opts) {
    opts.expires = new Date(Date.now() + opts.maxAge);
    opts.maxAge /= 1000;
  }

  if (opts.path == null) {
    opts.path = '/';
  }

  this.append('Set-Cookie', cookie.serialize(name, String(val), opts));

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.download"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>download (path, filename, callback)](#apidoc.element.node-odata._express.response.download)
- description and source-code
```javascript
function download(path, filename, callback) {
  var done = callback;
  var name = filename;

  // support function as second arg
  if (typeof filename === 'function') {
    done = filename;
    name = null;
  }

  // set Content-Disposition when file is sent
  var headers = {
    'Content-Disposition': contentDisposition(name || path)
  };

  // Resolve the full path for sendFile
  var fullPath = resolve(path);

  return this.sendFile(fullPath, { headers: headers }, done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.format"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>format (obj)](#apidoc.element.node-odata._express.response.format)
- description and source-code
```javascript
format = function (obj){
  var req = this.req;
  var next = req.next;

  var fn = obj.default;
  if (fn) delete obj.default;
  var keys = Object.keys(obj);

  var key = keys.length > 0
    ? req.accepts(keys)
    : false;

  this.vary("Accept");

  if (key) {
    this.set('Content-Type', normalizeType(key).value);
    obj[key](req, this, next);
  } else if (fn) {
    fn();
  } else {
    var err = new Error('Not Acceptable');
    err.status = err.statusCode = 406;
    err.types = normalizeTypes(keys).map(function(o){ return o.value });
    next(err);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.get"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>get (field)](#apidoc.element.node-odata._express.response.get)
- description and source-code
```javascript
get = function (field){
  return this.getHeader(field);
}
```
- example usage
```shell
...
    var resource = new _ODataResource2.default(name, model);
    this._resources.push(resource);
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.post('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
...
```

#### <a name="apidoc.element.node-odata._express.response.header"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>header (field, val)](#apidoc.element.node-odata._express.response.header)
- description and source-code
```javascript
function header(field, val) {
  if (arguments.length === 2) {
    var value = Array.isArray(val)
      ? val.map(String)
      : String(val);

    // add charset to content-type
    if (field.toLowerCase() === 'content-type' && !charsetRegExp.test(value)) {
      var charset = mime.charsets.lookup(value.split(';')[0]);
      if (charset) value += '; charset=' + charset.toLowerCase();
    }

    this.setHeader(field, value);
  } else {
    for (var key in field) {
      this.set(key, field[key]);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.json"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>json (obj)](#apidoc.element.node-odata._express.response.json)
- description and source-code
```javascript
function json(obj) {
  var val = obj;

  // allow status / body
  if (arguments.length === 2) {
    // res.json(body, status) backwards compat
    if (typeof arguments[1] === 'number') {
      deprecate('res.json(obj, status): Use res.status(status).json(obj) instead');
      this.statusCode = arguments[1];
    } else {
      deprecate('res.json(status, obj): Use res.status(status).json(obj) instead');
      this.statusCode = arguments[0];
      val = arguments[1];
    }
  }

  // settings
  var app = this.app;
  var replacer = app.get('json replacer');
  var spaces = app.get('json spaces');
  var body = stringify(val, replacer, spaces);

  // content-type
  if (!this.get('Content-Type')) {
    this.set('Content-Type', 'application/json');
  }

  return this.send(body);
}
```
- example usage
```shell
...
Object.defineProperty(exports, "__esModule", {
  value: true
});

exports.default = function () {
  var app = (0, _express2.default)();
  app.use(_bodyParser2.default.urlencoded({ extended: true }));
  app.use(_bodyParser2.default.json());
  app.use((0, _methodOverride2.default)());
  app.use(_express2.default.query());
  app.use((0, _cors2.default)());
  app.disable('x-powered-by');
  return app;
};
...
```

#### <a name="apidoc.element.node-odata._express.response.jsonp"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>jsonp (obj)](#apidoc.element.node-odata._express.response.jsonp)
- description and source-code
```javascript
function jsonp(obj) {
  var val = obj;

  // allow status / body
  if (arguments.length === 2) {
    // res.json(body, status) backwards compat
    if (typeof arguments[1] === 'number') {
      deprecate('res.jsonp(obj, status): Use res.status(status).json(obj) instead');
      this.statusCode = arguments[1];
    } else {
      deprecate('res.jsonp(status, obj): Use res.status(status).jsonp(obj) instead');
      this.statusCode = arguments[0];
      val = arguments[1];
    }
  }

  // settings
  var app = this.app;
  var replacer = app.get('json replacer');
  var spaces = app.get('json spaces');
  var body = stringify(val, replacer, spaces);
  var callback = this.req.query[app.get('jsonp callback name')];

  // content-type
  if (!this.get('Content-Type')) {
    this.set('X-Content-Type-Options', 'nosniff');
    this.set('Content-Type', 'application/json');
  }

  // fixup callback
  if (Array.isArray(callback)) {
    callback = callback[0];
  }

  // jsonp
  if (typeof callback === 'string' && callback.length !== 0) {
    this.charset = 'utf-8';
    this.set('X-Content-Type-Options', 'nosniff');
    this.set('Content-Type', 'text/javascript');

    // restrict callback charset
    callback = callback.replace(/[^\[\]\w$.]/g, '');

    // replace chars not allowed in JavaScript that are in JSON
    body = body
      .replace(/\u2028/g, '\\u2028')
      .replace(/\u2029/g, '\\u2029');

    // the /**/ is a specific security mitigation for "Rosetta Flash JSONP abuse"
    // the typeof check is just to reduce client error noise
    body = '/**/ typeof ' + callback + ' === \'function\' && ' + callback + '(' + body + ');';
  }

  return this.send(body);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.links"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>links (links)](#apidoc.element.node-odata._express.response.links)
- description and source-code
```javascript
links = function (links){
  var link = this.get('Link') || '';
  if (link) link += ', ';
  return this.set('Link', link + Object.keys(links).map(function(rel){
    return '<' + links[rel] + '>; rel="' + rel + '"';
  }).join(', '));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.location"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>location (url)](#apidoc.element.node-odata._express.response.location)
- description and source-code
```javascript
function location(url) {
  var loc = url;

  // "back" is an alias for the referrer
  if (url === 'back') {
    loc = this.req.get('Referrer') || '/';
  }

  // set location
  return this.set('Location', encodeUrl(loc));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.redirect"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>redirect (url)](#apidoc.element.node-odata._express.response.redirect)
- description and source-code
```javascript
function redirect(url) {
  var address = url;
  var body;
  var status = 302;

  // allow status / url
  if (arguments.length === 2) {
    if (typeof arguments[0] === 'number') {
      status = arguments[0];
      address = arguments[1];
    } else {
      deprecate('res.redirect(url, status): Use res.redirect(status, url) instead');
      status = arguments[1];
    }
  }

  // Set location header
  address = this.location(address).get('Location');

  // Support text/{plain,html} by default
  this.format({
    text: function(){
      body = statusCodes[status] + '. Redirecting to ' + address;
    },

    html: function(){
      var u = escapeHtml(address);
      body = '<p>' + statusCodes[status] + '. Redirecting to <a href="' + u + '">' + u + '</a></p>';
    },

    default: function(){
      body = '';
    }
  });

  // Respond
  this.statusCode = status;
  this.set('Content-Length', Buffer.byteLength(body));

  if (this.req.method === 'HEAD') {
    this.end();
  } else {
    this.end(body);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.render"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>render (view, options, callback)](#apidoc.element.node-odata._express.response.render)
- description and source-code
```javascript
function render(view, options, callback) {
  var app = this.req.app;
  var done = callback;
  var opts = options || {};
  var req = this.req;
  var self = this;

  // support callback function as second arg
  if (typeof options === 'function') {
    done = options;
    opts = {};
  }

  // merge res.locals
  opts._locals = self.locals;

  // default callback to respond
  done = done || function (err, str) {
    if (err) return req.next(err);
    self.send(str);
  };

  // render
  app.render(view, opts, done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.send"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>send (body)](#apidoc.element.node-odata._express.response.send)
- description and source-code
```javascript
function send(body) {
  var chunk = body;
  var encoding;
  var len;
  var req = this.req;
  var type;

  // settings
  var app = this.app;

  // allow status / body
  if (arguments.length === 2) {
    // res.send(body, status) backwards compat
    if (typeof arguments[0] !== 'number' && typeof arguments[1] === 'number') {
      deprecate('res.send(body, status): Use res.status(status).send(body) instead');
      this.statusCode = arguments[1];
    } else {
      deprecate('res.send(status, body): Use res.status(status).send(body) instead');
      this.statusCode = arguments[0];
      chunk = arguments[1];
    }
  }

  // disambiguate res.send(status) and res.send(status, num)
  if (typeof chunk === 'number' && arguments.length === 1) {
    // res.send(status) will set status message as text string
    if (!this.get('Content-Type')) {
      this.type('txt');
    }

    deprecate('res.send(status): Use res.sendStatus(status) instead');
    this.statusCode = chunk;
    chunk = statusCodes[chunk];
  }

  switch (typeof chunk) {
    // string defaulting to html
    case 'string':
      if (!this.get('Content-Type')) {
        this.type('html');
      }
      break;
    case 'boolean':
    case 'number':
    case 'object':
      if (chunk === null) {
        chunk = '';
      } else if (Buffer.isBuffer(chunk)) {
        if (!this.get('Content-Type')) {
          this.type('bin');
        }
      } else {
        return this.json(chunk);
      }
      break;
  }

  // write strings in utf-8
  if (typeof chunk === 'string') {
    encoding = 'utf8';
    type = this.get('Content-Type');

    // reflect this in content-type
    if (typeof type === 'string') {
      this.set('Content-Type', setCharset(type, 'utf-8'));
    }
  }

  // populate Content-Length
  if (chunk !== undefined) {
    if (!Buffer.isBuffer(chunk)) {
      // convert chunk to Buffer; saves later double conversions
      chunk = new Buffer(chunk, encoding);
      encoding = undefined;
    }

    len = chunk.length;
    this.set('Content-Length', len);
  }

  // populate ETag
  var etag;
  var generateETag = len !== undefined && app.get('etag fn');
  if (typeof generateETag === 'function' && !this.get('ETag')) {
    if ((etag = generateETag(chunk, encoding))) {
      this.set('ETag', etag);
    }
  }

  // freshness
  if (req.fresh) this.statusCode = 304;

  // strip irrelevant headers
  if (204 === this.statusCode || 304 === this.statusCode) {
    this.removeHeader('Content-Type');
    this.removeHeader('Content-Length');
    this.removeHeader('Transfer-Encoding');
    chunk = '';
  }

  if (req.method === 'HEAD') {
    // skip body for HEAD
    this.end();
  } else {
    // respond
    this.end(chunk, encoding);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.sendFile"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>sendFile (path, options, callback)](#apidoc.element.node-odata._express.response.sendFile)
- description and source-code
```javascript
function sendFile(path, options, callback) {
  var done = callback;
  var req = this.req;
  var res = this;
  var next = req.next;
  var opts = options || {};

  if (!path) {
    throw new TypeError('path argument is required to res.sendFile');
  }

  // support function as second arg
  if (typeof options === 'function') {
    done = options;
    opts = {};
  }

  if (!opts.root && !isAbsolute(path)) {
    throw new TypeError('path must be absolute or specify root to res.sendFile');
  }

  // create file stream
  var pathname = encodeURI(path);
  var file = send(req, pathname, opts);

  // transfer
  sendfile(res, file, opts, function (err) {
    if (done) return done(err);
    if (err && err.code === 'EISDIR') return next();

    // next() all but write errors
    if (err && err.code !== 'ECONNABORTED' && err.syscall !== 'write') {
      next(err);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.sendStatus"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>sendStatus (statusCode)](#apidoc.element.node-odata._express.response.sendStatus)
- description and source-code
```javascript
function sendStatus(statusCode) {
  var body = statusCodes[statusCode] || String(statusCode);

  this.statusCode = statusCode;
  this.type('txt');

  return this.send(body);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.sendfile"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>sendfile (arg0, arg1, arg2)](#apidoc.element.node-odata._express.response.sendfile)
- description and source-code
```javascript
sendfile = function (arg0, arg1, arg2) {
"use strict"
log.call(deprecate, message, site)
return fn.apply(this, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.set"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>set (field, val)](#apidoc.element.node-odata._express.response.set)
- description and source-code
```javascript
function header(field, val) {
  if (arguments.length === 2) {
    var value = Array.isArray(val)
      ? val.map(String)
      : String(val);

    // add charset to content-type
    if (field.toLowerCase() === 'content-type' && !charsetRegExp.test(value)) {
      var charset = mime.charsets.lookup(value.split(';')[0]);
      if (charset) value += '; charset=' + charset.toLowerCase();
    }

    this.setHeader(field, value);
  } else {
    for (var key in field) {
      this.set(key, field[key]);
    }
  }
  return this;
}
```
- example usage
```shell
...
}

_createClass(Server, [{
  key: 'defaultConfiguration',
  value: function defaultConfiguration(db) {
    var prefix = arguments.length <= 1 || arguments[1] === undefined ? '' : arguments[1];

    this.set('app', this._app);
    this.set('db', db);
    this.set('prefix', prefix);
  }
}, {
  key: 'resource',
  value: function resource(name, model) {
    if (model === undefined) {
...
```

#### <a name="apidoc.element.node-odata._express.response.status"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>status (code)](#apidoc.element.node-odata._express.response.status)
- description and source-code
```javascript
function status(code) {
  this.statusCode = code;
  return this;
}
```
- example usage
```shell
...
  value: function post(url, callback, auth) {
    var app = this.get('app');
    var prefix = this.get('prefix');
    app.post('' + prefix + url, function (req, res, next) {
      if (checkAuth(auth, req)) {
        callback(req, res, next);
      } else {
        res.status(401).end();
      }
    });
  }
}, {
  key: 'put',
  value: function put(url, callback, auth) {
    var app = this.get('app');
...
```

#### <a name="apidoc.element.node-odata._express.response.type"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>type (type)](#apidoc.element.node-odata._express.response.type)
- description and source-code
```javascript
function contentType(type) {
  var ct = type.indexOf('/') === -1
    ? mime.lookup(type)
    : type;

  return this.set('Content-Type', ct);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata._express.response.vary"></a>[function <span class="apidocSignatureSpan">node-odata._express.response.</span>vary (field)](#apidoc.element.node-odata._express.response.vary)
- description and source-code
```javascript
vary = function (field){
  // checks for back-compat
  if (!field || (Array.isArray(field) && !field.length)) {
    deprecate('res.vary(): Provide a field name');
    return this;
  }

  vary(this, field);

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-odata.express"></a>[module node-odata.express](#apidoc.module.node-odata.express)

#### <a name="apidoc.element.node-odata.express.default"></a>[function <span class="apidocSignatureSpan">node-odata.express.</span>default ()](#apidoc.element.node-odata.express.default)
- description and source-code
```javascript
default = function () {
  var app = (0, _express2.default)();
  app.use(_bodyParser2.default.urlencoded({ extended: true }));
  app.use(_bodyParser2.default.json());
  app.use((0, _methodOverride2.default)());
  app.use(_express2.default.query());
  app.use((0, _cors2.default)());
  app.disable('x-powered-by');
  return app;
}
```
- example usage
```shell
...
  }
}, {
  key: 'resource',
  value: function resource(name, model) {
    if (model === undefined) {
      return this._resources.name;
    }
    var resource = new _ODataResource2.default(name, model);
    this._resources.push(resource);
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
...
```



# <a name="apidoc.module.node-odata.server"></a>[module node-odata.server](#apidoc.module.node-odata.server)

#### <a name="apidoc.element.node-odata.server.default"></a>[function <span class="apidocSignatureSpan">node-odata.server.</span>default (db, prefix)](#apidoc.element.node-odata.server.default)
- description and source-code
```javascript
function Server(db, prefix) {
  _classCallCheck(this, Server);

  this._app = (0, _express2.default)();
  this._mongoose = _mongoose2.default;
  this._settings = {
    maxTop: 10000,
    maxSkip: 10000,
    orderby: undefined
  };
  this.defaultConfiguration(db, prefix);

  // TODO: Infact, resources is a mongooseModel instance, origin name is repositories.
  // Should mix _resources object and resources object: _resources + resource = resources.
  // Encapsulation to a object, separate mognoose, try to use *repository pattern*.
  // 这里也许应该让 resources 支持 odata 查询的, 以方便直接在代码中使用 OData 查询方式来进行数据筛选, 达到隔离 mongo 的效果.
  this._resources = [];
  this.resources = {};
}
```
- example usage
```shell
...
  }
}, {
  key: 'resource',
  value: function resource(name, model) {
    if (model === undefined) {
      return this._resources.name;
    }
    var resource = new _ODataResource2.default(name, model);
    this._resources.push(resource);
    return resource;
  }
}, {
  key: 'post',
  value: function post(url, callback, auth) {
    var app = this.get('app');
...
```



# <a name="apidoc.module.node-odata.utils"></a>[module node-odata.utils](#apidoc.module.node-odata.utils)

#### <a name="apidoc.element.node-odata.utils.min"></a>[function <span class="apidocSignatureSpan">node-odata.utils.</span>min (arr)](#apidoc.element.node-odata.utils.min)
- description and source-code
```javascript
function min(arr) {
  return arr.map(function (item) {
    return +item;
  }).filter(function (item) {
    return Number.isInteger(item);
  }).reduce(function (current, next) {
    return current < next ? current : next;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-odata.utils.split"></a>[function <span class="apidocSignatureSpan">node-odata.utils.</span>split (sentence)](#apidoc.element.node-odata.utils.split)
- description and source-code
```javascript
function split(sentence) {
  var keys = arguments.length <= 1 || arguments[1] === undefined ? [] : arguments[1];

  var keysArray = keys;
  if (!(keysArray instanceof Array)) {
    keysArray = [keysArray];
  }
  var result = [];
  var tmp = [];
  var words = sentence.split(' ');
  words.forEach(function (word) {
    if (keysArray.indexOf(word) > -1) {
      result.push(merge(tmp));
      result.push(word);
      tmp = [];
    } else {
      tmp.push(word);
    }
  });
  result.push(merge(tmp));
  return result;
}
```
- example usage
```shell
...

var keysArray = keys;
if (!(keysArray instanceof Array)) {
  keysArray = [keysArray];
}
var result = [];
var tmp = [];
var words = sentence.split(' ');
words.forEach(function (word) {
  if (keysArray.indexOf(word) > -1) {
    result.push(merge(tmp));
    result.push(word);
    tmp = [];
  } else {
    tmp.push(word);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
