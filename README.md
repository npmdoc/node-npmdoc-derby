# api documentation for  [derby (v0.9.7)](http://derbyjs.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-derby.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-derby) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-derby.svg)](https://travis-ci.org/npmdoc/node-npmdoc-derby)
#### MVC framework making it easy to write realtime, collaborative applications that run in both Node.js and browsers.

[![NPM](https://nodei.co/npm/derby.png?downloads=true)](https://www.npmjs.com/package/derby)

[![apidoc](https://npmdoc.github.io/node-npmdoc-derby/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-derby_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-derby/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-derby/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-derby/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Nate Smith"
    },
    "bugs": {
        "url": "https://github.com/derbyjs/derby/issues"
    },
    "dependencies": {
        "chokidar": "^1.2.0",
        "derby-parsing": "^0.5.0",
        "derby-templates": "^0.4.0",
        "html-util": "^0.2.1",
        "racer": "^0.9.0",
        "resolve": "^1.1.6",
        "through": "^2.3.4",
        "tracks": "^0.5.0"
    },
    "description": "MVC framework making it easy to write realtime, collaborative applications that run in both Node.js and browsers.",
    "devDependencies": {
        "browserify": "^11.2.0",
        "expect.js": "^0.3.1",
        "express": "^4.13.3",
        "jshint": "^2.8.0",
        "mocha": "^2.3.3"
    },
    "directories": {
        "doc": "docs",
        "test": "test"
    },
    "dist": {
        "shasum": "bda76b5c2fc70f8a2cb4876e63103e14f745dfd0",
        "tarball": "https://registry.npmjs.org/derby/-/derby-0.9.7.tgz"
    },
    "gitHead": "242f969ca74c76b89ec4fa9b79e7c554490d999f",
    "homepage": "http://derbyjs.com/",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "nateps",
            "email": "nate@nateps.com"
        },
        {
            "name": "josephg",
            "email": "me@josephg.com"
        },
        {
            "name": "ishbu",
            "email": "randal.truong@gmail.com"
        },
        {
            "name": "enjalot",
            "email": "enjalot@gmail.com"
        }
    ],
    "name": "derby",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/derbyjs/derby.git"
    },
    "scripts": {
        "test": "mocha test/all/*.mocha.js; ./node_modules/.bin/jshint lib/*.js test/*.js"
    },
    "version": "0.9.7"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module derby](#apidoc.module.derby)
1.  [function <span class="apidocSignatureSpan">derby.</span>App (derby, name, filename, options)](#apidoc.element.derby.App)
1.  [function <span class="apidocSignatureSpan">derby.</span>Controller (app, page, model)](#apidoc.element.derby.Controller)
1.  [function <span class="apidocSignatureSpan">derby.</span>Derby ()](#apidoc.element.derby.Derby)
1.  [function <span class="apidocSignatureSpan">derby.</span>Dom (controller)](#apidoc.element.derby.Dom)
1.  [function <span class="apidocSignatureSpan">derby.</span>Page (app, model, req, res)](#apidoc.element.derby.Page)
1.  [function <span class="apidocSignatureSpan">derby.</span>eventmodel ()](#apidoc.element.derby.eventmodel)
1.  object <span class="apidocSignatureSpan">derby.</span>App.prototype
1.  object <span class="apidocSignatureSpan">derby.</span>Controller.prototype
1.  object <span class="apidocSignatureSpan">derby.</span>Derby.prototype
1.  object <span class="apidocSignatureSpan">derby.</span>Dom.prototype
1.  object <span class="apidocSignatureSpan">derby.</span>Page.prototype
1.  object <span class="apidocSignatureSpan">derby.</span>components
1.  object <span class="apidocSignatureSpan">derby.</span>documentListeners
1.  object <span class="apidocSignatureSpan">derby.</span>eventmodel.prototype
1.  object <span class="apidocSignatureSpan">derby.</span>files
1.  object <span class="apidocSignatureSpan">derby.</span>textDiff

#### [module derby.App](#apidoc.module.derby.App)
1.  [function <span class="apidocSignatureSpan">derby.</span>App (derby, name, filename, options)](#apidoc.element.derby.App.App)

#### [module derby.App.prototype](#apidoc.module.derby.App.prototype)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_addAgent (agent)](#apidoc.element.derby.App.prototype._addAgent)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_autoRefresh (backend)](#apidoc.element.derby.App.prototype._autoRefresh)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_contentReady ()](#apidoc.element.derby.App.prototype._contentReady)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_finishInit ()](#apidoc.element.derby.App.prototype._finishInit)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_getScript ()](#apidoc.element.derby.App.prototype._getScript)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_handleMessage (agent, action, message)](#apidoc.element.derby.App.prototype._handleMessage)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_init (options)](#apidoc.element.derby.App.prototype._init)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_loadStyles (filename, options)](#apidoc.element.derby.App.prototype._loadStyles)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_refreshClients ()](#apidoc.element.derby.App.prototype._refreshClients)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_refreshStyles (filename, styles)](#apidoc.element.derby.App.prototype._refreshStyles)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_updateScriptViews ()](#apidoc.element.derby.App.prototype._updateScriptViews)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_viewsSource (options)](#apidoc.element.derby.App.prototype._viewsSource)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_watchBundle (filenames)](#apidoc.element.derby.App.prototype._watchBundle)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_watchStyles (filenames, filename, options)](#apidoc.element.derby.App.prototype._watchStyles)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>_watchViews (filenames, filename, namespace)](#apidoc.element.derby.App.prototype._watchViews)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>addListener (type, listener)](#apidoc.element.derby.App.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>bundle (backend, options, cb)](#apidoc.element.derby.App.prototype.bundle)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>component (viewName, constructor)](#apidoc.element.derby.App.prototype.component)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>createPage (req, res, next)](#apidoc.element.derby.App.prototype.createPage)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>deserialize ()](#apidoc.element.derby.App.prototype.deserialize)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>emit (type)](#apidoc.element.derby.App.prototype.emit)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>eventNames ()](#apidoc.element.derby.App.prototype.eventNames)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>getMaxListeners ()](#apidoc.element.derby.App.prototype.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>listenerCount (type)](#apidoc.element.derby.App.prototype.listenerCount)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>listeners (type)](#apidoc.element.derby.App.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>loadStyles (filename, options)](#apidoc.element.derby.App.prototype.loadStyles)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>loadViews (filename, namespace)](#apidoc.element.derby.App.prototype.loadViews)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>on (type, listener)](#apidoc.element.derby.App.prototype.on)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>onRoute (callback, page, next, done)](#apidoc.element.derby.App.prototype.onRoute)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>once (type, listener)](#apidoc.element.derby.App.prototype.once)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>prependListener (type, listener)](#apidoc.element.derby.App.prototype.prependListener)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.derby.App.prototype.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>removeAllListeners (type)](#apidoc.element.derby.App.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>removeListener (type, listener)](#apidoc.element.derby.App.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>serialize ()](#apidoc.element.derby.App.prototype.serialize)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>serverUse (module, id, options)](#apidoc.element.derby.App.prototype.serverUse)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>setMaxListeners (n)](#apidoc.element.derby.App.prototype.setMaxListeners)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>use (plugin, options)](#apidoc.element.derby.App.prototype.use)
1.  [function <span class="apidocSignatureSpan">derby.App.prototype.</span>writeScripts (backend, dir, options, cb)](#apidoc.element.derby.App.prototype.writeScripts)
1.  undefined <span class="apidocSignatureSpan">derby.App.prototype.</span>domain

#### [module derby.Controller](#apidoc.module.derby.Controller)
1.  [function <span class="apidocSignatureSpan">derby.</span>Controller (app, page, model)](#apidoc.element.derby.Controller.Controller)

#### [module derby.Controller.prototype](#apidoc.module.derby.Controller.prototype)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>addListener (type, listener)](#apidoc.element.derby.Controller.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>emit (type)](#apidoc.element.derby.Controller.prototype.emit)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>emitCancellable ()](#apidoc.element.derby.Controller.prototype.emitCancellable)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>emitDelayable ()](#apidoc.element.derby.Controller.prototype.emitDelayable)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>eventNames ()](#apidoc.element.derby.Controller.prototype.eventNames)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>getMaxListeners ()](#apidoc.element.derby.Controller.prototype.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>listenerCount (type)](#apidoc.element.derby.Controller.prototype.listenerCount)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>listeners (type)](#apidoc.element.derby.Controller.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>on (type, listener)](#apidoc.element.derby.Controller.prototype.on)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>once (type, listener)](#apidoc.element.derby.Controller.prototype.once)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>prependListener (type, listener)](#apidoc.element.derby.Controller.prototype.prependListener)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.derby.Controller.prototype.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>removeAllListeners (type)](#apidoc.element.derby.Controller.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>removeListener (type, listener)](#apidoc.element.derby.Controller.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>setMaxListeners (n)](#apidoc.element.derby.Controller.prototype.setMaxListeners)
1.  undefined <span class="apidocSignatureSpan">derby.Controller.prototype.</span>domain

#### [module derby.Derby](#apidoc.module.derby.Derby)
1.  [function <span class="apidocSignatureSpan">derby.</span>Derby ()](#apidoc.element.derby.Derby.Derby)

#### [module derby.Derby.prototype](#apidoc.module.derby.Derby.prototype)
1.  [function <span class="apidocSignatureSpan">derby.Derby.prototype.</span>App (derby, name, filename, options)](#apidoc.element.derby.Derby.prototype.App)
1.  [function <span class="apidocSignatureSpan">derby.Derby.prototype.</span>Component (parent, context, id, scope)](#apidoc.element.derby.Derby.prototype.Component)
1.  [function <span class="apidocSignatureSpan">derby.Derby.prototype.</span>Page (app, model, req, res)](#apidoc.element.derby.Derby.prototype.Page)
1.  [function <span class="apidocSignatureSpan">derby.Derby.prototype.</span>createApp (name, filename, options)](#apidoc.element.derby.Derby.prototype.createApp)
1.  [function <span class="apidocSignatureSpan">derby.Derby.prototype.</span>run (createServer)](#apidoc.element.derby.Derby.prototype.run)
1.  number <span class="apidocSignatureSpan">derby.Derby.prototype.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">derby.Derby.prototype.</span>_events
1.  object <span class="apidocSignatureSpan">derby.Derby.prototype.</span>domain

#### [module derby.Dom](#apidoc.module.derby.Dom)
1.  [function <span class="apidocSignatureSpan">derby.</span>Dom (controller)](#apidoc.element.derby.Dom.Dom)

#### [module derby.Dom.prototype](#apidoc.module.derby.Dom.prototype)
1.  [function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>_initListeners ()](#apidoc.element.derby.Dom.prototype._initListeners)
1.  [function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>_listenerIndex (domListener)](#apidoc.element.derby.Dom.prototype._listenerIndex)
1.  [function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>addListener (type, target, listener, useCapture)](#apidoc.element.derby.Dom.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>on (type, target, listener, useCapture)](#apidoc.element.derby.Dom.prototype.on)
1.  [function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>once (type, target, listener, useCapture)](#apidoc.element.derby.Dom.prototype.once)
1.  [function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>removeListener (type, target, listener, useCapture)](#apidoc.element.derby.Dom.prototype.removeListener)

#### [module derby.Page](#apidoc.module.derby.Page)
1.  [function <span class="apidocSignatureSpan">derby.</span>Page (app, model, req, res)](#apidoc.element.derby.Page.Page)

#### [module derby.Page.prototype](#apidoc.module.derby.Page.prototype)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_addContextListeners (eventModel)](#apidoc.element.derby.Page.prototype._addContextListeners)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_addListeners ()](#apidoc.element.derby.Page.prototype._addListeners)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_addModelListeners (eventModel)](#apidoc.element.derby.Page.prototype._addModelListeners)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_createContext ()](#apidoc.element.derby.Page.prototype._createContext)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_setRenderParams (ns)](#apidoc.element.derby.Page.prototype._setRenderParams)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_setRenderPrefix (ns)](#apidoc.element.derby.Page.prototype._setRenderPrefix)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>addListener (type, listener)](#apidoc.element.derby.Page.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>attach ()](#apidoc.element.derby.Page.prototype.attach)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>destroy ()](#apidoc.element.derby.Page.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>emit (type)](#apidoc.element.derby.Page.prototype.emit)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>emitCancellable ()](#apidoc.element.derby.Page.prototype.emitCancellable)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>emitDelayable ()](#apidoc.element.derby.Page.prototype.emitDelayable)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>eventNames ()](#apidoc.element.derby.Page.prototype.eventNames)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>get (viewName, ns, unescaped)](#apidoc.element.derby.Page.prototype.get)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>getFragment (viewName, ns)](#apidoc.element.derby.Page.prototype.getFragment)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>getMaxListeners ()](#apidoc.element.derby.Page.prototype.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>getView (viewName, ns)](#apidoc.element.derby.Page.prototype.getView)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>listenerCount (type)](#apidoc.element.derby.Page.prototype.listenerCount)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>listeners (type)](#apidoc.element.derby.Page.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>on (type, listener)](#apidoc.element.derby.Page.prototype.on)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>once (type, listener)](#apidoc.element.derby.Page.prototype.once)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>prependListener (type, listener)](#apidoc.element.derby.Page.prototype.prependListener)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.derby.Page.prototype.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>removeAllListeners (type)](#apidoc.element.derby.Page.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>removeListener (type, listener)](#apidoc.element.derby.Page.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>render (status, ns)](#apidoc.element.derby.Page.prototype.render)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>renderStatic (status, ns)](#apidoc.element.derby.Page.prototype.renderStatic)
1.  [function <span class="apidocSignatureSpan">derby.Page.prototype.</span>setMaxListeners (n)](#apidoc.element.derby.Page.prototype.setMaxListeners)
1.  undefined <span class="apidocSignatureSpan">derby.Page.prototype.</span>domain

#### [module derby.components](#apidoc.module.derby.components)
1.  [function <span class="apidocSignatureSpan">derby.components.</span>Component (parent, context, id, scope)](#apidoc.element.derby.components.Component)
1.  [function <span class="apidocSignatureSpan">derby.components.</span>ComponentFactory (constructor)](#apidoc.element.derby.components.ComponentFactory)
1.  [function <span class="apidocSignatureSpan">derby.components.</span>SingletonComponentFactory (constructor)](#apidoc.element.derby.components.SingletonComponentFactory)
1.  [function <span class="apidocSignatureSpan">derby.components.</span>createFactory (constructor)](#apidoc.element.derby.components.createFactory)

#### [module derby.documentListeners](#apidoc.module.derby.documentListeners)
1.  [function <span class="apidocSignatureSpan">derby.documentListeners.</span>add (doc)](#apidoc.element.derby.documentListeners.add)
1.  [function <span class="apidocSignatureSpan">derby.documentListeners.</span>inputSupportsSelection (input)](#apidoc.element.derby.documentListeners.inputSupportsSelection)

#### [module derby.eventmodel](#apidoc.module.derby.eventmodel)
1.  [function <span class="apidocSignatureSpan">derby.</span>eventmodel ()](#apidoc.element.derby.eventmodel.eventmodel)

#### [module derby.eventmodel.prototype](#apidoc.module.derby.eventmodel.prototype)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_addBinding (binding)](#apidoc.element.derby.eventmodel.prototype._addBinding)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_addItemContext (context)](#apidoc.element.derby.eventmodel.prototype._addItemContext)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_each (segments, pos, fn)](#apidoc.element.derby.eventmodel.prototype._each)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_insert (index, howMany)](#apidoc.element.derby.eventmodel.prototype._insert)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_move (from, to, howMany)](#apidoc.element.derby.eventmodel.prototype._move)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_remove (index, howMany)](#apidoc.element.derby.eventmodel.prototype._remove)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_removeItemContext (context)](#apidoc.element.derby.eventmodel.prototype._removeItemContext)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_set (previous, pass)](#apidoc.element.derby.eventmodel.prototype._set)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_updateArray (from, to)](#apidoc.element.derby.eventmodel.prototype._updateArray)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_updateChildItemContexts (from, to)](#apidoc.element.derby.eventmodel.prototype._updateChildItemContexts)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_updateObject ()](#apidoc.element.derby.eventmodel.prototype._updateObject)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>addBinding (segments, binding)](#apidoc.element.derby.eventmodel.prototype.addBinding)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>addItemContext (segments, context)](#apidoc.element.derby.eventmodel.prototype.addItemContext)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>arrayLookup (model, segmentsBefore, segmentsInside)](#apidoc.element.derby.eventmodel.prototype.arrayLookup)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>at (segments)](#apidoc.element.derby.eventmodel.prototype.at)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>child (segment)](#apidoc.element.derby.eventmodel.prototype.child)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>insert (segments, index, howMany)](#apidoc.element.derby.eventmodel.prototype.insert)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>isEmpty ()](#apidoc.element.derby.eventmodel.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>localUpdate (previous, pass)](#apidoc.element.derby.eventmodel.prototype.localUpdate)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>move (segments, from, to, howMany)](#apidoc.element.derby.eventmodel.prototype.move)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>mutate (segments, fn)](#apidoc.element.derby.eventmodel.prototype.mutate)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>refChild (ref)](#apidoc.element.derby.eventmodel.prototype.refChild)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>remove (segments, index, howMany)](#apidoc.element.derby.eventmodel.prototype.remove)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>removeBinding (binding)](#apidoc.element.derby.eventmodel.prototype.removeBinding)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>set (segments, previous, pass)](#apidoc.element.derby.eventmodel.prototype.set)
1.  [function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>update (previous, pass)](#apidoc.element.derby.eventmodel.prototype.update)

#### [module derby.files](#apidoc.module.derby.files)
1.  [function <span class="apidocSignatureSpan">derby.files.</span>cssCompiler (file, filename, options)](#apidoc.element.derby.files.cssCompiler)
1.  [function <span class="apidocSignatureSpan">derby.files.</span>htmlCompiler (file, filename)](#apidoc.element.derby.files.htmlCompiler)
1.  [function <span class="apidocSignatureSpan">derby.files.</span>loadStylesSync (app, sourceFilename, options)](#apidoc.element.derby.files.loadStylesSync)
1.  [function <span class="apidocSignatureSpan">derby.files.</span>loadViewsSync (app, sourceFilename, namespace)](#apidoc.element.derby.files.loadViewsSync)

#### [module derby.textDiff](#apidoc.module.derby.textDiff)
1.  [function <span class="apidocSignatureSpan">derby.textDiff.</span>onStringInsert (el, previous, index, text)](#apidoc.element.derby.textDiff.onStringInsert)
1.  [function <span class="apidocSignatureSpan">derby.textDiff.</span>onStringRemove (el, previous, index, howMany)](#apidoc.element.derby.textDiff.onStringRemove)
1.  [function <span class="apidocSignatureSpan">derby.textDiff.</span>onTextInput (model, segments, value)](#apidoc.element.derby.textDiff.onTextInput)



# <a name="apidoc.module.derby"></a>[module derby](#apidoc.module.derby)

#### <a name="apidoc.element.derby.App"></a>[function <span class="apidocSignatureSpan">derby.</span>App (derby, name, filename, options)](#apidoc.element.derby.App)
- description and source-code
```javascript
function App(derby, name, filename, options) {
  EventEmitter.call(this);
  this.derby = derby;
  this.name = name;
  this.filename = filename;
  this.scriptHash = '{{DERBY_SCRIPT_HASH}}';
  this.bundledAt = '{{DERBY_BUNDLED_AT}}';
  this.Page = createAppPage();
  this.proto = this.Page.prototype;
  this.views = new derbyTemplates.templates.Views();
  this.tracksRoutes = tracks.setup(this);
  this.model = null;
  this.page = null;
  this._init(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Controller"></a>[function <span class="apidocSignatureSpan">derby.</span>Controller (app, page, model)](#apidoc.element.derby.Controller)
- description and source-code
```javascript
function Controller(app, page, model) {
  EventEmitter.call(this);
  this.dom = new Dom(this);
  this.app = app;
  this.page = page;
  this.model = model;
  model.data.$controller = this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Derby"></a>[function <span class="apidocSignatureSpan">derby.</span>Derby ()](#apidoc.element.derby.Derby)
- description and source-code
```javascript
function Derby() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Dom"></a>[function <span class="apidocSignatureSpan">derby.</span>Dom (controller)](#apidoc.element.derby.Dom)
- description and source-code
```javascript
function Dom(controller) {
  this.controller = controller;
  this._listeners = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page"></a>[function <span class="apidocSignatureSpan">derby.</span>Page (app, model, req, res)](#apidoc.element.derby.Page)
- description and source-code
```javascript
function Page(app, model, req, res) {
  Controller.call(this, app, this, model);
  this.req = req;
  this.res = res;
  this.params = null;
  if (this.init) this.init(model);
  this.context = this._createContext();
  this._eventModel = null;
  this._removeModelListeners = null;
  this._components = {};
  this._addListeners();
}
```
- example usage
```shell
...
App.prototype.loadStyles = function() {};

App.prototype.createPage = function() {
if (this.page) {
  this.emit('destroyPage', this.page);
  this.page.destroy();
}
var page = new this.Page(this, this.model);
this.page = page;
return page;
};

App.prototype.onRoute = function(callback, page, next, done) {
if (this._waitForAttach) {
  // Cancel any routing before the initial page attachment. Instead, do a
...
```

#### <a name="apidoc.element.derby.eventmodel"></a>[function <span class="apidocSignatureSpan">derby.</span>eventmodel ()](#apidoc.element.derby.eventmodel)
- description and source-code
```javascript
function EventModel() {
  this.id = nextId++;

  // Most of these won't ever be filled in, so I'm just leaving them null.
  //
  // These contain our EventModel children.
  this.object = null;
  this.array = null;

  // This contains any EventModel children which have floating references.
  this.arrayByReference = null;

  // If the data stored here is ever used to lookup other values, this is an
  // object mapping remote child ID -> ref.
  //
  // Eg given x[y], y.refOut[x.id] = <Binding>
  this.refOut = null;

  // This is a map from ref id -> event model for events bound to this
  // EventModel but via a ref. We could just merge them into the main tree, but
  // this way they're easy to move.
  //
  // Eg, given x[y] (y=1), x.1.refChildren[ref id] is an EventModel.
  this.refChildren = null;

  this.bindings = null;

  // Item contexts are contexts which need their item number changed as this
  // EventModel object moves around its surrounding list.
  this.itemContexts = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.App"></a>[module derby.App](#apidoc.module.derby.App)

#### <a name="apidoc.element.derby.App.App"></a>[function <span class="apidocSignatureSpan">derby.</span>App (derby, name, filename, options)](#apidoc.element.derby.App.App)
- description and source-code
```javascript
function App(derby, name, filename, options) {
  EventEmitter.call(this);
  this.derby = derby;
  this.name = name;
  this.filename = filename;
  this.scriptHash = '{{DERBY_SCRIPT_HASH}}';
  this.bundledAt = '{{DERBY_BUNDLED_AT}}';
  this.Page = createAppPage();
  this.proto = this.Page.prototype;
  this.views = new derbyTemplates.templates.Views();
  this.tracksRoutes = tracks.setup(this);
  this.model = null;
  this.page = null;
  this._init(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.App.prototype"></a>[module derby.App.prototype](#apidoc.module.derby.App.prototype)

#### <a name="apidoc.element.derby.App.prototype._addAgent"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_addAgent (agent)](#apidoc.element.derby.App.prototype._addAgent)
- description and source-code
```javascript
_addAgent = function (agent) {
  this.agents[agent.clientId] = agent;
  var app = this;
  agent.stream.once('end', function() {
    delete app.agents[agent.clientId];
  });
}
```
- example usage
```shell
...
if (action === 'app') {
  if (message.name !== this.name) {
    return;
  }
  if (message.hash !== this.scriptHash) {
    return agent.send({derby: 'reload'});
  }
  this._addAgent(agent);
}
};

App.prototype._addAgent = function(agent) {
this.agents[agent.clientId] = agent;
var app = this;
agent.stream.once('end', function() {
...
```

#### <a name="apidoc.element.derby.App.prototype._autoRefresh"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_autoRefresh (backend)](#apidoc.element.derby.App.prototype._autoRefresh)
- description and source-code
```javascript
_autoRefresh = function (backend) {
  var agents = this.agents = {};
  var app = this;

  backend.use('receive', function(request, next) {
    var data = request.data;
    if (data.derby) {
      return app._handleMessage(request.agent, data.derby, data);
    }
    next();
  });
}
```
- example usage
```shell
...
};
App.prototype._finishInit = function() {
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
this.emit('model', this.model);
util.isProduction = data.nodeEnv === 'production';
if (!util.isProduction) this._autoRefresh();
this.model.unbundle(data);
var page = this.createPage();
page.params = this.model.get('$render.params');
this.emit('ready', page);
this._waitForAttach = false;
// Instead of attaching, do a route and render if a link was clicked before
// the page finished attaching
...
```

#### <a name="apidoc.element.derby.App.prototype._contentReady"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_contentReady ()](#apidoc.element.derby.App.prototype._contentReady)
- description and source-code
```javascript
_contentReady = function () {
  // Is the DOM ready to be used? Set to true once it occurs.
  var isReady = false;
  var app = this;

  // The ready event handler
  function onDOMContentLoaded() {
    if (document.addEventListener) {
      document.removeEventListener('DOMContentLoaded', onDOMContentLoaded, false);
    } else {
      // we're here because readyState !== 'loading' in oldIE
      // which is good enough for us to call the dom ready!
      document.detachEvent('onreadystatechange', onDOMContentLoaded);
    }
    onDOMReady();
  }

  // Handle when the DOM is ready
  function onDOMReady() {
    // Make sure that the DOM is not already loaded
    if (isReady) return;
    // Make sure body exists, at least, in case IE gets a little overzealous (ticket #5443).
    if (!document.body) return setTimeout(onDOMReady, 0);
    // Remember that the DOM is ready
    isReady = true;
    // Make sure this is always async and then finishin init
    setTimeout(function() {
      app._finishInit();
    }, 0);
  }

  // The DOM ready check for Internet Explorer
  function doScrollCheck() {
    if (isReady) return;
    try {
      // If IE is used, use the trick by Diego Perini
      // http://javascript.nwbox.com/IEContentLoaded/
      document.documentElement.doScroll('left');
    } catch (err) {
      setTimeout(doScrollCheck, 0);
      return;
    }
    // and execute any waiting functions
    onDOMReady();
  }

  // Catch cases where called after the browser event has already occurred.
  if (document.readyState !== 'loading') return onDOMReady();

  // Mozilla, Opera and webkit nightlies currently support this event
  if (document.addEventListener) {
    // Use the handy event callback
    document.addEventListener('DOMContentLoaded', onDOMContentLoaded, false);
    // A fallback to window.onload, that will always work
    window.addEventListener('load', onDOMContentLoaded, false);
    // If IE event model is used
  } else if (document.attachEvent) {
    // ensure firing before onload,
    // maybe late but safe also for iframes
    document.attachEvent('onreadystatechange', onDOMContentLoaded);
    // A fallback to window.onload, that will always work
    window.attachEvent('onload', onDOMContentLoaded);
    // If IE and not a frame
    // continually check to see if the document is ready
    var toplevel;
    try {
      toplevel = window.frameElement == null;
    } catch (err) {}
    if (document.documentElement.doScroll && toplevel) {
      doScrollCheck();
    }
  }
}
```
- example usage
```shell
...
App.prototype._init = function() {
this._waitForAttach = true;
this._cancelAttach = false;
this.model = new this.derby.Model();
serializedViews(derbyTemplates, this.views);
// Must init async so that app.on('model') listeners can be added.
// Must also wait for content ready so that bundle is fully downloaded.
this._contentReady();
};
App.prototype._finishInit = function() {
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
this.emit('model', this.model);
util.isProduction = data.nodeEnv === 'production';
...
```

#### <a name="apidoc.element.derby.App.prototype._finishInit"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_finishInit ()](#apidoc.element.derby.App.prototype._finishInit)
- description and source-code
```javascript
_finishInit = function () {
  var script = this._getScript();
  var data = JSON.parse(script.nextSibling.innerHTML);
  this.model.createConnection(data);
  this.emit('model', this.model);
  util.isProduction = data.nodeEnv === 'production';
  if (!util.isProduction) this._autoRefresh();
  this.model.unbundle(data);
  var page = this.createPage();
  page.params = this.model.get('$render.params');
  this.emit('ready', page);
  this._waitForAttach = false;
  // Instead of attaching, do a route and render if a link was clicked before
  // the page finished attaching
  if (this._cancelAttach) {
    this.history.refresh();
    return;
  }
  // Since an attachment failure is *fatal* and could happen as a result of a
  // browser extension like AdBlock, an invalid template, or a small bug in
  // Derby or Saddle, re-render from scratch on production failures
  if (util.isProduction) {
    try {
      page.attach();
    } catch (err) {
      this.history.refresh();
      console.warn('attachment error', err.stack);
    }
  } else {
    page.attach();
  }
  this.emit('load', page);
}
```
- example usage
```shell
...
  if (isReady) return;
  // Make sure body exists, at least, in case IE gets a little overzealous (ticket #5443).
  if (!document.body) return setTimeout(onDOMReady, 0);
  // Remember that the DOM is ready
  isReady = true;
  // Make sure this is always async and then finishin init
  setTimeout(function() {
    app._finishInit();
  }, 0);
}

// The DOM ready check for Internet Explorer
function doScrollCheck() {
  if (isReady) return;
  try {
...
```

#### <a name="apidoc.element.derby.App.prototype._getScript"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_getScript ()](#apidoc.element.derby.App.prototype._getScript)
- description and source-code
```javascript
_getScript = function () {
  return document.querySelector('script[data-derby-app]');
}
```
- example usage
```shell
...
this.model = new this.derby.Model();
serializedViews(derbyTemplates, this.views);
// Must init async so that app.on('model') listeners can be added.
// Must also wait for content ready so that bundle is fully downloaded.
this._contentReady();
};
App.prototype._finishInit = function() {
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
this.emit('model', this.model);
util.isProduction = data.nodeEnv === 'production';
if (!util.isProduction) this._autoRefresh();
this.model.unbundle(data);
var page = this.createPage();
...
```

#### <a name="apidoc.element.derby.App.prototype._handleMessage"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_handleMessage (agent, action, message)](#apidoc.element.derby.App.prototype._handleMessage)
- description and source-code
```javascript
_handleMessage = function (agent, action, message) {
  if (action === 'app') {
    if (message.name !== this.name) {
      return;
    }
    if (message.hash !== this.scriptHash) {
      return agent.send({derby: 'reload'});
    }
    this._addAgent(agent);
  }
}
```
- example usage
```shell
...
    hash: app.scriptHash
  });
});
connection.on('receive', function(request) {
  if (request.data.derby) {
    var message = request.data;
    request.data = null;
    app._handleMessage(message.derby, message);
  }
});
};

App.prototype._handleMessage = function(action, message) {
if (action === 'refreshViews') {
  var fn = new Function('return ' + message.views)(); // jshint ignore:line
...
```

#### <a name="apidoc.element.derby.App.prototype._init"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_init (options)](#apidoc.element.derby.App.prototype._init)
- description and source-code
```javascript
_init = function (options) {
  this.scriptFilename = null;
  this.scriptMapFilename = null;
  this.scriptBaseUrl = (options && options.scriptBaseUrl) || '';
  this.scriptMapBaseUrl = (options && options.scriptMapBaseUrl) || '';
  this.scriptCrossOrigin = (options && options.scriptCrossOrigin) || false;
  this.scriptUrl = null;
  this.scriptMapUrl = null;
  this.agents = null;
  this.styleExtensions = STYLE_EXTENSIONS.slice();
  this.viewExtensions = VIEW_EXTENSIONS.slice();
  this.compilers = util.copyObject(COMPILERS);

  this.serializedDir = path.dirname(this.filename || '') + '/derby-serialized';
  this.serializedBase = this.serializedDir + '/' + this.name;
  if (fs.existsSync(this.serializedBase + '.json')) {
    this.deserialize();
    this.loadViews = function() {};
    this.loadStyles = function() {};
    return;
  }
  this.views.register('Page',
    '<!DOCTYPE html>' +
    '<meta charset="utf-8">' +
    '<view is="{{$render.prefix}}TitleElement"></view>' +
    '<view is="{{$render.prefix}}Styles"></view>' +
    '<view is="{{$render.prefix}}Head"></view>' +
    '<view is="{{$render.prefix}}BodyElement"></view>',
    {serverOnly: true}
  );
  this.views.register('TitleElement',
    '<title><view is="{{$render.prefix}}Title"></view></title>'
  );
  this.views.register('BodyElement',
    '<body class="{{$bodyClass($render.ns)}}">' +
      '<view is="{{$render.prefix}}Body"></view>'
  );
  this.views.register('Title', 'Derby App');
  this.views.register('Styles', '', {serverOnly: true});
  this.views.register('Head', '', {serverOnly: true});
  this.views.register('Body', '');
  this.views.register('Tail', '');
}
```
- example usage
```shell
...
this.bundledAt = '{{DERBY_BUNDLED_AT}}';
this.Page = createAppPage();
this.proto = this.Page.prototype;
this.views = new derbyTemplates.templates.Views();
this.tracksRoutes = tracks.setup(this);
this.model = null;
this.page = null;
this._init(options);
}

function createAppPage() {
// Inherit from Page so that we can add controller functions as prototype
// methods on this app's pages
function AppPage() {
  Page.apply(this, arguments);
...
```

#### <a name="apidoc.element.derby.App.prototype._loadStyles"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_loadStyles (filename, options)](#apidoc.element.derby.App.prototype._loadStyles)
- description and source-code
```javascript
_loadStyles = function (filename, options) {
  var styles = files.loadStylesSync(this, filename, options);

  var filepath = '';
  if (!util.isProduction) {
<span class="apidocCodeCommentSpan">    /**
     * Mark the path to file as an attribute
     * Used in development to add event watchers and autorefreshing of styles
     * SEE: local file, method this._watchStyles
     * SEE: file ./App.js, method App._autoRefresh()
     */
</span>    filepath = ' data-filename="' + filename + '"';
  }
  var source = '<style' + filepath + '>' + styles.css + '</style>';

  this.views.register(filename, source, {
    serverOnly: true
  });

  if (!util.isProduction) {
    this._watchStyles(styles.files, filename, options);
  }

  return styles;
}
```
- example usage
```shell
...
  }
  if (!util.isProduction) this._watchViews(data.files, filename, namespace);
  // Make chainable
  return this;
};

App.prototype.loadStyles = function(filename, options) {
  this._loadStyles(filename, options);
  var stylesView = this.views.find('Styles');
  stylesView.source += '<view is="' + filename + '"></view>';
  // Make chainable
  return this;
};

App.prototype._loadStyles = function(filename, options) {
...
```

#### <a name="apidoc.element.derby.App.prototype._refreshClients"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_refreshClients ()](#apidoc.element.derby.App.prototype._refreshClients)
- description and source-code
```javascript
_refreshClients = function () {
  if (!this.agents) return;
  var views = this.views.serialize({minify: true});
  var message = {
    derby: 'refreshViews',
    views: views
  };
  for (var id in this.agents) {
    this.agents[id].send(message);
  }
}
```
- example usage
```shell
...
App.prototype._watchViews = function(filenames, filename, namespace) {
var app = this;
var watcher = chokidar.watch(filenames);
watcher.on('change', function() {
  watcher.close();
  app.loadViews(filename, namespace);
  app._updateScriptViews();
  app._refreshClients();
});
};

App.prototype._watchStyles = function(filenames, filename, options) {
var app = this;
var watcher = chokidar.watch(filenames);
watcher.on('change', function() {
...
```

#### <a name="apidoc.element.derby.App.prototype._refreshStyles"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_refreshStyles (filename, styles)](#apidoc.element.derby.App.prototype._refreshStyles)
- description and source-code
```javascript
_refreshStyles = function (filename, styles) {
  if (!this.agents) return;
  var data = {filename: filename, css: styles.css};
  var message = {
    derby: 'refreshStyles',
    filename: filename,
    css: styles.css
  };
  for (var id in this.agents) {
    this.agents[id].send(message);
  }
}
```
- example usage
```shell
...
App.prototype._watchStyles = function(filenames, filename, options) {
var app = this;
var watcher = chokidar.watch(filenames);
watcher.on('change', function() {
  watcher.close();
  var styles = app._loadStyles(filename, options);
  app._updateScriptViews();
  app._refreshStyles(filename, styles);
});
};

App.prototype._watchBundle = function(filenames) {
if (!process.send) return;
var app = this;
var watcher = chokidar.watch(filenames);
...
```

#### <a name="apidoc.element.derby.App.prototype._updateScriptViews"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_updateScriptViews ()](#apidoc.element.derby.App.prototype._updateScriptViews)
- description and source-code
```javascript
_updateScriptViews = function () {
  if (!this.scriptFilename) return;
  var script = fs.readFileSync(this.scriptFilename, 'utf8');
  var i = script.indexOf('/*DERBY_SERIALIZED_VIEWS*/');
  var before = script.slice(0, i);
  var i = script.indexOf('/*DERBY_SERIALIZED_VIEWS_END*/');
  var after = script.slice(i + 30);
  var viewsSource = this._viewsSource();
  fs.writeFileSync(this.scriptFilename, before + viewsSource + after, 'utf8');
}
```
- example usage
```shell
...

App.prototype._watchViews = function(filenames, filename, namespace) {
var app = this;
var watcher = chokidar.watch(filenames);
watcher.on('change', function() {
  watcher.close();
  app.loadViews(filename, namespace);
  app._updateScriptViews();
  app._refreshClients();
});
};

App.prototype._watchStyles = function(filenames, filename, options) {
var app = this;
var watcher = chokidar.watch(filenames);
...
```

#### <a name="apidoc.element.derby.App.prototype._viewsSource"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_viewsSource (options)](#apidoc.element.derby.App.prototype._viewsSource)
- description and source-code
```javascript
_viewsSource = function (options) {
  return '/*DERBY_SERIALIZED_VIEWS*/' +
    'module.exports = ' + this.views.serialize(options) + ';' +
    '/*DERBY_SERIALIZED_VIEWS_END*/';
}
```
- example usage
```shell
...
  cb = options;
  options = null;
}
options || (options = {});
if (options.minify == null) options.minify = util.isProduction;
// Turn all of the app's currently registered views into a javascript
// function that can recreate them in the client
var viewsSource = this._viewsSource(options);
var bundleFiles = [];
backend.once('bundle', function(bundle) {
  bundle.require(path.dirname(__dirname), {expose: 'derby'});
  // Hack to inject the views script into the Browserify bundle by replacing
  // the empty _views.js file with the generated source
  var viewsFilename = require.resolve('./_views');
  bundle.transform(function(filename) {
...
```

#### <a name="apidoc.element.derby.App.prototype._watchBundle"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_watchBundle (filenames)](#apidoc.element.derby.App.prototype._watchBundle)
- description and source-code
```javascript
_watchBundle = function (filenames) {
  if (!process.send) return;
  var app = this;
  var watcher = chokidar.watch(filenames);
  watcher.on('change', function() {
    watcher.close();
    process.send({type: 'reload'});
  });
}
```
- example usage
```shell
...
backend.bundle(app.filename, options, function(err, source, map) {
  if (err) return cb(err);
  app.scriptHash = crypto.createHash('md5').update(source).digest('hex');
  source = source.replace('{{DERBY_SCRIPT_HASH}}', app.scriptHash);
  source = source.replace(/['"]{{DERBY_BUNDLED_AT}}['"]/, Date.now());
  if (!util.isProduction) {
    app._autoRefresh(backend);
    app._watchBundle(bundleFiles);
  }
  cb(null, source, map);
});
};

App.prototype.writeScripts = function(backend, dir, options, cb) {
var app = this;
...
```

#### <a name="apidoc.element.derby.App.prototype._watchStyles"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_watchStyles (filenames, filename, options)](#apidoc.element.derby.App.prototype._watchStyles)
- description and source-code
```javascript
_watchStyles = function (filenames, filename, options) {
  var app = this;
  var watcher = chokidar.watch(filenames);
  watcher.on('change', function() {
    watcher.close();
    var styles = app._loadStyles(filename, options);
    app._updateScriptViews();
    app._refreshStyles(filename, styles);
  });
}
```
- example usage
```shell
...
var source = '<style' + filepath + '>' + styles.css + '</style>';

this.views.register(filename, source, {
  serverOnly: true
});

if (!util.isProduction) {
  this._watchStyles(styles.files, filename, options);
}

return styles;
};

App.prototype._watchViews = function(filenames, filename, namespace) {
var app = this;
...
```

#### <a name="apidoc.element.derby.App.prototype._watchViews"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>_watchViews (filenames, filename, namespace)](#apidoc.element.derby.App.prototype._watchViews)
- description and source-code
```javascript
_watchViews = function (filenames, filename, namespace) {
  var app = this;
  var watcher = chokidar.watch(filenames);
  watcher.on('change', function() {
    watcher.close();
    app.loadViews(filename, namespace);
    app._updateScriptViews();
    app._refreshClients();
  });
}
```
- example usage
```shell
...

App.prototype.loadViews = function(filename, namespace) {
var data = files.loadViewsSync(this, filename, namespace);
for (var i = 0, len = data.views.length; i < len; i++) {
  var item = data.views[i];
  this.views.register(item.name, item.source, item.options);
}
if (!util.isProduction) this._watchViews(data.files, filename, namespace);
// Make chainable
return this;
};

App.prototype.loadStyles = function(filename, options) {
this._loadStyles(filename, options);
var stylesView = this.views.find('Styles');
...
```

#### <a name="apidoc.element.derby.App.prototype.addListener"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>addListener (type, listener)](#apidoc.element.derby.App.prototype.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...

Dom.prototype.once = function(type, target, listener, useCapture) {
  if (typeof target === 'function') {
    useCapture = listener;
    listener = target;
    target = document;
  }
  this.addListener(type, target, wrappedListener, useCapture);
  var dom = this;
  function wrappedListener() {
    dom.removeListener(type, target, wrappedListener, useCapture);
    return listener.apply(this, arguments);
  }
};
...
```

#### <a name="apidoc.element.derby.App.prototype.bundle"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>bundle (backend, options, cb)](#apidoc.element.derby.App.prototype.bundle)
- description and source-code
```javascript
bundle = function (backend, options, cb) {
  var app = this;
  if (typeof options === 'function') {
    cb = options;
    options = null;
  }
  options || (options = {});
  if (options.minify == null) options.minify = util.isProduction;
  // Turn all of the app's currently registered views into a javascript
  // function that can recreate them in the client
  var viewsSource = this._viewsSource(options);
  var bundleFiles = [];
  backend.once('bundle', function(bundle) {
    bundle.require(path.dirname(__dirname), {expose: 'derby'});
    // Hack to inject the views script into the Browserify bundle by replacing
    // the empty _views.js file with the generated source
    var viewsFilename = require.resolve('./_views');
    bundle.transform(function(filename) {
      if (filename !== viewsFilename) return through();
      return through(
        function write() {}
      , function end() {
          this.queue(viewsSource);
          this.queue(null);
        }
      );
    }, {global: true});
    bundle.on('file', function(filename) {
      bundleFiles.push(filename);
    });
    app.emit('bundle', bundle);
  });
  backend.bundle(app.filename, options, function(err, source, map) {
    if (err) return cb(err);
    app.scriptHash = crypto.createHash('md5').update(source).digest('hex');
    source = source.replace('{{DERBY_SCRIPT_HASH}}', app.scriptHash);
    source = source.replace(/['"]{{DERBY_BUNDLED_AT}}['"]/, Date.now());
    if (!util.isProduction) {
      app._autoRefresh(backend);
      app._watchBundle(bundleFiles);
    }
    cb(null, source, map);
  });
}
```
- example usage
```shell
...
    );
  }, {global: true});
  bundle.on('file', function(filename) {
    bundleFiles.push(filename);
  });
  app.emit('bundle', bundle);
});
backend.bundle(app.filename, options, function(err, source, map) {
  if (err) return cb(err);
  app.scriptHash = crypto.createHash('md5').update(source).digest('hex');
  source = source.replace('{{DERBY_SCRIPT_HASH}}', app.scriptHash);
  source = source.replace(/['"]{{DERBY_BUNDLED_AT}}['"]/, Date.now());
  if (!util.isProduction) {
    app._autoRefresh(backend);
    app._watchBundle(bundleFiles);
...
```

#### <a name="apidoc.element.derby.App.prototype.component"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>component (viewName, constructor)](#apidoc.element.derby.App.prototype.component)
- description and source-code
```javascript
component = function (viewName, constructor) {
  if (typeof viewName === 'function') {
    constructor = viewName;
    viewName = null;
  }

  // Inherit from Component
  extendComponent(constructor);

  // Load template view from filename
  if (constructor.prototype.view) {
    var viewFilename = constructor.prototype.view;
    viewName = constructor.prototype.name || path.basename(viewFilename, '.html');
    this.loadViews(viewFilename, viewName);

  } else if (!viewName) {
    if (constructor.prototype.name) {
      viewName = constructor.prototype.name;
      var view = this.views.register(viewName);
      view.template = templates.emptyTemplate;
    } else {
      throw new Error('No view name specified for component');
    }
  }

  // Associate the appropriate view with the component type
  var view = this.views.find(viewName);
  if (!view) {
    var message = this.views.findErrorMessage(viewName);
    throw new Error(message);
  }
  view.componentFactory = createFactory(constructor);

  // Make chainable
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.createPage"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>createPage (req, res, next)](#apidoc.element.derby.App.prototype.createPage)
- description and source-code
```javascript
createPage = function (req, res, next) {
  var model = req.model || new racer.Model();
  this.emit('model', model);
  var page = new this.Page(this, model, req, res);
  if (next) {
    model.on('error', function(err){
      model.hasErrored = true;
      next(err);
    });
    page.on('error', next);
  }
  return page;
}
```
- example usage
```shell
...
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
this.emit('model', this.model);
util.isProduction = data.nodeEnv === 'production';
if (!util.isProduction) this._autoRefresh();
this.model.unbundle(data);
var page = this.createPage();
page.params = this.model.get('$render.params');
this.emit('ready', page);
this._waitForAttach = false;
// Instead of attaching, do a route and render if a link was clicked before
// the page finished attaching
if (this._cancelAttach) {
  this.history.refresh();
...
```

#### <a name="apidoc.element.derby.App.prototype.deserialize"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>deserialize ()](#apidoc.element.derby.App.prototype.deserialize)
- description and source-code
```javascript
deserialize = function () {
  var serializedViews = require(this.serializedBase + '.views.js');
  var serialized = require(this.serializedBase + '.json');
  serializedViews(derbyTemplates, this.views);
  this.scriptUrl = (this.scriptBaseUrl || serialized.scriptBaseUrl) + serialized.scriptUrl;
  this.scriptMapUrl = (this.scriptMapBaseUrl || serialized.scriptMapBaseUrl) + serialized.scriptMapUrl;
}
```
- example usage
```shell
...
this.styleExtensions = STYLE_EXTENSIONS.slice();
this.viewExtensions = VIEW_EXTENSIONS.slice();
this.compilers = util.copyObject(COMPILERS);

this.serializedDir = path.dirname(this.filename || '') + '/derby-serialized';
this.serializedBase = this.serializedDir + '/' + this.name;
if (fs.existsSync(this.serializedBase + '.json')) {
  this.deserialize();
  this.loadViews = function() {};
  this.loadStyles = function() {};
  return;
}
this.views.register('Page',
  '<!DOCTYPE html>' +
  '<meta charset="utf-8">' +
...
```

#### <a name="apidoc.element.derby.App.prototype.emit"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>emit (type)](#apidoc.element.derby.App.prototype.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
...
// Must also wait for content ready so that bundle is fully downloaded.
this._contentReady();
};
App.prototype._finishInit = function() {
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
this.emit('model', this.model);
util.isProduction = data.nodeEnv === 'production';
if (!util.isProduction) this._autoRefresh();
this.model.unbundle(data);
var page = this.createPage();
page.params = this.model.get('$render.params');
this.emit('ready', page);
this._waitForAttach = false;
...
```

#### <a name="apidoc.element.derby.App.prototype.eventNames"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>eventNames ()](#apidoc.element.derby.App.prototype.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.getMaxListeners"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>getMaxListeners ()](#apidoc.element.derby.App.prototype.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.listenerCount"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>listenerCount (type)](#apidoc.element.derby.App.prototype.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.listeners"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>listeners (type)](#apidoc.element.derby.App.prototype.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.loadStyles"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>loadStyles (filename, options)](#apidoc.element.derby.App.prototype.loadStyles)
- description and source-code
```javascript
loadStyles = function (filename, options) {
  this._loadStyles(filename, options);
  var stylesView = this.views.find('Styles');
  stylesView.source += '<view is="' + filename + '"></view>';
  // Make chainable
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.loadViews"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>loadViews (filename, namespace)](#apidoc.element.derby.App.prototype.loadViews)
- description and source-code
```javascript
loadViews = function (filename, namespace) {
  var data = files.loadViewsSync(this, filename, namespace);
  for (var i = 0, len = data.views.length; i < len; i++) {
    var item = data.views[i];
    this.views.register(item.name, item.source, item.options);
  }
  if (!util.isProduction) this._watchViews(data.files, filename, namespace);
  // Make chainable
  return this;
}
```
- example usage
```shell
...
};

App.prototype._watchViews = function(filenames, filename, namespace) {
var app = this;
var watcher = chokidar.watch(filenames);
watcher.on('change', function() {
  watcher.close();
  app.loadViews(filename, namespace);
  app._updateScriptViews();
  app._refreshClients();
});
};

App.prototype._watchStyles = function(filenames, filename, options) {
var app = this;
...
```

#### <a name="apidoc.element.derby.App.prototype.on"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>on (type, listener)](#apidoc.element.derby.App.prototype.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...

// Overriden on server
App.prototype._init = function() {
this._waitForAttach = true;
this._cancelAttach = false;
this.model = new this.derby.Model();
serializedViews(derbyTemplates, this.views);
// Must init async so that app.on('model') listeners can be added.
// Must also wait for content ready so that bundle is fully downloaded.
this._contentReady();
};
App.prototype._finishInit = function() {
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
...
```

#### <a name="apidoc.element.derby.App.prototype.onRoute"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>onRoute (callback, page, next, done)](#apidoc.element.derby.App.prototype.onRoute)
- description and source-code
```javascript
onRoute = function (callback, page, next, done) {
  if (this._waitForAttach) {
    // Cancel any routing before the initial page attachment. Instead, do a
    // render once derby is ready
    this._cancelAttach = true;
    return;
  }
  this.emit('route', page);
  // HACK: To update render in transitional routes
  page.model.set('$render.params', page.params);
  page.model.set('$render.url', page.params.url);
  page.model.set('$render.query', page.params.query);
  // If transitional
  if (done) {
    var app = this;
    var _done = function() {
      app.emit('routeDone', page, 'transition');
      done();
    };
    callback.call(page, page, page.model, page.params, next, _done);
    return;
  }
  callback.call(page, page, page.model, page.params, next);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.once"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>once (type, listener)](#apidoc.element.derby.App.prototype.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
...
}
options || (options = {});
if (options.minify == null) options.minify = util.isProduction;
// Turn all of the app's currently registered views into a javascript
// function that can recreate them in the client
var viewsSource = this._viewsSource(options);
var bundleFiles = [];
backend.once('bundle', function(bundle) {
  bundle.require(path.dirname(__dirname), {expose: 'derby'});
  // Hack to inject the views script into the Browserify bundle by replacing
  // the empty _views.js file with the generated source
  var viewsFilename = require.resolve('./_views');
  bundle.transform(function(filename) {
    if (filename !== viewsFilename) return through();
    return through(
...
```

#### <a name="apidoc.element.derby.App.prototype.prependListener"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>prependListener (type, listener)](#apidoc.element.derby.App.prototype.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.prependOnceListener"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.derby.App.prototype.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>removeAllListeners (type)](#apidoc.element.derby.App.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>removeListener (type, listener)](#apidoc.element.derby.App.prototype.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
...
  useCapture = listener;
  listener = target;
  target = document;
}
this.addListener(type, target, wrappedListener, useCapture);
var dom = this;
function wrappedListener() {
  dom.removeListener(type, target, wrappedListener, useCapture);
  return listener.apply(this, arguments);
}
};

Dom.prototype.removeListener = function(type, target, listener, useCapture) {
if (typeof target === 'function') {
  useCapture = listener;
...
```

#### <a name="apidoc.element.derby.App.prototype.serialize"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>serialize ()](#apidoc.element.derby.App.prototype.serialize)
- description and source-code
```javascript
serialize = function () {
  if (!fs.existsSync(this.serializedDir)) {
    fs.mkdirSync(this.serializedDir);
  }
  // Don't minify the views (which doesn't include template source), since this
  // is for use on the server
  var viewsSource = this._viewsSource({server: true, minify: true});
  fs.writeFileSync(this.serializedBase + '.views.js', viewsSource, 'utf8');
  var scriptUrl = (this.scriptUrl.indexOf(this.scriptBaseUrl) === 0) ?
    this.scriptUrl.slice(this.scriptBaseUrl.length) :
    this.scriptUrl;
  var scriptMapUrl = (this.scriptMapUrl.indexOf(this.scriptMapBaseUrl) === 0) ?
    this.scriptMapUrl.slice(this.scriptMapBaseUrl.length) :
    this.scriptMapUrl;
  var serialized = JSON.stringify({
    scriptBaseUrl: this.scriptBaseUrl
  , scriptMapBaseUrl: this.scriptMapBaseUrl
  , scriptUrl: scriptUrl
  , scriptMapUrl: scriptMapUrl
  });
  fs.writeFileSync(this.serializedBase + '.json', serialized, 'utf8');
}
```
- example usage
```shell
...
  }
  cb && cb();
});
};

App.prototype._viewsSource = function(options) {
return '/*DERBY_SERIALIZED_VIEWS*/' +
  'module.exports = ' + this.views.serialize(options) + ';' +
  '/*DERBY_SERIALIZED_VIEWS_END*/';
};

App.prototype.serialize = function() {
if (!fs.existsSync(this.serializedDir)) {
  fs.mkdirSync(this.serializedDir);
}
...
```

#### <a name="apidoc.element.derby.App.prototype.serverUse"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>serverUse (module, id, options)](#apidoc.element.derby.App.prototype.serverUse)
- description and source-code
```javascript
function serverUse(module, id, options) {
  if (!isServer) return this;
  var plugin = module.require(id);
  return this.use(plugin, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>setMaxListeners (n)](#apidoc.element.derby.App.prototype.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.App.prototype.use"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>use (plugin, options)](#apidoc.element.derby.App.prototype.use)
- description and source-code
```javascript
function use(plugin, options) {
  // Don't include a plugin more than once
  var plugins = this._plugins || (this._plugins = []);
  if (plugins.indexOf(plugin) === -1) {
    plugins.push(plugin);
    plugin(this, options);
  }
  return this;
}
```
- example usage
```shell
...
  fs.writeFileSync(this.scriptFilename, before + viewsSource + after, 'utf8');
};

App.prototype._autoRefresh = function(backend) {
  var agents = this.agents = {};
  var app = this;

  backend.use('receive', function(request, next) {
    var data = request.data;
    if (data.derby) {
      return app._handleMessage(request.agent, data.derby, data);
    }
    next();
  });
};
...
```

#### <a name="apidoc.element.derby.App.prototype.writeScripts"></a>[function <span class="apidocSignatureSpan">derby.App.prototype.</span>writeScripts (backend, dir, options, cb)](#apidoc.element.derby.App.prototype.writeScripts)
- description and source-code
```javascript
writeScripts = function (backend, dir, options, cb) {
  var app = this;
  this.bundle(backend, options, function(err, source, map) {
    if (err) return cb(err);
    dir = path.join(dir, 'derby');
    if (!fs.existsSync(dir)) fs.mkdirSync(dir);
    var filename = app.name + '-' + app.scriptHash;
    var base = path.join(dir, filename);
    app.scriptUrl = app.scriptBaseUrl + '/derby/' + filename + '.js';

    // Write current map and bundle files
    if (!(options && options.disableScriptMap)) {
      app.scriptMapUrl = app.scriptMapBaseUrl +  '/derby/' + filename + '.map.json';
      source += '\n//# sourceMappingURL=' + app.scriptMapUrl;
      app.scriptMapFilename = base + '.map.json';
      fs.writeFileSync(app.scriptMapFilename, map, 'utf8');
    }
    app.scriptFilename = base + '.js';
    fs.writeFileSync(app.scriptFilename, source, 'utf8');

    // Delete app bundles with same name in development so files don't
    // accumulate. Don't do this automatically in production, since there could
    // be race conditions with multiple processes intentionally running
    // different versions of the app in parallel out of the same directory,
    // such as during a rolling restart.
    if (!util.isProduction) {
      var appPrefix = app.name + '-';
      var currentBundlePrefix = appPrefix + app.scriptHash;
      var filenames = fs.readdirSync(dir);
      for (var i = 0; i < filenames.length; i++) {
        var filename = filenames[i];
        if (filename.indexOf(appPrefix) !== 0) {
          // Not a bundle for this app, skip.
          continue;
        }
        if (filename.indexOf(currentBundlePrefix) === 0) {
          // Current (newly written) bundle for this app, skip.
          continue;
        }
        // Older bundle for this app, clean it up.
        var oldFilename = path.join(dir, filename);
        fs.unlinkSync(oldFilename);
      }
    }
    cb && cb();
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.Controller"></a>[module derby.Controller](#apidoc.module.derby.Controller)

#### <a name="apidoc.element.derby.Controller.Controller"></a>[function <span class="apidocSignatureSpan">derby.</span>Controller (app, page, model)](#apidoc.element.derby.Controller.Controller)
- description and source-code
```javascript
function Controller(app, page, model) {
  EventEmitter.call(this);
  this.dom = new Dom(this);
  this.app = app;
  this.page = page;
  this.model = model;
  model.data.$controller = this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.Controller.prototype"></a>[module derby.Controller.prototype](#apidoc.module.derby.Controller.prototype)

#### <a name="apidoc.element.derby.Controller.prototype.addListener"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>addListener (type, listener)](#apidoc.element.derby.Controller.prototype.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...

Dom.prototype.once = function(type, target, listener, useCapture) {
  if (typeof target === 'function') {
    useCapture = listener;
    listener = target;
    target = document;
  }
  this.addListener(type, target, wrappedListener, useCapture);
  var dom = this;
  function wrappedListener() {
    dom.removeListener(type, target, wrappedListener, useCapture);
    return listener.apply(this, arguments);
  }
};
...
```

#### <a name="apidoc.element.derby.Controller.prototype.emit"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>emit (type)](#apidoc.element.derby.Controller.prototype.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
...
// Must also wait for content ready so that bundle is fully downloaded.
this._contentReady();
};
App.prototype._finishInit = function() {
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
this.emit('model', this.model);
util.isProduction = data.nodeEnv === 'production';
if (!util.isProduction) this._autoRefresh();
this.model.unbundle(data);
var page = this.createPage();
page.params = this.model.get('$render.params');
this.emit('ready', page);
this._waitForAttach = false;
...
```

#### <a name="apidoc.element.derby.Controller.prototype.emitCancellable"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>emitCancellable ()](#apidoc.element.derby.Controller.prototype.emitCancellable)
- description and source-code
```javascript
emitCancellable = function () {
  var cancelled = false;
  function cancel() {
    cancelled = true;
  }

  var args = Array.prototype.slice.call(arguments);
  args.push(cancel);
  this.emit.apply(this, args);

  return cancelled;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Controller.prototype.emitDelayable"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>emitDelayable ()](#apidoc.element.derby.Controller.prototype.emitDelayable)
- description and source-code
```javascript
emitDelayable = function () {
  var args = Array.prototype.slice.call(arguments);
  var callback = args.pop();

  var delayed = false;
  function delay() {
    delayed = true;
    return callback;
  }

  args.push(delay);
  this.emit.apply(this, args);
  if (!delayed) callback();

  return delayed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Controller.prototype.eventNames"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>eventNames ()](#apidoc.element.derby.Controller.prototype.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Controller.prototype.getMaxListeners"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>getMaxListeners ()](#apidoc.element.derby.Controller.prototype.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Controller.prototype.listenerCount"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>listenerCount (type)](#apidoc.element.derby.Controller.prototype.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Controller.prototype.listeners"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>listeners (type)](#apidoc.element.derby.Controller.prototype.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Controller.prototype.on"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>on (type, listener)](#apidoc.element.derby.Controller.prototype.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...

// Overriden on server
App.prototype._init = function() {
this._waitForAttach = true;
this._cancelAttach = false;
this.model = new this.derby.Model();
serializedViews(derbyTemplates, this.views);
// Must init async so that app.on('model') listeners can be added.
// Must also wait for content ready so that bundle is fully downloaded.
this._contentReady();
};
App.prototype._finishInit = function() {
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
...
```

#### <a name="apidoc.element.derby.Controller.prototype.once"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>once (type, listener)](#apidoc.element.derby.Controller.prototype.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
...
}
options || (options = {});
if (options.minify == null) options.minify = util.isProduction;
// Turn all of the app's currently registered views into a javascript
// function that can recreate them in the client
var viewsSource = this._viewsSource(options);
var bundleFiles = [];
backend.once('bundle', function(bundle) {
  bundle.require(path.dirname(__dirname), {expose: 'derby'});
  // Hack to inject the views script into the Browserify bundle by replacing
  // the empty _views.js file with the generated source
  var viewsFilename = require.resolve('./_views');
  bundle.transform(function(filename) {
    if (filename !== viewsFilename) return through();
    return through(
...
```

#### <a name="apidoc.element.derby.Controller.prototype.prependListener"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>prependListener (type, listener)](#apidoc.element.derby.Controller.prototype.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Controller.prototype.prependOnceListener"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.derby.Controller.prototype.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Controller.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>removeAllListeners (type)](#apidoc.element.derby.Controller.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Controller.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>removeListener (type, listener)](#apidoc.element.derby.Controller.prototype.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
...
  useCapture = listener;
  listener = target;
  target = document;
}
this.addListener(type, target, wrappedListener, useCapture);
var dom = this;
function wrappedListener() {
  dom.removeListener(type, target, wrappedListener, useCapture);
  return listener.apply(this, arguments);
}
};

Dom.prototype.removeListener = function(type, target, listener, useCapture) {
if (typeof target === 'function') {
  useCapture = listener;
...
```

#### <a name="apidoc.element.derby.Controller.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">derby.Controller.prototype.</span>setMaxListeners (n)](#apidoc.element.derby.Controller.prototype.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.Derby"></a>[module derby.Derby](#apidoc.module.derby.Derby)

#### <a name="apidoc.element.derby.Derby.Derby"></a>[function <span class="apidocSignatureSpan">derby.</span>Derby ()](#apidoc.element.derby.Derby.Derby)
- description and source-code
```javascript
function Derby() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.Derby.prototype"></a>[module derby.Derby.prototype](#apidoc.module.derby.Derby.prototype)

#### <a name="apidoc.element.derby.Derby.prototype.App"></a>[function <span class="apidocSignatureSpan">derby.Derby.prototype.</span>App (derby, name, filename, options)](#apidoc.element.derby.Derby.prototype.App)
- description and source-code
```javascript
function App(derby, name, filename, options) {
  EventEmitter.call(this);
  this.derby = derby;
  this.name = name;
  this.filename = filename;
  this.scriptHash = '{{DERBY_SCRIPT_HASH}}';
  this.bundledAt = '{{DERBY_BUNDLED_AT}}';
  this.Page = createAppPage();
  this.proto = this.Page.prototype;
  this.views = new derbyTemplates.templates.Views();
  this.tracksRoutes = tracks.setup(this);
  this.model = null;
  this.page = null;
  this._init(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Derby.prototype.Component"></a>[function <span class="apidocSignatureSpan">derby.Derby.prototype.</span>Component (parent, context, id, scope)](#apidoc.element.derby.Derby.prototype.Component)
- description and source-code
```javascript
function Component(parent, context, id, scope) {
  this.parent = parent;
  this.context = context;
  this.id = id;
  this._scope = scope;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Derby.prototype.Page"></a>[function <span class="apidocSignatureSpan">derby.Derby.prototype.</span>Page (app, model, req, res)](#apidoc.element.derby.Derby.prototype.Page)
- description and source-code
```javascript
function Page(app, model, req, res) {
  Controller.call(this, app, this, model);
  this.req = req;
  this.res = res;
  this.params = null;
  if (this.init) this.init(model);
  this.context = this._createContext();
  this._eventModel = null;
  this._removeModelListeners = null;
  this._components = {};
  this._addListeners();
}
```
- example usage
```shell
...
App.prototype.loadStyles = function() {};

App.prototype.createPage = function() {
if (this.page) {
  this.emit('destroyPage', this.page);
  this.page.destroy();
}
var page = new this.Page(this, this.model);
this.page = page;
return page;
};

App.prototype.onRoute = function(callback, page, next, done) {
if (this._waitForAttach) {
  // Cancel any routing before the initial page attachment. Instead, do a
...
```

#### <a name="apidoc.element.derby.Derby.prototype.createApp"></a>[function <span class="apidocSignatureSpan">derby.Derby.prototype.</span>createApp (name, filename, options)](#apidoc.element.derby.Derby.prototype.createApp)
- description and source-code
```javascript
createApp = function (name, filename, options) {
  return new App(this, name, filename, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Derby.prototype.run"></a>[function <span class="apidocSignatureSpan">derby.Derby.prototype.</span>run (createServer)](#apidoc.element.derby.Derby.prototype.run)
- description and source-code
```javascript
run = function (createServer) {
  // In production
  if (this.util.isProduction) return createServer();
  if (cluster.isMaster) {
    console.log('Master pid ', process.pid);
    startWorker();
  } else {
    createServer();
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.Dom"></a>[module derby.Dom](#apidoc.module.derby.Dom)

#### <a name="apidoc.element.derby.Dom.Dom"></a>[function <span class="apidocSignatureSpan">derby.</span>Dom (controller)](#apidoc.element.derby.Dom.Dom)
- description and source-code
```javascript
function Dom(controller) {
  this.controller = controller;
  this._listeners = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.Dom.prototype"></a>[module derby.Dom.prototype](#apidoc.module.derby.Dom.prototype)

#### <a name="apidoc.element.derby.Dom.prototype._initListeners"></a>[function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>_initListeners ()](#apidoc.element.derby.Dom.prototype._initListeners)
- description and source-code
```javascript
_initListeners = function () {
  var dom = this;
  this.controller.on('destroy', function domOnDestroy() {
    var listeners = dom._listeners;
    if (!listeners) return;
    for (var i = listeners.length; i--;) {
      listeners[i].remove();
    }
    dom._listeners = null;
  });
  return this._listeners = [];
}
```
- example usage
```shell
...
    listener = target;
    target = document;
  }
  var domListener =
    (type === 'destroy') ? new DestroyListener(target, listener) :
    new DomListener(type, target, listener, useCapture);
  if (-1 === this._listenerIndex(domListener)) {
    var listeners = this._listeners || this._initListeners();
    listeners.push(domListener);
  }
  domListener.add();
};
Dom.prototype.on = Dom.prototype.addListener;

Dom.prototype.once = function(type, target, listener, useCapture) {
...
```

#### <a name="apidoc.element.derby.Dom.prototype._listenerIndex"></a>[function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>_listenerIndex (domListener)](#apidoc.element.derby.Dom.prototype._listenerIndex)
- description and source-code
```javascript
_listenerIndex = function (domListener) {
  var listeners = this._listeners;
  if (!listeners) return -1;
  for (var i = listeners.length; i--;) {
    if (listeners[i].equals(domListener)) return i;
  }
  return -1;
}
```
- example usage
```shell
...
    useCapture = listener;
    listener = target;
    target = document;
  }
  var domListener =
    (type === 'destroy') ? new DestroyListener(target, listener) :
    new DomListener(type, target, listener, useCapture);
  if (-1 === this._listenerIndex(domListener)) {
    var listeners = this._listeners || this._initListeners();
    listeners.push(domListener);
  }
  domListener.add();
};
Dom.prototype.on = Dom.prototype.addListener;
...
```

#### <a name="apidoc.element.derby.Dom.prototype.addListener"></a>[function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>addListener (type, target, listener, useCapture)](#apidoc.element.derby.Dom.prototype.addListener)
- description and source-code
```javascript
addListener = function (type, target, listener, useCapture) {
  if (typeof target === 'function') {
    useCapture = listener;
    listener = target;
    target = document;
  }
  var domListener =
    (type === 'destroy') ? new DestroyListener(target, listener) :
    new DomListener(type, target, listener, useCapture);
  if (-1 === this._listenerIndex(domListener)) {
    var listeners = this._listeners || this._initListeners();
    listeners.push(domListener);
  }
  domListener.add();
}
```
- example usage
```shell
...

Dom.prototype.once = function(type, target, listener, useCapture) {
  if (typeof target === 'function') {
    useCapture = listener;
    listener = target;
    target = document;
  }
  this.addListener(type, target, wrappedListener, useCapture);
  var dom = this;
  function wrappedListener() {
    dom.removeListener(type, target, wrappedListener, useCapture);
    return listener.apply(this, arguments);
  }
};
...
```

#### <a name="apidoc.element.derby.Dom.prototype.on"></a>[function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>on (type, target, listener, useCapture)](#apidoc.element.derby.Dom.prototype.on)
- description and source-code
```javascript
on = function (type, target, listener, useCapture) {
  if (typeof target === 'function') {
    useCapture = listener;
    listener = target;
    target = document;
  }
  var domListener =
    (type === 'destroy') ? new DestroyListener(target, listener) :
    new DomListener(type, target, listener, useCapture);
  if (-1 === this._listenerIndex(domListener)) {
    var listeners = this._listeners || this._initListeners();
    listeners.push(domListener);
  }
  domListener.add();
}
```
- example usage
```shell
...

// Overriden on server
App.prototype._init = function() {
this._waitForAttach = true;
this._cancelAttach = false;
this.model = new this.derby.Model();
serializedViews(derbyTemplates, this.views);
// Must init async so that app.on('model') listeners can be added.
// Must also wait for content ready so that bundle is fully downloaded.
this._contentReady();
};
App.prototype._finishInit = function() {
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
...
```

#### <a name="apidoc.element.derby.Dom.prototype.once"></a>[function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>once (type, target, listener, useCapture)](#apidoc.element.derby.Dom.prototype.once)
- description and source-code
```javascript
once = function (type, target, listener, useCapture) {
  if (typeof target === 'function') {
    useCapture = listener;
    listener = target;
    target = document;
  }
  this.addListener(type, target, wrappedListener, useCapture);
  var dom = this;
  function wrappedListener() {
    dom.removeListener(type, target, wrappedListener, useCapture);
    return listener.apply(this, arguments);
  }
}
```
- example usage
```shell
...
}
options || (options = {});
if (options.minify == null) options.minify = util.isProduction;
// Turn all of the app's currently registered views into a javascript
// function that can recreate them in the client
var viewsSource = this._viewsSource(options);
var bundleFiles = [];
backend.once('bundle', function(bundle) {
  bundle.require(path.dirname(__dirname), {expose: 'derby'});
  // Hack to inject the views script into the Browserify bundle by replacing
  // the empty _views.js file with the generated source
  var viewsFilename = require.resolve('./_views');
  bundle.transform(function(filename) {
    if (filename !== viewsFilename) return through();
    return through(
...
```

#### <a name="apidoc.element.derby.Dom.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">derby.Dom.prototype.</span>removeListener (type, target, listener, useCapture)](#apidoc.element.derby.Dom.prototype.removeListener)
- description and source-code
```javascript
removeListener = function (type, target, listener, useCapture) {
  if (typeof target === 'function') {
    useCapture = listener;
    listener = target;
    target = document;
  }
  var domListener = new DomListener(type, target, listener, useCapture);
  domListener.remove();
  var i = this._listenerIndex(domListener);
  if (i > -1) this._listeners.splice(i, 1);
}
```
- example usage
```shell
...
  useCapture = listener;
  listener = target;
  target = document;
}
this.addListener(type, target, wrappedListener, useCapture);
var dom = this;
function wrappedListener() {
  dom.removeListener(type, target, wrappedListener, useCapture);
  return listener.apply(this, arguments);
}
};

Dom.prototype.removeListener = function(type, target, listener, useCapture) {
if (typeof target === 'function') {
  useCapture = listener;
...
```



# <a name="apidoc.module.derby.Page"></a>[module derby.Page](#apidoc.module.derby.Page)

#### <a name="apidoc.element.derby.Page.Page"></a>[function <span class="apidocSignatureSpan">derby.</span>Page (app, model, req, res)](#apidoc.element.derby.Page.Page)
- description and source-code
```javascript
function Page(app, model, req, res) {
  Controller.call(this, app, this, model);
  this.req = req;
  this.res = res;
  this.params = null;
  if (this.init) this.init(model);
  this.context = this._createContext();
  this._eventModel = null;
  this._removeModelListeners = null;
  this._components = {};
  this._addListeners();
}
```
- example usage
```shell
...
App.prototype.loadStyles = function() {};

App.prototype.createPage = function() {
if (this.page) {
  this.emit('destroyPage', this.page);
  this.page.destroy();
}
var page = new this.Page(this, this.model);
this.page = page;
return page;
};

App.prototype.onRoute = function(callback, page, next, done) {
if (this._waitForAttach) {
  // Cancel any routing before the initial page attachment. Instead, do a
...
```



# <a name="apidoc.module.derby.Page.prototype"></a>[module derby.Page.prototype](#apidoc.module.derby.Page.prototype)

#### <a name="apidoc.element.derby.Page.prototype._addContextListeners"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_addContextListeners (eventModel)](#apidoc.element.derby.Page.prototype._addContextListeners)
- description and source-code
```javascript
_addContextListeners = function (eventModel) {
  this.context.meta.addBinding = addBinding;
  this.context.meta.removeBinding = removeBinding;
  this.context.meta.removeNode = removeNode;
  this.context.meta.addItemContext = addItemContext;
  this.context.meta.removeItemContext = removeItemContext;

  function addItemContext(context) {
    var segments = context.expression.resolve(context);
    eventModel.addItemContext(segments, context);
  }
  function removeItemContext(context) {
    // TODO
  }
  function addBinding(binding) {
    patchTextBinding(binding);
    var expressions = binding.template.expressions;
    if (expressions) {
      for (var i = 0, len = expressions.length; i < len; i++) {
        addDependencies(eventModel, expressions[i], binding);
      }
    } else {
      var expression = binding.template.expression;
      addDependencies(eventModel, expression, binding);
    }
  }
  function removeBinding(binding) {
    var bindingWrappers = binding.meta;
    if (!bindingWrappers) return;
    for (var i = bindingWrappers.length; i--;) {
      eventModel.removeBinding(bindingWrappers[i]);
    }
  }
  function removeNode(node) {
    var component = node.$component;
    if (component && !component.singleton) {
      component.destroy();
    }
    var destroyListeners = node.$destroyListeners;
    if (destroyListeners) {
      for (var i = 0; i < destroyListeners.length; i++) {
        destroyListeners[i]();
      }
    }
  }
}
```
- example usage
```shell
...
context.alias = '#root';
return context;
};

Page.prototype._addListeners = function() {
var eventModel = this._eventModel = new EventModel();
this._addModelListeners(eventModel);
this._addContextListeners(eventModel);
};

Page.prototype.destroy = function() {
this.emit('destroy');
this._removeModelListeners();
for (var id in this._components) {
  var component = this._components[id];
...
```

#### <a name="apidoc.element.derby.Page.prototype._addListeners"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_addListeners ()](#apidoc.element.derby.Page.prototype._addListeners)
- description and source-code
```javascript
_addListeners = function () {}
```
- example usage
```shell
...
this.res = res;
this.params = null;
if (this.init) this.init(model);
this.context = this._createContext();
this._eventModel = null;
this._removeModelListeners = null;
this._components = {};
this._addListeners();
}

util.mergeInto(Page.prototype, Controller.prototype);

Page.prototype.$bodyClass = function(ns) {
if (!ns) return;
var classNames = [];
...
```

#### <a name="apidoc.element.derby.Page.prototype._addModelListeners"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_addModelListeners (eventModel)](#apidoc.element.derby.Page.prototype._addModelListeners)
- description and source-code
```javascript
_addModelListeners = function (eventModel) {
  var model = this.model;
  if (!model) return;

  var context = this.context;
  var changeListener = model.on('change', '**', function onChange(path, value, previous, pass) {
    var segments = util.castSegments(path.split('.'));
    // The pass parameter is passed in for special handling of updates
    // resulting from stringInsert or stringRemove
    eventModel.set(segments, previous, pass);
  });
  var loadListener = model.on('load', '**', function onLoad(path) {
    var segments = util.castSegments(path.split('.'));
    eventModel.set(segments);
  });
  var unloadListener = model.on('unload', '**', function onUnload(path) {
    var segments = util.castSegments(path.split('.'));
    eventModel.set(segments);
  });
  var insertListener = model.on('insert', '**', function onInsert(path, index, values) {
    var segments = util.castSegments(path.split('.'));
    eventModel.insert(segments, index, values.length);
  });
  var removeListener = model.on('remove', '**', function onRemove(path, index, values) {
    var segments = util.castSegments(path.split('.'));
    eventModel.remove(segments, index, values.length);
  });
  var moveListener = model.on('move', '**', function onMove(path, from, to, howMany) {
    var segments = util.castSegments(path.split('.'));
    eventModel.move(segments, from, to, howMany);
  });

  this._removeModelListeners = function() {
    model.removeListener('change', changeListener);
    model.removeListener('load', loadListener);
    model.removeListener('unload', unloadListener);
    model.removeListener('insert', insertListener);
    model.removeListener('remove', removeListener);
    model.removeListener('move', moveListener);
  };
}
```
- example usage
```shell
...
context.expression = new expressions.PathExpression([]);
context.alias = '#root';
return context;
};

Page.prototype._addListeners = function() {
var eventModel = this._eventModel = new EventModel();
this._addModelListeners(eventModel);
this._addContextListeners(eventModel);
};

Page.prototype.destroy = function() {
this.emit('destroy');
this._removeModelListeners();
for (var id in this._components) {
...
```

#### <a name="apidoc.element.derby.Page.prototype._createContext"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_createContext ()](#apidoc.element.derby.Page.prototype._createContext)
- description and source-code
```javascript
_createContext = function () {
  var contextMeta = new contexts.ContextMeta();
  contextMeta.views = this.app && this.app.views;
  var context = new contexts.Context(contextMeta, this);
  context.expression = new expressions.PathExpression([]);
  context.alias = '#root';
  return context;
}
```
- example usage
```shell
...

function Page(app, model, req, res) {
  Controller.call(this, app, this, model);
  this.req = req;
  this.res = res;
  this.params = null;
  if (this.init) this.init(model);
  this.context = this._createContext();
  this._eventModel = null;
  this._removeModelListeners = null;
  this._components = {};
  this._addListeners();
}

util.mergeInto(Page.prototype, Controller.prototype);
...
```

#### <a name="apidoc.element.derby.Page.prototype._setRenderParams"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_setRenderParams (ns)](#apidoc.element.derby.Page.prototype._setRenderParams)
- description and source-code
```javascript
_setRenderParams = function (ns) {
  this.model.set('$render.ns', ns);
  this.model.set('$render.params', this.params);
  this.model.set('$render.url', this.params && this.params.url);
  this.model.set('$render.query', this.params && this.params.query);
}
```
- example usage
```shell
...
Page.prototype.getView = function(viewName, ns) {
return this.app.views.find(viewName, ns);
};

Page.prototype.render = function(ns) {
this.app.emit('render', this);
this.context.pause();
this._setRenderParams(ns);
var titleFragment = this.getFragment('TitleElement', ns);
var bodyFragment = this.getFragment('BodyElement', ns);
var titleElement = document.getElementsByTagName('title')[0];
titleElement.parentNode.replaceChild(titleFragment, titleElement);
document.body.parentNode.replaceChild(bodyFragment, document.body);
this.context.unpause();
if (this.create) this.create(this.model, this.dom);
...
```

#### <a name="apidoc.element.derby.Page.prototype._setRenderPrefix"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>_setRenderPrefix (ns)](#apidoc.element.derby.Page.prototype._setRenderPrefix)
- description and source-code
```javascript
_setRenderPrefix = function (ns) {
  var prefix = (ns) ? ns + ':' : '';
  this.model.set('$render.prefix', prefix);
}
```
- example usage
```shell
...

Page.prototype._setRenderPrefix = function(ns) {
var prefix = (ns) ? ns + ':' : '';
this.model.set('$render.prefix', prefix);
};

Page.prototype.get = function(viewName, ns, unescaped) {
this._setRenderPrefix(ns);
var view = this.getView(viewName, ns);
return view.get(this.context, unescaped);
};

Page.prototype.getFragment = function(viewName, ns) {
this._setRenderPrefix(ns);
var view = this.getView(viewName, ns);
...
```

#### <a name="apidoc.element.derby.Page.prototype.addListener"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>addListener (type, listener)](#apidoc.element.derby.Page.prototype.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...

Dom.prototype.once = function(type, target, listener, useCapture) {
  if (typeof target === 'function') {
    useCapture = listener;
    listener = target;
    target = document;
  }
  this.addListener(type, target, wrappedListener, useCapture);
  var dom = this;
  function wrappedListener() {
    dom.removeListener(type, target, wrappedListener, useCapture);
    return listener.apply(this, arguments);
  }
};
...
```

#### <a name="apidoc.element.derby.Page.prototype.attach"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>attach ()](#apidoc.element.derby.Page.prototype.attach)
- description and source-code
```javascript
attach = function () {
  this.context.pause();
  var ns = this.model.get('$render.ns');
  var titleView = this.getView('TitleElement', ns);
  var bodyView = this.getView('BodyElement', ns);
  var titleElement = document.getElementsByTagName('title')[0];
  titleView.attachTo(titleElement.parentNode, titleElement, this.context);
  bodyView.attachTo(document.body.parentNode, document.body, this.context);
  this.context.unpause();
  if (this.create) this.create(this.model, this.dom);
}
```
- example usage
```shell
...
  return;
}
// Since an attachment failure is *fatal* and could happen as a result of a
// browser extension like AdBlock, an invalid template, or a small bug in
// Derby or Saddle, re-render from scratch on production failures
if (util.isProduction) {
  try {
    page.attach();
  } catch (err) {
    this.history.refresh();
    console.warn('attachment error', err.stack);
  }
} else {
  page.attach();
}
...
```

#### <a name="apidoc.element.derby.Page.prototype.destroy"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>destroy ()](#apidoc.element.derby.Page.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  this.emit('destroy');
  this._removeModelListeners();
  for (var id in this._components) {
    var component = this._components[id];
    component.destroy();
  }
  // Remove all data, refs, listeners, and reactive functions
  // for the previous page
  var silentModel = this.model.silent();
  silentModel.destroy('_page');
  silentModel.destroy('$components');
  // Unfetch and unsubscribe from all queries and documents
  silentModel.unloadAll && silentModel.unloadAll();
}
```
- example usage
```shell
...
App.prototype.loadViews = function() {};

App.prototype.loadStyles = function() {};

App.prototype.createPage = function() {
  if (this.page) {
    this.emit('destroyPage', this.page);
    this.page.destroy();
  }
  var page = new this.Page(this, this.model);
  this.page = page;
  return page;
};

App.prototype.onRoute = function(callback, page, next, done) {
...
```

#### <a name="apidoc.element.derby.Page.prototype.emit"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>emit (type)](#apidoc.element.derby.Page.prototype.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
...
// Must also wait for content ready so that bundle is fully downloaded.
this._contentReady();
};
App.prototype._finishInit = function() {
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
this.emit('model', this.model);
util.isProduction = data.nodeEnv === 'production';
if (!util.isProduction) this._autoRefresh();
this.model.unbundle(data);
var page = this.createPage();
page.params = this.model.get('$render.params');
this.emit('ready', page);
this._waitForAttach = false;
...
```

#### <a name="apidoc.element.derby.Page.prototype.emitCancellable"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>emitCancellable ()](#apidoc.element.derby.Page.prototype.emitCancellable)
- description and source-code
```javascript
emitCancellable = function () {
  var cancelled = false;
  function cancel() {
    cancelled = true;
  }

  var args = Array.prototype.slice.call(arguments);
  args.push(cancel);
  this.emit.apply(this, args);

  return cancelled;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page.prototype.emitDelayable"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>emitDelayable ()](#apidoc.element.derby.Page.prototype.emitDelayable)
- description and source-code
```javascript
emitDelayable = function () {
  var args = Array.prototype.slice.call(arguments);
  var callback = args.pop();

  var delayed = false;
  function delay() {
    delayed = true;
    return callback;
  }

  args.push(delay);
  this.emit.apply(this, args);
  if (!delayed) callback();

  return delayed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page.prototype.eventNames"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>eventNames ()](#apidoc.element.derby.Page.prototype.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page.prototype.get"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>get (viewName, ns, unescaped)](#apidoc.element.derby.Page.prototype.get)
- description and source-code
```javascript
get = function (viewName, ns, unescaped) {
  this._setRenderPrefix(ns);
  var view = this.getView(viewName, ns);
  return view.get(this.context, unescaped);
}
```
- example usage
```shell
...
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
this.emit('model', this.model);
util.isProduction = data.nodeEnv === 'production';
if (!util.isProduction) this._autoRefresh();
this.model.unbundle(data);
var page = this.createPage();
page.params = this.model.get('$render.params');
this.emit('ready', page);
this._waitForAttach = false;
// Instead of attaching, do a route and render if a link was clicked before
// the page finished attaching
if (this._cancelAttach) {
  this.history.refresh();
  return;
...
```

#### <a name="apidoc.element.derby.Page.prototype.getFragment"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>getFragment (viewName, ns)](#apidoc.element.derby.Page.prototype.getFragment)
- description and source-code
```javascript
getFragment = function (viewName, ns) {
  this._setRenderPrefix(ns);
  var view = this.getView(viewName, ns);
  return view.getFragment(this.context);
}
```
- example usage
```shell
...
  var view = this.getView(viewName, ns);
  return view.get(this.context, unescaped);
};

Page.prototype.getFragment = function(viewName, ns) {
  this._setRenderPrefix(ns);
  var view = this.getView(viewName, ns);
  return view.getFragment(this.context);
};

Page.prototype.getView = function(viewName, ns) {
  return this.app.views.find(viewName, ns);
};

Page.prototype.render = function(ns) {
...
```

#### <a name="apidoc.element.derby.Page.prototype.getMaxListeners"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>getMaxListeners ()](#apidoc.element.derby.Page.prototype.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page.prototype.getView"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>getView (viewName, ns)](#apidoc.element.derby.Page.prototype.getView)
- description and source-code
```javascript
getView = function (viewName, ns) {
  return this.app.views.find(viewName, ns);
}
```
- example usage
```shell
...
Page.prototype._setRenderPrefix = function(ns) {
var prefix = (ns) ? ns + ':' : '';
this.model.set('$render.prefix', prefix);
};

Page.prototype.get = function(viewName, ns, unescaped) {
this._setRenderPrefix(ns);
var view = this.getView(viewName, ns);
return view.get(this.context, unescaped);
};

Page.prototype.getFragment = function(viewName, ns) {
this._setRenderPrefix(ns);
var view = this.getView(viewName, ns);
return view.getFragment(this.context);
...
```

#### <a name="apidoc.element.derby.Page.prototype.listenerCount"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>listenerCount (type)](#apidoc.element.derby.Page.prototype.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page.prototype.listeners"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>listeners (type)](#apidoc.element.derby.Page.prototype.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page.prototype.on"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>on (type, listener)](#apidoc.element.derby.Page.prototype.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...

// Overriden on server
App.prototype._init = function() {
this._waitForAttach = true;
this._cancelAttach = false;
this.model = new this.derby.Model();
serializedViews(derbyTemplates, this.views);
// Must init async so that app.on('model') listeners can be added.
// Must also wait for content ready so that bundle is fully downloaded.
this._contentReady();
};
App.prototype._finishInit = function() {
var script = this._getScript();
var data = JSON.parse(script.nextSibling.innerHTML);
this.model.createConnection(data);
...
```

#### <a name="apidoc.element.derby.Page.prototype.once"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>once (type, listener)](#apidoc.element.derby.Page.prototype.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
...
}
options || (options = {});
if (options.minify == null) options.minify = util.isProduction;
// Turn all of the app's currently registered views into a javascript
// function that can recreate them in the client
var viewsSource = this._viewsSource(options);
var bundleFiles = [];
backend.once('bundle', function(bundle) {
  bundle.require(path.dirname(__dirname), {expose: 'derby'});
  // Hack to inject the views script into the Browserify bundle by replacing
  // the empty _views.js file with the generated source
  var viewsFilename = require.resolve('./_views');
  bundle.transform(function(filename) {
    if (filename !== viewsFilename) return through();
    return through(
...
```

#### <a name="apidoc.element.derby.Page.prototype.prependListener"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>prependListener (type, listener)](#apidoc.element.derby.Page.prototype.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page.prototype.prependOnceListener"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.derby.Page.prototype.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>removeAllListeners (type)](#apidoc.element.derby.Page.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>removeListener (type, listener)](#apidoc.element.derby.Page.prototype.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
...
  useCapture = listener;
  listener = target;
  target = document;
}
this.addListener(type, target, wrappedListener, useCapture);
var dom = this;
function wrappedListener() {
  dom.removeListener(type, target, wrappedListener, useCapture);
  return listener.apply(this, arguments);
}
};

Dom.prototype.removeListener = function(type, target, listener, useCapture) {
if (typeof target === 'function') {
  useCapture = listener;
...
```

#### <a name="apidoc.element.derby.Page.prototype.render"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>render (status, ns)](#apidoc.element.derby.Page.prototype.render)
- description and source-code
```javascript
render = function (status, ns) {
  if (typeof status !== 'number') {
    ns = status;
    status = null;
  }
  this.app.emit('render', this);

  if (status) this.res.statusCode = status;
  // Prevent the browser from storing the HTML response in its back cache, since
  // that will cause it to render with the data from the initial load first
  this.res.setHeader('Cache-Control', 'no-store');
  // Set HTML utf-8 content type unless already set
  if (!this.res.getHeader('Content-Type')) {
    this.res.setHeader('Content-Type', 'text/html; charset=utf-8');
  }

  this._setRenderParams(ns);
  var pageHtml = this.get('Page', ns);
  this.res.write(pageHtml);

  var bundleScriptTag = '<script async data-derby-app src="' + this.app.scriptUrl + '"';
  if (this.app.scriptCrossOrigin) {
    // Scripts loaded from a different origin (such as a CDN) won't report
    // much information to the host page's window.onerror. Adding the
    // "crossorigin" attribute to the script tag allows reporting of detailed
    // error info to the host page.
    // HOWEVER - if the "crossorigin" attribute is present for a script tag
    // with a cross-origin "src", then the script's HTTP response MUST have
    // an appropriate "Access-Control-Allow-Origin" header set. Otherwise,
    // the browser will refuse to load the script.
    bundleScriptTag += ' crossorigin';
  }
  bundleScriptTag += '></script>';
  this.res.write(bundleScriptTag);

  this.res.write('<script type="application/json">');
  var tailHtml = this.get('Tail', ns);

  this.model.destroy('$components');

  var page = this;
  this.model.bundle(function(err, bundle) {
    if (page.model.hasErrored) return;
    if (err) return page.emit('error', err);
    var json = stringifyBundle(bundle);
    page.res.write(json);
    page.res.end('</script>' + tailHtml);
    page.app.emit('routeDone', page, 'render');
  });
}
```
- example usage
```shell
...
};

App.prototype._handleMessage = function(action, message) {
if (action === 'refreshViews') {
  var fn = new Function('return ' + message.views)(); // jshint ignore:line
  fn(derbyTemplates, this.views);
  var ns = this.model.get('$render.ns');
  this.page.render(ns);

} else if (action === 'refreshStyles') {
  var styleElement = document.querySelector('style[data-filename="' +
    message.filename + '"]');
  if (styleElement) styleElement.innerHTML = message.css;

} else if (action === 'reload') {
...
```

#### <a name="apidoc.element.derby.Page.prototype.renderStatic"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>renderStatic (status, ns)](#apidoc.element.derby.Page.prototype.renderStatic)
- description and source-code
```javascript
renderStatic = function (status, ns) {
  if (typeof status !== 'number') {
    ns = status;
    status = null;
  }
  this.app.emit('renderStatic', this);

  if (status) this.res.statusCode = status;
  this.params = pageParams(this.req);
  this._setRenderParams(ns);
  var pageHtml = this.get('Page', ns);
  var tailHtml = this.get('Tail', ns);
  this.res.send(pageHtml + tailHtml);
  this.app.emit('routeDone', this, 'renderStatic');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.Page.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">derby.Page.prototype.</span>setMaxListeners (n)](#apidoc.element.derby.Page.prototype.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.components"></a>[module derby.components](#apidoc.module.derby.components)

#### <a name="apidoc.element.derby.components.Component"></a>[function <span class="apidocSignatureSpan">derby.components.</span>Component (parent, context, id, scope)](#apidoc.element.derby.components.Component)
- description and source-code
```javascript
function Component(parent, context, id, scope) {
  this.parent = parent;
  this.context = context;
  this.id = id;
  this._scope = scope;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.components.ComponentFactory"></a>[function <span class="apidocSignatureSpan">derby.components.</span>ComponentFactory (constructor)](#apidoc.element.derby.components.ComponentFactory)
- description and source-code
```javascript
function ComponentFactory(constructor) {
  this.constructor = constructor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.components.SingletonComponentFactory"></a>[function <span class="apidocSignatureSpan">derby.components.</span>SingletonComponentFactory (constructor)](#apidoc.element.derby.components.SingletonComponentFactory)
- description and source-code
```javascript
function SingletonComponentFactory(constructor) {
  this.constructor = constructor;
  this.component = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.components.createFactory"></a>[function <span class="apidocSignatureSpan">derby.components.</span>createFactory (constructor)](#apidoc.element.derby.components.createFactory)
- description and source-code
```javascript
function createFactory(constructor) {
  return (constructor.prototype.singleton) ?
    new SingletonComponentFactory(constructor) :
    new ComponentFactory(constructor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.documentListeners"></a>[module derby.documentListeners](#apidoc.module.derby.documentListeners)

#### <a name="apidoc.element.derby.documentListeners.add"></a>[function <span class="apidocSignatureSpan">derby.documentListeners.</span>add (doc)](#apidoc.element.derby.documentListeners.add)
- description and source-code
```javascript
function addDocumentListeners(doc) {
  doc.addEventListener('input', documentInput, true);
  doc.addEventListener('change', documentChange, true);

  // Listen to more events for versions of IE with buggy input event implementations
  if (parseFloat(window.navigator.appVersion.split('MSIE ')[1]) <= 9) {
    // We're listening on selectionchange because there's no other event emitted when
    // the user clicks 'delete' from a context menu when right clicking on selected text.
    // So although this event fires overly aggressively, it's the only real way
    // to ensure that we can detect all changes to the input value in IE <= 9
    doc.addEventListener('selectionchange', function(e){
      if (document.activeElement) {
        documentInput({target: document.activeElement}); // selectionchange evts don't have the e.target we need
      }
    }, true);
  }

  // For some reason valueAsNumber returns NaN for number inputs in IE
  // until a new IE version that handles this is released, parse input.value as a fallback
  var input = document.createElement('input');
  input.type = 'number';
  input.value = '7';
  if (input.valueAsNumber !== input.valueAsNumber) {
    var oldInputValue = inputValue;
    inputValue = function(input) {
      if (input.type === 'number') {
        return inputIsNumberValue(input) ? parseFloat(input.value) : input.value;
      } else {
        return oldInputValue.apply(this, arguments);
      }
    };
  }
}
```
- example usage
```shell
...
Derby.prototype.Component = components.Component;

Derby.prototype.createApp = function(name, filename, options) {
  return new App(this, name, filename, options);
};

if (!racer.util.isServer) {
  require('./documentListeners').add(document);
}

racer.util.serverRequire(module, './Derby.server');
...
```

#### <a name="apidoc.element.derby.documentListeners.inputSupportsSelection"></a>[function <span class="apidocSignatureSpan">derby.documentListeners.</span>inputSupportsSelection (input)](#apidoc.element.derby.documentListeners.inputSupportsSelection)
- description and source-code
```javascript
function inputSupportsSelection(input) {
  var type = input.type;
  return (
    type === 'text' ||
    type === 'textarea' ||
    type === 'search' ||
    type === 'url' ||
    type === 'tel' ||
    type === 'password'
  );
}
```
- example usage
```shell
...
}

function patchTextBinding(binding) {
  if (
    binding instanceof templates.AttributeBinding &&
    binding.name === 'value' &&
    (binding.element.tagName === 'INPUT' || binding.element.tagName === 'TEXTAREA') &&
    documentListeners.inputSupportsSelection(binding.element) &&
    binding.template.expression.resolve(binding.context)
  ) {
    binding.update = textInputUpdate;
  }
}

function textInputUpdate(previous, pass) {
...
```



# <a name="apidoc.module.derby.eventmodel"></a>[module derby.eventmodel](#apidoc.module.derby.eventmodel)

#### <a name="apidoc.element.derby.eventmodel.eventmodel"></a>[function <span class="apidocSignatureSpan">derby.</span>eventmodel ()](#apidoc.element.derby.eventmodel.eventmodel)
- description and source-code
```javascript
function EventModel() {
  this.id = nextId++;

  // Most of these won't ever be filled in, so I'm just leaving them null.
  //
  // These contain our EventModel children.
  this.object = null;
  this.array = null;

  // This contains any EventModel children which have floating references.
  this.arrayByReference = null;

  // If the data stored here is ever used to lookup other values, this is an
  // object mapping remote child ID -> ref.
  //
  // Eg given x[y], y.refOut[x.id] = <Binding>
  this.refOut = null;

  // This is a map from ref id -> event model for events bound to this
  // EventModel but via a ref. We could just merge them into the main tree, but
  // this way they're easy to move.
  //
  // Eg, given x[y] (y=1), x.1.refChildren[ref id] is an EventModel.
  this.refChildren = null;

  this.bindings = null;

  // Item contexts are contexts which need their item number changed as this
  // EventModel object moves around its surrounding list.
  this.itemContexts = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.derby.eventmodel.prototype"></a>[module derby.eventmodel.prototype](#apidoc.module.derby.eventmodel.prototype)

#### <a name="apidoc.element.derby.eventmodel.prototype._addBinding"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_addBinding (binding)](#apidoc.element.derby.eventmodel.prototype._addBinding)
- description and source-code
```javascript
_addBinding = function (binding) {
  var bindings = this.bindings || (this.bindings = new BindingsMap());
  binding.eventModels || (binding.eventModels = new EventModelsMap());
  bindings[binding.id] = binding;
  binding.eventModels[this.id] = this;
}
```
- example usage
```shell
...
  bindings[binding.id] = binding;
  binding.eventModels[this.id] = this;
};

// This is the main hook to add bindings to the event model tree. It should
// only be called on the root EventModel object.
EventModel.prototype.addBinding = function(segments, binding) {
  this.at(segments)._addBinding(binding);
};

// This is used for objects (contexts in derby's case) that have a .item
// property which refers to an array index.
EventModel.prototype.addItemContext = function(segments, context) {
  this.at(segments)._addItemContext(context);
};
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype._addItemContext"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_addItemContext (context)](#apidoc.element.derby.eventmodel.prototype._addItemContext)
- description and source-code
```javascript
_addItemContext = function (context) {
  if (!context._id) context._id = nextId++;
  if (!this.itemContexts) this.itemContexts = new ItemContextsMap();
  this.itemContexts[context._id] = context;
}
```
- example usage
```shell
...
EventModel.prototype.addBinding = function(segments, binding) {
this.at(segments)._addBinding(binding);
};

// This is used for objects (contexts in derby's case) that have a .item
// property which refers to an array index.
EventModel.prototype.addItemContext = function(segments, context) {
this.at(segments)._addItemContext(context);
};

EventModel.prototype.removeBinding = function(binding) {
if (!binding.eventModels) return;
for (var id in binding.eventModels) {
  var eventModel = binding.eventModels[id];
  if (eventModel.bindings) delete eventModel.bindings[binding.id];
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype._each"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_each (segments, pos, fn)](#apidoc.element.derby.eventmodel.prototype._each)
- description and source-code
```javascript
_each = function (segments, pos, fn) {
  // Our refChildren are effectively merged into this object.
  if (this.refChildren) {
    for (var id in this.refChildren) {
      var refChild = this.refChildren[id];
      if (refChild) refChild._each(segments, pos, fn);
    }
  }

  if (segments.length === pos) {
    fn(this);
    return;
  }

  var segment = segments[pos];
  var child;
  if (typeof segment === 'string') {
    // Object. Just recurse into our objects set. Its possible to rewrite this
    // function to simply loop in the case of object lookups, but I don't think
    // it'll buy us much.
    child = this.object && this.object[segment];
    if (child) child._each(segments, pos + 1, fn);

  } else {
    // Number. Recurse both into the fixed list and the reference list.
    child = this.array && this.array[segment];
    if (child) child._each(segments, pos + 1, fn);

    child = this.arrayByReference && this.arrayByReference[segment];
    if (child) child._each(segments, pos + 1, fn);
  }
}
```
- example usage
```shell
...
};

EventModel.prototype._each = function(segments, pos, fn) {
// Our refChildren are effectively merged into this object.
if (this.refChildren) {
  for (var id in this.refChildren) {
    var refChild = this.refChildren[id];
    if (refChild) refChild._each(segments, pos, fn);
  }
}

if (segments.length === pos) {
  fn(this);
  return;
}
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype._insert"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_insert (index, howMany)](#apidoc.element.derby.eventmodel.prototype._insert)
- description and source-code
```javascript
_insert = function (index, howMany) {
  // Update fixed paths
  this._updateArray(index);

  // Update relative paths
  if (this.arrayByReference && this.arrayByReference.length > index) {
    // Shift the actual items in the array references array.

    // This probably isn't the best way to implement insert. Other options are
    // using concat() on slices or though constructing a temporary array and
    // using splice.call. Hopefully if this method is slow it'll come up during
    // profiling.
    for (var i = 0; i < howMany; i++) {
      this.arrayByReference.splice(index, 0, null);
    }

    // Update the path in the contexts
    this._updateChildItemContexts(index + howMany);
  }

  // Finally call our bindings.
  if (this.bindings) {
    for (var id in this.bindings) {
      var binding = this.bindings[id];
      if (binding) binding.insert(index, howMany);
    }
  }
  this._updateObject();
}
```
- example usage
```shell
...
this.mutate(segments, function childSet(child) {
  child._set(previous, pass);
});
};

EventModel.prototype.insert = function(segments, index, howMany) {
this.mutate(segments, function childInsert(child) {
  child._insert(index, howMany);
});
};

EventModel.prototype.remove = function(segments, index, howMany) {
this.mutate(segments, function childRemove(child) {
  child._remove(index, howMany);
});
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype._move"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_move (from, to, howMany)](#apidoc.element.derby.eventmodel.prototype._move)
- description and source-code
```javascript
_move = function (from, to, howMany) {
  // first points to the first element that was moved. end points to the list
  // element past the end of the changed region.
  var first, end;
  if (from < to) {
    first = from;
    end = to + howMany;
  } else {
    first = to;
    end = from + howMany;
  }

  // Update fixed paths.
  this._updateArray(first, end);

  // Update relative paths
  var arr = this.arrayByReference;
  if (arr && arr.length > first) {
    // Remove from the old location
    var values = arr.splice(from, howMany);

    // Insert at the new location
    arr.splice.apply(arr, [to, 0].concat(values));

    // Update the path in the contexts
    this._updateChildItemContexts(first, end);
  }

  // Finally call our bindings.
  if (this.bindings) {
    for (var id in this.bindings) {
      var binding = this.bindings[id];
      if (binding) binding.move(from, to, howMany);
    }
  }
  this._updateObject();
}
```
- example usage
```shell
...
  this.mutate(segments, function childRemove(child) {
    child._remove(index, howMany);
  });
};

EventModel.prototype.move = function(segments, from, to, howMany) {
  this.mutate(segments, function childMove(child) {
    child._move(from, to, howMany);
  });
};
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype._remove"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_remove (index, howMany)](#apidoc.element.derby.eventmodel.prototype._remove)
- description and source-code
```javascript
_remove = function (index, howMany) {
  // Update fixed paths. Both the removed items and items after it may have changed.
  this._updateArray(index);

  if (this.arrayByReference) {
    // Update relative paths. First throw away all the children which have been removed.
    this.arrayByReference.splice(index, howMany);

    this._updateChildItemContexts(index);
  }

  // Call bindings.
  if (this.bindings) {
    for (var id in this.bindings) {
      var binding = this.bindings[id];
      if (binding) binding.remove(index, howMany);
    }
  }
  this._updateObject();
}
```
- example usage
```shell
...
this.mutate(segments, function childInsert(child) {
  child._insert(index, howMany);
});
};

EventModel.prototype.remove = function(segments, index, howMany) {
this.mutate(segments, function childRemove(child) {
  child._remove(index, howMany);
});
};

EventModel.prototype.move = function(segments, from, to, howMany) {
this.mutate(segments, function childMove(child) {
  child._move(from, to, howMany);
});
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype._removeItemContext"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_removeItemContext (context)](#apidoc.element.derby.eventmodel.prototype._removeItemContext)
- description and source-code
```javascript
_removeItemContext = function (context) {
  if (this.itemContexts) {
    delete this.itemContexts[context._id];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.eventmodel.prototype._set"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_set (previous, pass)](#apidoc.element.derby.eventmodel.prototype._set)
- description and source-code
```javascript
_set = function (previous, pass) {
  // This just updates anything thats bound to the whole subtree. An alternate
  // implementation could be passed in the new value at this node (which we
  // cache), then compare with the old version and only update parts of the
  // subtree which are relevant. I don't know if thats an important
  // optimization - it really depends on your use case.
  this.update(previous, pass);
}
```
- example usage
```shell
...
    var wildcardSegments = segments.slice(0, i);
    wildcardSegments.push('*');
    this._each(wildcardSegments, 0, childSetWildcard);
  }
};

function childSetWildcard(child) {
  child._set();
}

EventModel.prototype.set = function(segments, previous, pass) {
  this.mutate(segments, function childSet(child) {
    child._set(previous, pass);
  });
};
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype._updateArray"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_updateArray (from, to)](#apidoc.element.derby.eventmodel.prototype._updateArray)
- description and source-code
```javascript
_updateArray = function (from, to) {
  if (!this.array) return;

  if (from == null) from = 0;
  if (to == null) to = this.array.length;

  for (var i = from; i < to; i++) {
    var binding = this.array[i];
    if (binding) binding.update();
  }
}
```
- example usage
```shell
...
  // optimization - it really depends on your use case.
  this.update(previous, pass);
};

// Insert into this EventModel node.
EventModel.prototype._insert = function(index, howMany) {
  // Update fixed paths
  this._updateArray(index);

  // Update relative paths
  if (this.arrayByReference && this.arrayByReference.length > index) {
// Shift the actual items in the array references array.

// This probably isn't the best way to implement insert. Other options are
// using concat() on slices or though constructing a temporary array and
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype._updateChildItemContexts"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_updateChildItemContexts (from, to)](#apidoc.element.derby.eventmodel.prototype._updateChildItemContexts)
- description and source-code
```javascript
_updateChildItemContexts = function (from, to) {
  if (!this.arrayByReference) return;

  if (from == null) from = 0;
  if (to == null) to = this.arrayByReference.length;

  for (var i = from; i < to; i++) {
    var contexts = this.arrayByReference[i] &&
      this.arrayByReference[i].itemContexts;
    if (contexts) {
      for (var key in contexts) {
        contexts[key].item = i;
      }
    }
  }
}
```
- example usage
```shell
...
  // using splice.call. Hopefully if this method is slow it'll come up during
  // profiling.
  for (var i = 0; i < howMany; i++) {
    this.arrayByReference.splice(index, 0, null);
  }

  // Update the path in the contexts
  this._updateChildItemContexts(index + howMany);
}

// Finally call our bindings.
if (this.bindings) {
  for (var id in this.bindings) {
    var binding = this.bindings[id];
    if (binding) binding.insert(index, howMany);
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype._updateObject"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>_updateObject ()](#apidoc.element.derby.eventmodel.prototype._updateObject)
- description and source-code
```javascript
_updateObject = function () {
  if (this.object) {
    for (var key in this.object) {
      var binding = this.object[key];
      if (binding) binding.update();
    }
  }
}
```
- example usage
```shell
...
// Finally call our bindings.
if (this.bindings) {
  for (var id in this.bindings) {
    var binding = this.bindings[id];
    if (binding) binding.insert(index, howMany);
  }
}
this._updateObject();
};

// Remove howMany child elements from this EventModel at index.
EventModel.prototype._remove = function(index, howMany) {
// Update fixed paths. Both the removed items and items after it may have changed.
this._updateArray(index);
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.addBinding"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>addBinding (segments, binding)](#apidoc.element.derby.eventmodel.prototype.addBinding)
- description and source-code
```javascript
addBinding = function (segments, binding) {
  this.at(segments)._addBinding(binding);
}
```
- example usage
```shell
...
    this.eventModel.removeBinding(this);
  }
  // Add new dependencies
  if (!dependencies) return;
  this.dependencies = dependencies;
  for (var i = 0, len = dependencies.length; i < len; i++) {
    var dependency = dependencies[i];
    if (dependency) this.eventModel.addBinding(dependency, this);
  }
};
BindingWrapper.prototype.update = function(previous, pass) {
  this.binding.update(previous, pass);
  this.updateDependencies();
};
BindingWrapper.prototype.insert = function(index, howMany) {
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.addItemContext"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>addItemContext (segments, context)](#apidoc.element.derby.eventmodel.prototype.addItemContext)
- description and source-code
```javascript
addItemContext = function (segments, context) {
  this.at(segments)._addItemContext(context);
}
```
- example usage
```shell
...
this.context.meta.removeBinding = removeBinding;
this.context.meta.removeNode = removeNode;
this.context.meta.addItemContext = addItemContext;
this.context.meta.removeItemContext = removeItemContext;

function addItemContext(context) {
  var segments = context.expression.resolve(context);
  eventModel.addItemContext(segments, context);
}
function removeItemContext(context) {
  // TODO
}
function addBinding(binding) {
  patchTextBinding(binding);
  var expressions = binding.template.expressions;
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.arrayLookup"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>arrayLookup (model, segmentsBefore, segmentsInside)](#apidoc.element.derby.eventmodel.prototype.arrayLookup)
- description and source-code
```javascript
arrayLookup = function (model, segmentsBefore, segmentsInside) {
  var segments = expressions.pathSegments(segmentsInside);
  var item = expressions.lookup(segments, model.data);

  var source = this.at(segmentsInside);

  // What the array currently resolves to. Given x[y] with y=1, container is
  // the EM for x
  var container = this.at(segmentsBefore);

  if (!source.refOut) source.refOut = new RefOutMap();

  var ref = source.refOut[container.id];
  if (ref == null) {
    ref = new ModelRef(model, item, segmentsInside, container);
    source.refOut[container.id] = ref;
  }

  return ref;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.eventmodel.prototype.at"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>at (segments)](#apidoc.element.derby.eventmodel.prototype.at)
- description and source-code
```javascript
at = function (segments) {
  // For unbound dependancies.
  if (segments == null) return this;

  var eventModel = this;

  for (var i = 0; i < segments.length; i++) {
    eventModel = eventModel.child(segments[i]);
  }

  return eventModel;
}
```
- example usage
```shell
...
return this.refChildren[id];
};

EventModel.prototype.arrayLookup = function(model, segmentsBefore, segmentsInside) {
var segments = expressions.pathSegments(segmentsInside);
var item = expressions.lookup(segments, model.data);

var source = this.at(segmentsInside);

// What the array currently resolves to. Given x[y] with y=1, container is
// the EM for x
var container = this.at(segmentsBefore);

if (!source.refOut) source.refOut = new RefOutMap();
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.child"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>child (segment)](#apidoc.element.derby.eventmodel.prototype.child)
- description and source-code
```javascript
child = function (segment) {
  var container;
  if (typeof segment === 'string') {
    // Object
    if (!this.object) this.object = {};
    container = this.object;

  } else if (typeof segment === 'number') {
    // Array by value
    if (!this.array) this.array = [];
    container = this.array;

  } else if (segment instanceof ModelRef) {
    // Array reference. We'll need to lookup the child with the right
    // value, then look inside its ref children for the right EventModel
    // (so we can update it later). This is pretty janky, but should be
    // *correct* even in the face of recursive array accessors.
    //
    // This will calculate it based on the current segment values, but refs
    // cache the EM anyway.
    //return this.child(segment.item).refChild(segment);
    return segment.result;

  } else {
    // Array by reference
    if (!this.arrayByReference) this.arrayByReference = [];
    container = this.arrayByReference;
    segment = segment.item;
  }

  return container[segment] || (container[segment] = new EventModel());
}
```
- example usage
```shell
...

// outside is a reference to the EventModel of the thing on the lhs of the
// brackets. For example, in x[y].z, outside is the EventModel of x.
this.outside = outside;

// result is the EventModel of the evaluated version of the brackets. In
// x[y].z, its the EventModel of x[y].
this.result = outside.child(item).refChild(this);
}

ModelRef.prototype.update = function() {
var segments = expressions.pathSegments(this.segments);
var newItem = expressions.lookup(segments, this.model.data);
if (this.item === newItem) return;
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.insert"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>insert (segments, index, howMany)](#apidoc.element.derby.eventmodel.prototype.insert)
- description and source-code
```javascript
insert = function (segments, index, howMany) {
  this.mutate(segments, function childInsert(child) {
    child._insert(index, howMany);
  });
}
```
- example usage
```shell
...
});
var unloadListener = model.on('unload', '**', function onUnload(path) {
  var segments = util.castSegments(path.split('.'));
  eventModel.set(segments);
});
var insertListener = model.on('insert', '**', function onInsert(path, index, values) {
  var segments = util.castSegments(path.split('.'));
  eventModel.insert(segments, index, values.length);
});
var removeListener = model.on('remove', '**', function onRemove(path, index, values) {
  var segments = util.castSegments(path.split('.'));
  eventModel.remove(segments, index, values.length);
});
var moveListener = model.on('move', '**', function onMove(path, from, to, howMany) {
  var segments = util.castSegments(path.split('.'));
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>isEmpty ()](#apidoc.element.derby.eventmodel.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  if (hasKeys(this.dependancies)) return false;
  if (hasKeys(this.itemContexts)) return false;

  if (this.object) {
    if (hasKeys(this.object)) return false;
    this.object = null;
  }

  if (this.arrayByReference) {
    for (var i = 0; i < this.arrayByReference.length; i++) {
      if (this.arrayByReference[i] != null) return false;
    }
    this.arrayByReference = null;
  }

  if (this.array) {
    for (var i = 0; i < this.array.length; i++) {
      if (this.array[i] != null) return false;
    }
    this.array = null;
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.eventmodel.prototype.localUpdate"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>localUpdate (previous, pass)](#apidoc.element.derby.eventmodel.prototype.localUpdate)
- description and source-code
```javascript
localUpdate = function (previous, pass) {
  if (this.bindings) {
    for (var id in this.bindings) {
      var binding = this.bindings[id];
      if (binding) binding.update(previous, pass);
    }
  }

  // If our value changed, we also need to update anything that depends on it
  // via refOut.
  if (this.refOut) {
    for (var id in this.refOut) {
      var ref = this.refOut[id];
      if (ref) ref.update();
    }
  }
}
```
- example usage
```shell
...
    if (ref) ref.update();
  }
}
};

// This is used when an object subtree is replaced / removed.
EventModel.prototype.update = function(previous, pass) {
this.localUpdate(previous, pass);

if (this.object) {
  for (var key in this.object) {
    var binding = this.object[key];
    if (binding) binding.update();
  }
}
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.move"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>move (segments, from, to, howMany)](#apidoc.element.derby.eventmodel.prototype.move)
- description and source-code
```javascript
move = function (segments, from, to, howMany) {
  this.mutate(segments, function childMove(child) {
    child._move(from, to, howMany);
  });
}
```
- example usage
```shell
...
});
var removeListener = model.on('remove', '**', function onRemove(path, index, values) {
  var segments = util.castSegments(path.split('.'));
  eventModel.remove(segments, index, values.length);
});
var moveListener = model.on('move', '**', function onMove(path, from, to, howMany) {
  var segments = util.castSegments(path.split('.'));
  eventModel.move(segments, from, to, howMany);
});

this._removeModelListeners = function() {
  model.removeListener('change', changeListener);
  model.removeListener('load', loadListener);
  model.removeListener('unload', unloadListener);
  model.removeListener('insert', insertListener);
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.mutate"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>mutate (segments, fn)](#apidoc.element.derby.eventmodel.prototype.mutate)
- description and source-code
```javascript
mutate = function (segments, fn) {
  // This finds & returns a list of all event models which exist and could match
  // the specified path. The path cannot contain contexts like derby expression
  // segment lists (just because I don't think thats a useful feature and its not
  // implemented)
  this._each(segments, 0, fn);

  // Also emit all mutations as sets on star paths, which are how dependencies
  // for view helper functions are represented. They should react to a path
  // or any child path being modified
  for (var i = 0, len = segments.length; i++ < len;) {
    var wildcardSegments = segments.slice(0, i);
    wildcardSegments.push('*');
    this._each(wildcardSegments, 0, childSetWildcard);
  }
}
```
- example usage
```shell
...
};

function childSetWildcard(child) {
child._set();
}

EventModel.prototype.set = function(segments, previous, pass) {
this.mutate(segments, function childSet(child) {
  child._set(previous, pass);
});
};

EventModel.prototype.insert = function(segments, index, howMany) {
this.mutate(segments, function childInsert(child) {
  child._insert(index, howMany);
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.refChild"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>refChild (ref)](#apidoc.element.derby.eventmodel.prototype.refChild)
- description and source-code
```javascript
refChild = function (ref) {
  if (!this.refChildren) this.refChildren = new RefChildrenMap();
  var id = ref.id;

  if (!this.refChildren[id]) {
    this.refChildren[id] = new EventModel();
  }
  return this.refChildren[id];
}
```
- example usage
```shell
...

// outside is a reference to the EventModel of the thing on the lhs of the
// brackets. For example, in x[y].z, outside is the EventModel of x.
this.outside = outside;

// result is the EventModel of the evaluated version of the brackets. In
// x[y].z, its the EventModel of x[y].
this.result = outside.child(item).refChild(this);
}

ModelRef.prototype.update = function() {
var segments = expressions.pathSegments(this.segments);
var newItem = expressions.lookup(segments, this.model.data);
if (this.item === newItem) return;
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.remove"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>remove (segments, index, howMany)](#apidoc.element.derby.eventmodel.prototype.remove)
- description and source-code
```javascript
remove = function (segments, index, howMany) {
  this.mutate(segments, function childRemove(child) {
    child._remove(index, howMany);
  });
}
```
- example usage
```shell
...

Dom.prototype._initListeners = function() {
  var dom = this;
  this.controller.on('destroy', function domOnDestroy() {
    var listeners = dom._listeners;
    if (!listeners) return;
    for (var i = listeners.length; i--;) {
      listeners[i].remove();
    }
    dom._listeners = null;
  });
  return this._listeners = [];
};

Dom.prototype._listenerIndex = function(domListener) {
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.removeBinding"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>removeBinding (binding)](#apidoc.element.derby.eventmodel.prototype.removeBinding)
- description and source-code
```javascript
removeBinding = function (binding) {
  if (!binding.eventModels) return;
  for (var id in binding.eventModels) {
    var eventModel = binding.eventModels[id];
    if (eventModel.bindings) delete eventModel.bindings[binding.id];
  }
  binding.eventModels = null;
}
```
- example usage
```shell
...
    addDependencies(eventModel, expression, binding);
  }
}
function removeBinding(binding) {
  var bindingWrappers = binding.meta;
  if (!bindingWrappers) return;
  for (var i = bindingWrappers.length; i--;) {
    eventModel.removeBinding(bindingWrappers[i]);
  }
}
function removeNode(node) {
  var component = node.$component;
  if (component && !component.singleton) {
    component.destroy();
  }
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.set"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>set (segments, previous, pass)](#apidoc.element.derby.eventmodel.prototype.set)
- description and source-code
```javascript
set = function (segments, previous, pass) {
  this.mutate(segments, function childSet(child) {
    child._set(previous, pass);
  });
}
```
- example usage
```shell
...
  // Cancel any routing before the initial page attachment. Instead, do a
  // render once derby is ready
  this._cancelAttach = true;
  return;
}
this.emit('route', page);
// HACK: To update render in transitional routes
page.model.set('$render.params', page.params);
page.model.set('$render.url', page.params.url);
page.model.set('$render.query', page.params.query);
// If transitional
if (done) {
  var app = this;
  var _done = function() {
    app.emit('routeDone', page, 'transition');
...
```

#### <a name="apidoc.element.derby.eventmodel.prototype.update"></a>[function <span class="apidocSignatureSpan">derby.eventmodel.prototype.</span>update (previous, pass)](#apidoc.element.derby.eventmodel.prototype.update)
- description and source-code
```javascript
update = function (previous, pass) {
  this.localUpdate(previous, pass);

  if (this.object) {
    for (var key in this.object) {
      var binding = this.object[key];
      if (binding) binding.update();
    }
  }

  if (this.array) {
    for (var i = 0; i < this.array.length; i++) {
      var binding = this.array[i];
      if (binding) binding.update();
    }
  }

  if (this.arrayByReference) {
    for (var i = 0; i < this.arrayByReference.length; i++) {
      var binding = this.arrayByReference[i];
      if (binding) binding.update();
    }
  }
}
```
- example usage
```shell
...
  bundle.on('file', function(filename) {
    bundleFiles.push(filename);
  });
  app.emit('bundle', bundle);
});
backend.bundle(app.filename, options, function(err, source, map) {
  if (err) return cb(err);
  app.scriptHash = crypto.createHash('md5').update(source).digest('hex');
  source = source.replace('{{DERBY_SCRIPT_HASH}}', app.scriptHash);
  source = source.replace(/['"]{{DERBY_BUNDLED_AT}}['"]/, Date.now());
  if (!util.isProduction) {
    app._autoRefresh(backend);
    app._watchBundle(bundleFiles);
  }
  cb(null, source, map);
...
```



# <a name="apidoc.module.derby.files"></a>[module derby.files](#apidoc.module.derby.files)

#### <a name="apidoc.element.derby.files.cssCompiler"></a>[function <span class="apidocSignatureSpan">derby.files.</span>cssCompiler (file, filename, options)](#apidoc.element.derby.files.cssCompiler)
- description and source-code
```javascript
function cssCompiler(file, filename, options) {
  return {css: file, files: [filename]};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.files.htmlCompiler"></a>[function <span class="apidocSignatureSpan">derby.files.</span>htmlCompiler (file, filename)](#apidoc.element.derby.files.htmlCompiler)
- description and source-code
```javascript
function htmlCompiler(file, filename) {
  return file;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.derby.files.loadStylesSync"></a>[function <span class="apidocSignatureSpan">derby.files.</span>loadStylesSync (app, sourceFilename, options)](#apidoc.element.derby.files.loadStylesSync)
- description and source-code
```javascript
function loadStylesSync(app, sourceFilename, options) {
  options || (options = {compress: util.isProduction});
  var resolved = resolve.sync(sourceFilename, {extensions: app.styleExtensions, packageFilter: deleteMain});
  if (!resolved) {
    throw new Error('Style file not found: ' + sourceFilename);
  }
  var extension = path.extname(resolved);
  var compiler = app.compilers[extension];
  if (!compiler) {
    throw new Error('Unable to find compiler for: ' + extension);
  }
  var file = fs.readFileSync(resolved, 'utf8');
  return compiler(file, resolved, options);
}
```
- example usage
```shell
...
var stylesView = this.views.find('Styles');
stylesView.source += '<view is="' + filename + '"></view>';
// Make chainable
return this;
};

App.prototype._loadStyles = function(filename, options) {
var styles = files.loadStylesSync(this, filename, options);

var filepath = '';
if (!util.isProduction) {
  /**
   * Mark the path to file as an attribute
   * Used in development to add event watchers and autorefreshing of styles
   * SEE: local file, method this._watchStyles
...
```

#### <a name="apidoc.element.derby.files.loadViewsSync"></a>[function <span class="apidocSignatureSpan">derby.files.</span>loadViewsSync (app, sourceFilename, namespace)](#apidoc.element.derby.files.loadViewsSync)
- description and source-code
```javascript
function loadViewsSync(app, sourceFilename, namespace) {
  var views = [];
  var files = [];
  var resolved = resolve.sync(sourceFilename, {extensions: app.viewExtensions, packageFilter: deleteMain});
  if (!resolved) {
    throw new Error('View template file not found: ' + sourceFilename);
  }

  var file = fs.readFileSync(resolved, 'utf8');

  var extension = path.extname(resolved);
  var compiler = app.compilers[extension];
  if (!compiler) {
    throw new Error('Unable to find compiler for: ' + extension);
  }

  var htmlFile = compiler(file, resolved);

  var parsed = parseViews(namespace, htmlFile, resolved, app.viewExtensions);
  for (var i = 0, len = parsed.imports.length; i < len; i++) {
    var item = parsed.imports[i];
    var imported = loadViewsSync(app, item.filename, item.namespace);
    views = views.concat(imported.views);
    files = files.concat(imported.files);
  }
  return {
    views: views.concat(parsed.views)
  , files: files.concat(resolved)
  };
}
```
- example usage
```shell
...
var serialized = require(this.serializedBase + '.json');
serializedViews(derbyTemplates, this.views);
this.scriptUrl = (this.scriptBaseUrl || serialized.scriptBaseUrl) + serialized.scriptUrl;
this.scriptMapUrl = (this.scriptMapBaseUrl || serialized.scriptMapBaseUrl) + serialized.scriptMapUrl;
};

App.prototype.loadViews = function(filename, namespace) {
var data = files.loadViewsSync(this, filename, namespace);
for (var i = 0, len = data.views.length; i < len; i++) {
  var item = data.views[i];
  this.views.register(item.name, item.source, item.options);
}
if (!util.isProduction) this._watchViews(data.files, filename, namespace);
// Make chainable
return this;
...
```



# <a name="apidoc.module.derby.textDiff"></a>[module derby.textDiff](#apidoc.module.derby.textDiff)

#### <a name="apidoc.element.derby.textDiff.onStringInsert"></a>[function <span class="apidocSignatureSpan">derby.textDiff.</span>onStringInsert (el, previous, index, text)](#apidoc.element.derby.textDiff.onStringInsert)
- description and source-code
```javascript
function onStringInsert(el, previous, index, text) {
  function transformCursor(cursor) {
    return (index < cursor) ? cursor + text.length : cursor;
  }
  previous || (previous = '');
  var newText = previous.slice(0, index) + text + previous.slice(index);
  replaceText(el, newText, transformCursor);
}
```
- example usage
```shell
...
textUpdate(this, this.element, previous, pass);
}
function textUpdate(binding, element, previous, pass) {
if (pass) {
  if (pass.$event && pass.$event.target === element) {
    return;
  } else if (pass.$stringInsert) {
    return textDiff.onStringInsert(
      element,
      previous,
      pass.$stringInsert.index,
      pass.$stringInsert.text
    );
  } else if (pass.$stringRemove) {
    return textDiff.onStringRemove(
...
```

#### <a name="apidoc.element.derby.textDiff.onStringRemove"></a>[function <span class="apidocSignatureSpan">derby.textDiff.</span>onStringRemove (el, previous, index, howMany)](#apidoc.element.derby.textDiff.onStringRemove)
- description and source-code
```javascript
function onStringRemove(el, previous, index, howMany) {
  function transformCursor(cursor) {
    return (index < cursor) ? cursor - Math.min(howMany, cursor - index) : cursor;
  }
  previous || (previous = '');
  var newText = previous.slice(0, index) + previous.slice(index + howMany);
  replaceText(el, newText, transformCursor);
}
```
- example usage
```shell
...
    return textDiff.onStringInsert(
      element,
      previous,
      pass.$stringInsert.index,
      pass.$stringInsert.text
    );
  } else if (pass.$stringRemove) {
    return textDiff.onStringRemove(
      element,
      previous,
      pass.$stringRemove.index,
      pass.$stringRemove.howMany
    );
  }
}
...
```

#### <a name="apidoc.element.derby.textDiff.onTextInput"></a>[function <span class="apidocSignatureSpan">derby.textDiff.</span>onTextInput (model, segments, value)](#apidoc.element.derby.textDiff.onTextInput)
- description and source-code
```javascript
function onTextInput(model, segments, value) {
  var previous = model._get(segments) || '';
  if (previous === value) return;
  var start = 0;
  while (previous.charAt(start) === value.charAt(start)) {
    start++;
  }
  var end = 0;
  while (
    previous.charAt(previous.length - 1 - end) === value.charAt(value.length - 1 - end) &&
    end + start < previous.length &&
    end + start < value.length
  ) {
    end++;
  }

  if (previous.length !== start + end) {
    var howMany = previous.length - start - end;
    model._stringRemove(segments, start, howMany);
  }
  if (value.length !== start + end) {
    var inserted = value.slice(start, value.length - end);
    model._stringInsert(segments, start, inserted);
  }
}
```
- example usage
```shell
...
}

function textDiffBinding(binding, value, pass) {
var expression = binding.template.expression;
var segments = expression.pathSegments(binding.context);
if (segments) {
  var model = binding.context.controller.model.pass(pass);
  textDiff.onTextInput(model, segments, value);
} else if (expression.set) {
  expression.set(binding.context, value);
}
}

function setOptionBindings(parent) {
for (var node = parent.firstChild; node; node = node.nextSibling) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
