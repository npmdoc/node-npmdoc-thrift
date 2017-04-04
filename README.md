# api documentation for  [thrift (v0.10.0)](http://thrift.apache.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-thrift.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-thrift) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-thrift.svg)](https://travis-ci.org/npmdoc/node-npmdoc-thrift)
#### node.js bindings for the Apache Thrift RPC system

[![NPM](https://nodei.co/npm/thrift.png?downloads=true)](https://www.npmjs.com/package/thrift)

[![apidoc](https://npmdoc.github.io/node-npmdoc-thrift/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-thrift_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-thrift/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-thrift/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-thrift/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Apache Thrift Developers",
        "email": "dev@thrift.apache.org",
        "url": "http://thrift.apache.org"
    },
    "bugs": {
        "url": "https://issues.apache.org/jira/browse/THRIFT"
    },
    "dependencies": {
        "node-int64": "~0.3.0",
        "q": "1.0.x",
        "ws": "~0.4.32"
    },
    "description": "node.js bindings for the Apache Thrift RPC system",
    "devDependencies": {
        "buffer-equals": "^1.0.3",
        "commander": "2.1.x",
        "connect": "2.7.x",
        "istanbul": "^0.3.5",
        "run-browser": "^2.0.1",
        "tape": "~3.5.0"
    },
    "directories": {
        "lib": "./lib/nodejs/lib/thrift"
    },
    "dist": {
        "shasum": "339af65921677b30560aa51d6f7ab1b8091c9376",
        "tarball": "https://registry.npmjs.org/thrift/-/thrift-0.10.0.tgz"
    },
    "engines": {
        "node": ">= 0.2.4"
    },
    "files": [
        "lib/nodejs/lib/thrift",
        "lib/nodejs/README.md"
    ],
    "gitHead": "b2a4d4ae21c789b689dd162deb819665567f481c",
    "homepage": "http://thrift.apache.org/",
    "license": "Apache-2.0",
    "licenses": [
        {
            "type": "Apache-2.0",
            "url": "http://www.apache.org/licenses/LICENSE-2.0"
        }
    ],
    "main": "./lib/nodejs/lib/thrift",
    "maintainers": [
        {
            "name": "wadey",
            "email": "wade@wades.im"
        },
        {
            "name": "jfarrell",
            "email": "jfarrell@apache.org"
        }
    ],
    "name": "thrift",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "https://git-wip-us.apache.org/repos/asf/thrift.git"
    },
    "scripts": {
        "cover": "lib/nodejs/test/testAll.sh COVER",
        "test": "lib/nodejs/test/testAll.sh"
    },
    "version": "0.10.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module thrift](#apidoc.module.thrift)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Connection (stream, options)](#apidoc.element.thrift.Connection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>HttpConnection (host, port, options)](#apidoc.element.thrift.HttpConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Int64 (a1, a2)](#apidoc.element.thrift.Int64)
1.  [function <span class="apidocSignatureSpan">thrift.</span>MultiplexedProcessor (stream, options)](#apidoc.element.thrift.MultiplexedProcessor)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Multiplexer ()](#apidoc.element.thrift.Multiplexer)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Q (value)](#apidoc.element.thrift.Q)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Q.Promise (resolver)](#apidoc.element.thrift.Q.Promise)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Q.defer ()](#apidoc.element.thrift.Q.defer)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Q.makePromise (descriptor, fallback, inspect)](#apidoc.element.thrift.Q.makePromise)
1.  [function <span class="apidocSignatureSpan">thrift.</span>TBinaryProtocol (trans, strictRead, strictWrite)](#apidoc.element.thrift.TBinaryProtocol)
1.  [function <span class="apidocSignatureSpan">thrift.</span>TBufferedTransport (buffer, callback)](#apidoc.element.thrift.TBufferedTransport)
1.  [function <span class="apidocSignatureSpan">thrift.</span>TCompactProtocol (trans)](#apidoc.element.thrift.TCompactProtocol)
1.  [function <span class="apidocSignatureSpan">thrift.</span>TFramedTransport (buffer, callback)](#apidoc.element.thrift.TFramedTransport)
1.  [function <span class="apidocSignatureSpan">thrift.</span>TJSONProtocol (trans)](#apidoc.element.thrift.TJSONProtocol)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Thrift.TApplicationException (type, message)](#apidoc.element.thrift.Thrift.TApplicationException)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Thrift.TException (message)](#apidoc.element.thrift.Thrift.TException)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Thrift.TProtocolException (type, message)](#apidoc.element.thrift.Thrift.TProtocolException)
1.  [function <span class="apidocSignatureSpan">thrift.</span>WSConnection (host, port, options)](#apidoc.element.thrift.WSConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>XHRConnection (host, port, options)](#apidoc.element.thrift.XHRConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createClient (ServiceClient, connection)](#apidoc.element.thrift.createClient)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createConnection (host, port, options)](#apidoc.element.thrift.createConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createHttpClient (ServiceClient, connection)](#apidoc.element.thrift.createHttpClient)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createHttpConnection (host, port, options)](#apidoc.element.thrift.createHttpConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createMultiplexServer (processor, options)](#apidoc.element.thrift.createMultiplexServer)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createSSLConnection (host, port, options)](#apidoc.element.thrift.createSSLConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createServer (processor, handler, options)](#apidoc.element.thrift.createServer)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createStdIOClient (ServiceClient, connection)](#apidoc.element.thrift.createStdIOClient)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createStdIOConnection (command, options)](#apidoc.element.thrift.createStdIOConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createWSClient (ServiceClient, connection)](#apidoc.element.thrift.createWSClient)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createWSConnection (host, port, options)](#apidoc.element.thrift.createWSConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createWebServer (options)](#apidoc.element.thrift.createWebServer)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createXHRClient (ServiceClient, connection)](#apidoc.element.thrift.createXHRClient)
1.  [function <span class="apidocSignatureSpan">thrift.</span>createXHRConnection (host, port, options)](#apidoc.element.thrift.createXHRConnection)
1.  object <span class="apidocSignatureSpan">thrift.</span>Connection.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>HttpConnection.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>Int64.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>MultiplexedProcessor.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>Multiplexer.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>Q.defer.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>Q.makePromise.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>TBinaryProtocol.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>TBufferedTransport.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>TCompactProtocol.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>TFramedTransport.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>TJSONProtocol.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>Thrift
1.  object <span class="apidocSignatureSpan">thrift.</span>Thrift.TApplicationException.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>WSConnection.prototype
1.  object <span class="apidocSignatureSpan">thrift.</span>XHRConnection.prototype

#### [module thrift.Connection](#apidoc.module.thrift.Connection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Connection (stream, options)](#apidoc.element.thrift.Connection.Connection)
1.  [function <span class="apidocSignatureSpan">thrift.Connection.</span>super_ ()](#apidoc.element.thrift.Connection.super_)

#### [module thrift.Connection.prototype](#apidoc.module.thrift.Connection.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.Connection.prototype.</span>connection_gone ()](#apidoc.element.thrift.Connection.prototype.connection_gone)
1.  [function <span class="apidocSignatureSpan">thrift.Connection.prototype.</span>destroy ()](#apidoc.element.thrift.Connection.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">thrift.Connection.prototype.</span>end ()](#apidoc.element.thrift.Connection.prototype.end)
1.  [function <span class="apidocSignatureSpan">thrift.Connection.prototype.</span>initialize_retry_vars ()](#apidoc.element.thrift.Connection.prototype.initialize_retry_vars)
1.  [function <span class="apidocSignatureSpan">thrift.Connection.prototype.</span>write (data)](#apidoc.element.thrift.Connection.prototype.write)

#### [module thrift.HttpConnection](#apidoc.module.thrift.HttpConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>HttpConnection (host, port, options)](#apidoc.element.thrift.HttpConnection.HttpConnection)
1.  [function <span class="apidocSignatureSpan">thrift.HttpConnection.</span>super_ ()](#apidoc.element.thrift.HttpConnection.super_)

#### [module thrift.HttpConnection.prototype](#apidoc.module.thrift.HttpConnection.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.HttpConnection.prototype.</span>write (data)](#apidoc.element.thrift.HttpConnection.prototype.write)

#### [module thrift.Int64](#apidoc.module.thrift.Int64)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Int64 (a1, a2)](#apidoc.element.thrift.Int64.Int64)
1.  number <span class="apidocSignatureSpan">thrift.Int64.</span>MAX_INT
1.  number <span class="apidocSignatureSpan">thrift.Int64.</span>MIN_INT

#### [module thrift.Int64.prototype](#apidoc.module.thrift.Int64.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>_2scomp ()](#apidoc.element.thrift.Int64.prototype._2scomp)
1.  [function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>copy (targetBuffer, targetOffset)](#apidoc.element.thrift.Int64.prototype.copy)
1.  [function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>inspect ()](#apidoc.element.thrift.Int64.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>setValue (hi, lo)](#apidoc.element.thrift.Int64.prototype.setValue)
1.  [function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>toBuffer (rawBuffer)](#apidoc.element.thrift.Int64.prototype.toBuffer)
1.  [function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>toNumber (allowImprecise)](#apidoc.element.thrift.Int64.prototype.toNumber)
1.  [function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>toOctetString (sep)](#apidoc.element.thrift.Int64.prototype.toOctetString)
1.  [function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>toString (radix)](#apidoc.element.thrift.Int64.prototype.toString)
1.  [function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>valueOf ()](#apidoc.element.thrift.Int64.prototype.valueOf)

#### [module thrift.MultiplexedProcessor](#apidoc.module.thrift.MultiplexedProcessor)
1.  [function <span class="apidocSignatureSpan">thrift.</span>MultiplexedProcessor (stream, options)](#apidoc.element.thrift.MultiplexedProcessor.MultiplexedProcessor)

#### [module thrift.MultiplexedProcessor.prototype](#apidoc.module.thrift.MultiplexedProcessor.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.MultiplexedProcessor.prototype.</span>process (inp, out)](#apidoc.element.thrift.MultiplexedProcessor.prototype.process)
1.  [function <span class="apidocSignatureSpan">thrift.MultiplexedProcessor.prototype.</span>registerProcessor (name, handler)](#apidoc.element.thrift.MultiplexedProcessor.prototype.registerProcessor)

#### [module thrift.Multiplexer](#apidoc.module.thrift.Multiplexer)
1.  [function <span class="apidocSignatureSpan">thrift.</span>Multiplexer ()](#apidoc.element.thrift.Multiplexer.Multiplexer)

#### [module thrift.Multiplexer.prototype](#apidoc.module.thrift.Multiplexer.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.Multiplexer.prototype.</span>createClient (serviceName, ServiceClient, connection)](#apidoc.element.thrift.Multiplexer.prototype.createClient)

#### [module thrift.Q](#apidoc.module.thrift.Q)
1.  boolean <span class="apidocSignatureSpan">thrift.Q.</span>longStackSupport
1.  [function <span class="apidocSignatureSpan">thrift.</span>Q (value)](#apidoc.element.thrift.Q.Q)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>Promise (resolver)](#apidoc.element.thrift.Q.Promise)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>all (promises)](#apidoc.element.thrift.Q.all)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>allResolved ()](#apidoc.element.thrift.Q.allResolved)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>allSettled (promises)](#apidoc.element.thrift.Q.allSettled)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>async (makeGenerator)](#apidoc.element.thrift.Q.async)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>catch (object, rejected)](#apidoc.element.thrift.Q.catch)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>defer ()](#apidoc.element.thrift.Q.defer)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>del (object, key)](#apidoc.element.thrift.Q.del)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>delay (object, timeout)](#apidoc.element.thrift.Q.delay)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>delete (object, key)](#apidoc.element.thrift.Q.delete)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>denodeify (callback)](#apidoc.element.thrift.Q.denodeify)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>dispatch (object, op, args)](#apidoc.element.thrift.Q.dispatch)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>done (object, fulfilled, rejected, progress)](#apidoc.element.thrift.Q.done)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>fail (object, rejected)](#apidoc.element.thrift.Q.fail)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>fapply (object, args)](#apidoc.element.thrift.Q.fapply)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>fbind (object)](#apidoc.element.thrift.Q.fbind)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>fcall (object)](#apidoc.element.thrift.Q.fcall)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>fin (object, callback)](#apidoc.element.thrift.Q.fin)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>finally (object, callback)](#apidoc.element.thrift.Q.finally)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>fulfill (value)](#apidoc.element.thrift.Q.fulfill)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>get (object, key)](#apidoc.element.thrift.Q.get)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>getUnhandledReasons ()](#apidoc.element.thrift.Q.getUnhandledReasons)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>invoke (object, name)](#apidoc.element.thrift.Q.invoke)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>isFulfilled (object)](#apidoc.element.thrift.Q.isFulfilled)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>isPending (object)](#apidoc.element.thrift.Q.isPending)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>isPromise (object)](#apidoc.element.thrift.Q.isPromise)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>isPromiseAlike (object)](#apidoc.element.thrift.Q.isPromiseAlike)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>isRejected (object)](#apidoc.element.thrift.Q.isRejected)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>join (x, y)](#apidoc.element.thrift.Q.join)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>keys (object)](#apidoc.element.thrift.Q.keys)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>makePromise (descriptor, fallback, inspect)](#apidoc.element.thrift.Q.makePromise)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>mapply (object, name, args)](#apidoc.element.thrift.Q.mapply)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>master (object)](#apidoc.element.thrift.Q.master)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>mcall (object, name)](#apidoc.element.thrift.Q.mcall)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>nbind (callback, thisp)](#apidoc.element.thrift.Q.nbind)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>nearer (value)](#apidoc.element.thrift.Q.nearer)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>nextTick (task)](#apidoc.element.thrift.Q.nextTick)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>nfapply (callback, args)](#apidoc.element.thrift.Q.nfapply)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>nfbind (callback)](#apidoc.element.thrift.Q.nfbind)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>nfcall (callback)](#apidoc.element.thrift.Q.nfcall)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>ninvoke (object, name)](#apidoc.element.thrift.Q.ninvoke)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>nmapply (object, name, args)](#apidoc.element.thrift.Q.nmapply)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>nmcall (object, name)](#apidoc.element.thrift.Q.nmcall)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>nodeify (object, nodeback)](#apidoc.element.thrift.Q.nodeify)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>npost (object, name, args)](#apidoc.element.thrift.Q.npost)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>nsend (object, name)](#apidoc.element.thrift.Q.nsend)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>passByCopy (object)](#apidoc.element.thrift.Q.passByCopy)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>post (object, name, args)](#apidoc.element.thrift.Q.post)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>progress (object, progressed)](#apidoc.element.thrift.Q.progress)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>promise (resolver)](#apidoc.element.thrift.Q.promise)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>promised (callback)](#apidoc.element.thrift.Q.promised)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>race (answerPs)](#apidoc.element.thrift.Q.race)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>reject (reason)](#apidoc.element.thrift.Q.reject)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>resetUnhandledRejections ()](#apidoc.element.thrift.Q.resetUnhandledRejections)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>resolve (value)](#apidoc.element.thrift.Q.resolve)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>return (value)](#apidoc.element.thrift.Q.return)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>send (object, name)](#apidoc.element.thrift.Q.send)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>set (object, key, value)](#apidoc.element.thrift.Q.set)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>spawn (makeGenerator)](#apidoc.element.thrift.Q.spawn)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>spread (value, fulfilled, rejected)](#apidoc.element.thrift.Q.spread)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>stopUnhandledRejectionTracking ()](#apidoc.element.thrift.Q.stopUnhandledRejectionTracking)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>thenReject (promise, reason)](#apidoc.element.thrift.Q.thenReject)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>thenResolve (promise, value)](#apidoc.element.thrift.Q.thenResolve)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>timeout (object, ms, message)](#apidoc.element.thrift.Q.timeout)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>try (object)](#apidoc.element.thrift.Q.try)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>when (value, fulfilled, rejected, progressed)](#apidoc.element.thrift.Q.when)

#### [module thrift.Q.Promise](#apidoc.module.thrift.Q.Promise)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>Promise (resolver)](#apidoc.element.thrift.Q.Promise.Promise)
1.  [function <span class="apidocSignatureSpan">thrift.Q.Promise.</span>all (promises)](#apidoc.element.thrift.Q.Promise.all)
1.  [function <span class="apidocSignatureSpan">thrift.Q.Promise.</span>race (answerPs)](#apidoc.element.thrift.Q.Promise.race)
1.  [function <span class="apidocSignatureSpan">thrift.Q.Promise.</span>reject (reason)](#apidoc.element.thrift.Q.Promise.reject)
1.  [function <span class="apidocSignatureSpan">thrift.Q.Promise.</span>resolve (value)](#apidoc.element.thrift.Q.Promise.resolve)

#### [module thrift.Q.defer](#apidoc.module.thrift.Q.defer)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>defer ()](#apidoc.element.thrift.Q.defer.defer)

#### [module thrift.Q.defer.prototype](#apidoc.module.thrift.Q.defer.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.Q.defer.prototype.</span>makeNodeResolver ()](#apidoc.element.thrift.Q.defer.prototype.makeNodeResolver)

#### [module thrift.Q.makePromise](#apidoc.module.thrift.Q.makePromise)
1.  [function <span class="apidocSignatureSpan">thrift.Q.</span>makePromise (descriptor, fallback, inspect)](#apidoc.element.thrift.Q.makePromise.makePromise)

#### [module thrift.Q.makePromise.prototype](#apidoc.module.thrift.Q.makePromise.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>all ()](#apidoc.element.thrift.Q.makePromise.prototype.all)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>allResolved ()](#apidoc.element.thrift.Q.makePromise.prototype.allResolved)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>allSettled ()](#apidoc.element.thrift.Q.makePromise.prototype.allSettled)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>catch (rejected)](#apidoc.element.thrift.Q.makePromise.prototype.catch)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>del (key)](#apidoc.element.thrift.Q.makePromise.prototype.del)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>delay (timeout)](#apidoc.element.thrift.Q.makePromise.prototype.delay)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>delete (key)](#apidoc.element.thrift.Q.makePromise.prototype.delete)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>denodeify ()](#apidoc.element.thrift.Q.makePromise.prototype.denodeify)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>dispatch (op, args)](#apidoc.element.thrift.Q.makePromise.prototype.dispatch)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>done (fulfilled, rejected, progress)](#apidoc.element.thrift.Q.makePromise.prototype.done)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>fail (rejected)](#apidoc.element.thrift.Q.makePromise.prototype.fail)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>fapply (args)](#apidoc.element.thrift.Q.makePromise.prototype.fapply)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>fbind ()](#apidoc.element.thrift.Q.makePromise.prototype.fbind)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>fcall ()](#apidoc.element.thrift.Q.makePromise.prototype.fcall)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>fin (callback)](#apidoc.element.thrift.Q.makePromise.prototype.fin)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>finally (callback)](#apidoc.element.thrift.Q.makePromise.prototype.finally)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>get (key)](#apidoc.element.thrift.Q.makePromise.prototype.get)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>invoke (name)](#apidoc.element.thrift.Q.makePromise.prototype.invoke)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>isFulfilled ()](#apidoc.element.thrift.Q.makePromise.prototype.isFulfilled)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>isPending ()](#apidoc.element.thrift.Q.makePromise.prototype.isPending)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>isRejected ()](#apidoc.element.thrift.Q.makePromise.prototype.isRejected)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>join (that)](#apidoc.element.thrift.Q.makePromise.prototype.join)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>keys ()](#apidoc.element.thrift.Q.makePromise.prototype.keys)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>mapply (name, args)](#apidoc.element.thrift.Q.makePromise.prototype.mapply)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>mcall (name)](#apidoc.element.thrift.Q.makePromise.prototype.mcall)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nbind ()](#apidoc.element.thrift.Q.makePromise.prototype.nbind)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nfapply (args)](#apidoc.element.thrift.Q.makePromise.prototype.nfapply)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nfbind ()](#apidoc.element.thrift.Q.makePromise.prototype.nfbind)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nfcall ()](#apidoc.element.thrift.Q.makePromise.prototype.nfcall)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>ninvoke (name)](#apidoc.element.thrift.Q.makePromise.prototype.ninvoke)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nmapply (name, args)](#apidoc.element.thrift.Q.makePromise.prototype.nmapply)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nmcall (name)](#apidoc.element.thrift.Q.makePromise.prototype.nmcall)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nodeify (nodeback)](#apidoc.element.thrift.Q.makePromise.prototype.nodeify)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>npost (name, args)](#apidoc.element.thrift.Q.makePromise.prototype.npost)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nsend (name)](#apidoc.element.thrift.Q.makePromise.prototype.nsend)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>passByCopy ()](#apidoc.element.thrift.Q.makePromise.prototype.passByCopy)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>post (name, args)](#apidoc.element.thrift.Q.makePromise.prototype.post)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>progress (progressed)](#apidoc.element.thrift.Q.makePromise.prototype.progress)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>race ()](#apidoc.element.thrift.Q.makePromise.prototype.race)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>send (name)](#apidoc.element.thrift.Q.makePromise.prototype.send)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>set (key, value)](#apidoc.element.thrift.Q.makePromise.prototype.set)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>spread (fulfilled, rejected)](#apidoc.element.thrift.Q.makePromise.prototype.spread)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>then (fulfilled, rejected, progressed)](#apidoc.element.thrift.Q.makePromise.prototype.then)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>thenReject (reason)](#apidoc.element.thrift.Q.makePromise.prototype.thenReject)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>thenResolve (value)](#apidoc.element.thrift.Q.makePromise.prototype.thenResolve)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>timeout (ms, message)](#apidoc.element.thrift.Q.makePromise.prototype.timeout)
1.  [function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>toString ()](#apidoc.element.thrift.Q.makePromise.prototype.toString)

#### [module thrift.TBinaryProtocol](#apidoc.module.thrift.TBinaryProtocol)
1.  [function <span class="apidocSignatureSpan">thrift.</span>TBinaryProtocol (trans, strictRead, strictWrite)](#apidoc.element.thrift.TBinaryProtocol.TBinaryProtocol)

#### [module thrift.TBinaryProtocol.prototype](#apidoc.module.thrift.TBinaryProtocol.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>flush ()](#apidoc.element.thrift.TBinaryProtocol.prototype.flush)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>getTransport ()](#apidoc.element.thrift.TBinaryProtocol.prototype.getTransport)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readBinary ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readBinary)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readBool ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readBool)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readByte ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readByte)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readDouble ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readDouble)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readFieldBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readFieldBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readFieldEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readFieldEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readI16 ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readI16)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readI32 ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readI32)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readI64 ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readI64)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readListBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readListBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readListEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readListEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readMapBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readMapBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readMapEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readMapEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readMessageBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readMessageBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readMessageEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readMessageEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readSetBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readSetBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readSetEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readSetEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readString ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readString)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readStructBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readStructBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readStructEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readStructEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>skip (type)](#apidoc.element.thrift.TBinaryProtocol.prototype.skip)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeBinary (arg)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeBinary)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeBool (bool)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeBool)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeByte (b)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeByte)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeDouble (dub)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeDouble)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeFieldBegin (name, type, id)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeFieldBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeFieldEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeFieldEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeFieldStop ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeFieldStop)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeI16 (i16)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeI16)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeI32 (i32)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeI32)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeI64 (i64)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeI64)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeListBegin (etype, size)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeListBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeListEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeListEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeMapBegin (ktype, vtype, size)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeMapBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeMapEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeMapEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeMessageBegin (name, type, seqid)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeMessageBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeMessageEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeMessageEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeSetBegin (etype, size)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeSetBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeSetEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeSetEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeString (arg)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeString)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeStringOrBinary (name, encoding, arg)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeStringOrBinary)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeStructBegin (name)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeStructBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeStructEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeStructEnd)

#### [module thrift.TBufferedTransport](#apidoc.module.thrift.TBufferedTransport)
1.  [function <span class="apidocSignatureSpan">thrift.</span>TBufferedTransport (buffer, callback)](#apidoc.element.thrift.TBufferedTransport.TBufferedTransport)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.</span>receiver (callback, seqid)](#apidoc.element.thrift.TBufferedTransport.receiver)

#### [module thrift.TBufferedTransport.prototype](#apidoc.module.thrift.TBufferedTransport.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>borrow ()](#apidoc.element.thrift.TBufferedTransport.prototype.borrow)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>close ()](#apidoc.element.thrift.TBufferedTransport.prototype.close)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>commitPosition ()](#apidoc.element.thrift.TBufferedTransport.prototype.commitPosition)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>consume (bytesConsumed)](#apidoc.element.thrift.TBufferedTransport.prototype.consume)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>ensureAvailable (len)](#apidoc.element.thrift.TBufferedTransport.prototype.ensureAvailable)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>flush ()](#apidoc.element.thrift.TBufferedTransport.prototype.flush)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>isOpen ()](#apidoc.element.thrift.TBufferedTransport.prototype.isOpen)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>open ()](#apidoc.element.thrift.TBufferedTransport.prototype.open)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>read (len)](#apidoc.element.thrift.TBufferedTransport.prototype.read)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>readByte ()](#apidoc.element.thrift.TBufferedTransport.prototype.readByte)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>readDouble ()](#apidoc.element.thrift.TBufferedTransport.prototype.readDouble)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>readI16 ()](#apidoc.element.thrift.TBufferedTransport.prototype.readI16)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>readI32 ()](#apidoc.element.thrift.TBufferedTransport.prototype.readI32)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>readString (len)](#apidoc.element.thrift.TBufferedTransport.prototype.readString)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>rollbackPosition ()](#apidoc.element.thrift.TBufferedTransport.prototype.rollbackPosition)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>setCurrSeqId (seqid)](#apidoc.element.thrift.TBufferedTransport.prototype.setCurrSeqId)
1.  [function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>write (buf)](#apidoc.element.thrift.TBufferedTransport.prototype.write)

#### [module thrift.TCompactProtocol](#apidoc.module.thrift.TCompactProtocol)
1.  [function <span class="apidocSignatureSpan">thrift.</span>TCompactProtocol (trans)](#apidoc.element.thrift.TCompactProtocol.TCompactProtocol)
1.  number <span class="apidocSignatureSpan">thrift.TCompactProtocol.</span>PROTOCOL_ID
1.  number <span class="apidocSignatureSpan">thrift.TCompactProtocol.</span>TYPE_BITS
1.  number <span class="apidocSignatureSpan">thrift.TCompactProtocol.</span>TYPE_MASK
1.  number <span class="apidocSignatureSpan">thrift.TCompactProtocol.</span>TYPE_SHIFT_AMOUNT
1.  number <span class="apidocSignatureSpan">thrift.TCompactProtocol.</span>VERSION_MASK
1.  number <span class="apidocSignatureSpan">thrift.TCompactProtocol.</span>VERSION_N
1.  object <span class="apidocSignatureSpan">thrift.TCompactProtocol.</span>TTypeToCType
1.  object <span class="apidocSignatureSpan">thrift.TCompactProtocol.</span>Types

#### [module thrift.TCompactProtocol.prototype](#apidoc.module.thrift.TCompactProtocol.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>flush ()](#apidoc.element.thrift.TCompactProtocol.prototype.flush)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>getCompactType (ttype)](#apidoc.element.thrift.TCompactProtocol.prototype.getCompactType)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>getTType (type)](#apidoc.element.thrift.TCompactProtocol.prototype.getTType)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>getTransport ()](#apidoc.element.thrift.TCompactProtocol.prototype.getTransport)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>i32ToZigzag (n)](#apidoc.element.thrift.TCompactProtocol.prototype.i32ToZigzag)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>i64ToZigzag (l)](#apidoc.element.thrift.TCompactProtocol.prototype.i64ToZigzag)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readBinary ()](#apidoc.element.thrift.TCompactProtocol.prototype.readBinary)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readBool ()](#apidoc.element.thrift.TCompactProtocol.prototype.readBool)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readByte ()](#apidoc.element.thrift.TCompactProtocol.prototype.readByte)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readDouble ()](#apidoc.element.thrift.TCompactProtocol.prototype.readDouble)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readFieldBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readFieldBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readFieldEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readFieldEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readI16 ()](#apidoc.element.thrift.TCompactProtocol.prototype.readI16)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readI32 ()](#apidoc.element.thrift.TCompactProtocol.prototype.readI32)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readI64 ()](#apidoc.element.thrift.TCompactProtocol.prototype.readI64)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readListBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readListBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readListEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readListEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readMapBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readMapBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readMapEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readMapEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readMessageBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readMessageBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readMessageEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readMessageEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readSetBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readSetBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readSetEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readSetEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readString ()](#apidoc.element.thrift.TCompactProtocol.prototype.readString)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readStructBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readStructBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readStructEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readStructEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readVarint32 ()](#apidoc.element.thrift.TCompactProtocol.prototype.readVarint32)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readVarint64 ()](#apidoc.element.thrift.TCompactProtocol.prototype.readVarint64)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>skip (type)](#apidoc.element.thrift.TCompactProtocol.prototype.skip)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeBinary (arg)](#apidoc.element.thrift.TCompactProtocol.prototype.writeBinary)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeBool (value)](#apidoc.element.thrift.TCompactProtocol.prototype.writeBool)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeByte (b)](#apidoc.element.thrift.TCompactProtocol.prototype.writeByte)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeCollectionBegin (elemType, size)](#apidoc.element.thrift.TCompactProtocol.prototype.writeCollectionBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeDouble (v)](#apidoc.element.thrift.TCompactProtocol.prototype.writeDouble)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeFieldBegin (name, type, id)](#apidoc.element.thrift.TCompactProtocol.prototype.writeFieldBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeFieldBeginInternal (name, fieldType, fieldId, typeOverride)](#apidoc.element.thrift.TCompactProtocol.prototype.writeFieldBeginInternal)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeFieldEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeFieldEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeFieldStop ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeFieldStop)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeI16 (i16)](#apidoc.element.thrift.TCompactProtocol.prototype.writeI16)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeI32 (i32)](#apidoc.element.thrift.TCompactProtocol.prototype.writeI32)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeI64 (i64)](#apidoc.element.thrift.TCompactProtocol.prototype.writeI64)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeListBegin (elemType, size)](#apidoc.element.thrift.TCompactProtocol.prototype.writeListBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeListEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeListEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeMapBegin (keyType, valType, size)](#apidoc.element.thrift.TCompactProtocol.prototype.writeMapBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeMapEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeMapEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeMessageBegin (name, type, seqid)](#apidoc.element.thrift.TCompactProtocol.prototype.writeMessageBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeMessageEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeMessageEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeSetBegin (elemType, size)](#apidoc.element.thrift.TCompactProtocol.prototype.writeSetBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeSetEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeSetEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeString (arg)](#apidoc.element.thrift.TCompactProtocol.prototype.writeString)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeStringOrBinary (name, encoding, arg)](#apidoc.element.thrift.TCompactProtocol.prototype.writeStringOrBinary)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeStructBegin (name)](#apidoc.element.thrift.TCompactProtocol.prototype.writeStructBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeStructEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeStructEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeVarint32 (n)](#apidoc.element.thrift.TCompactProtocol.prototype.writeVarint32)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeVarint64 (n)](#apidoc.element.thrift.TCompactProtocol.prototype.writeVarint64)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>zigzagToI32 (n)](#apidoc.element.thrift.TCompactProtocol.prototype.zigzagToI32)
1.  [function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>zigzagToI64 (n)](#apidoc.element.thrift.TCompactProtocol.prototype.zigzagToI64)

#### [module thrift.TFramedTransport](#apidoc.module.thrift.TFramedTransport)
1.  [function <span class="apidocSignatureSpan">thrift.</span>TFramedTransport (buffer, callback)](#apidoc.element.thrift.TFramedTransport.TFramedTransport)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.</span>receiver (callback, seqid)](#apidoc.element.thrift.TFramedTransport.receiver)

#### [module thrift.TFramedTransport.prototype](#apidoc.module.thrift.TFramedTransport.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>borrow ()](#apidoc.element.thrift.TFramedTransport.prototype.borrow)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>close ()](#apidoc.element.thrift.TFramedTransport.prototype.close)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>commitPosition ()](#apidoc.element.thrift.TFramedTransport.prototype.commitPosition)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>consume (bytesConsumed)](#apidoc.element.thrift.TFramedTransport.prototype.consume)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>ensureAvailable (len)](#apidoc.element.thrift.TFramedTransport.prototype.ensureAvailable)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>flush ()](#apidoc.element.thrift.TFramedTransport.prototype.flush)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>isOpen ()](#apidoc.element.thrift.TFramedTransport.prototype.isOpen)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>open ()](#apidoc.element.thrift.TFramedTransport.prototype.open)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>read (len)](#apidoc.element.thrift.TFramedTransport.prototype.read)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>readByte ()](#apidoc.element.thrift.TFramedTransport.prototype.readByte)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>readDouble ()](#apidoc.element.thrift.TFramedTransport.prototype.readDouble)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>readI16 ()](#apidoc.element.thrift.TFramedTransport.prototype.readI16)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>readI32 ()](#apidoc.element.thrift.TFramedTransport.prototype.readI32)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>readString (len)](#apidoc.element.thrift.TFramedTransport.prototype.readString)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>rollbackPosition ()](#apidoc.element.thrift.TFramedTransport.prototype.rollbackPosition)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>setCurrSeqId (seqid)](#apidoc.element.thrift.TFramedTransport.prototype.setCurrSeqId)
1.  [function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>write (buf, encoding)](#apidoc.element.thrift.TFramedTransport.prototype.write)

#### [module thrift.TJSONProtocol](#apidoc.module.thrift.TJSONProtocol)
1.  [function <span class="apidocSignatureSpan">thrift.</span>TJSONProtocol (trans)](#apidoc.element.thrift.TJSONProtocol.TJSONProtocol)
1.  number <span class="apidocSignatureSpan">thrift.TJSONProtocol.</span>Version
1.  object <span class="apidocSignatureSpan">thrift.TJSONProtocol.</span>RType
1.  object <span class="apidocSignatureSpan">thrift.TJSONProtocol.</span>Type

#### [module thrift.TJSONProtocol.prototype](#apidoc.module.thrift.TJSONProtocol.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>flush ()](#apidoc.element.thrift.TJSONProtocol.prototype.flush)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>getTransport ()](#apidoc.element.thrift.TJSONProtocol.prototype.getTransport)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readBinary ()](#apidoc.element.thrift.TJSONProtocol.prototype.readBinary)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readBool ()](#apidoc.element.thrift.TJSONProtocol.prototype.readBool)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readByte ()](#apidoc.element.thrift.TJSONProtocol.prototype.readByte)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readDouble ()](#apidoc.element.thrift.TJSONProtocol.prototype.readDouble)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readFieldBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readFieldBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readFieldEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readFieldEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readI16 ()](#apidoc.element.thrift.TJSONProtocol.prototype.readI16)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readI32 (f)](#apidoc.element.thrift.TJSONProtocol.prototype.readI32)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readI64 ()](#apidoc.element.thrift.TJSONProtocol.prototype.readI64)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readListBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readListBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readListEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readListEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readMapBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readMapBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readMapEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readMapEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readMessageBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readMessageBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readMessageEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readMessageEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readSetBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readSetBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readSetEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readSetEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readString ()](#apidoc.element.thrift.TJSONProtocol.prototype.readString)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readStructBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readStructBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readStructEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readStructEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readValue (f)](#apidoc.element.thrift.TJSONProtocol.prototype.readValue)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>skip (type)](#apidoc.element.thrift.TJSONProtocol.prototype.skip)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeBinary (arg)](#apidoc.element.thrift.TJSONProtocol.prototype.writeBinary)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeBool (bool)](#apidoc.element.thrift.TJSONProtocol.prototype.writeBool)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeByte (byte)](#apidoc.element.thrift.TJSONProtocol.prototype.writeByte)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeDouble (dub)](#apidoc.element.thrift.TJSONProtocol.prototype.writeDouble)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeFieldBegin (name, fieldType, fieldId)](#apidoc.element.thrift.TJSONProtocol.prototype.writeFieldBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeFieldEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeFieldEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeFieldStop ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeFieldStop)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeI16 (i16)](#apidoc.element.thrift.TJSONProtocol.prototype.writeI16)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeI32 (i32)](#apidoc.element.thrift.TJSONProtocol.prototype.writeI32)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeI64 (i64)](#apidoc.element.thrift.TJSONProtocol.prototype.writeI64)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeListBegin (elemType, size)](#apidoc.element.thrift.TJSONProtocol.prototype.writeListBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeListEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeListEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeMapBegin (keyType, valType, size)](#apidoc.element.thrift.TJSONProtocol.prototype.writeMapBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeMapEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeMapEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeMessageBegin (name, messageType, seqid)](#apidoc.element.thrift.TJSONProtocol.prototype.writeMessageBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeMessageEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeMessageEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeSetBegin (elemType, size)](#apidoc.element.thrift.TJSONProtocol.prototype.writeSetBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeSetEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeSetEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeString (arg)](#apidoc.element.thrift.TJSONProtocol.prototype.writeString)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeStructBegin (name)](#apidoc.element.thrift.TJSONProtocol.prototype.writeStructBegin)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeStructEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeStructEnd)
1.  [function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeToTransportIfStackIsFlushable ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeToTransportIfStackIsFlushable)

#### [module thrift.Thrift](#apidoc.module.thrift.Thrift)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.</span>TApplicationException (type, message)](#apidoc.element.thrift.Thrift.TApplicationException)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.</span>TException (message)](#apidoc.element.thrift.Thrift.TException)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.</span>TProtocolException (type, message)](#apidoc.element.thrift.Thrift.TProtocolException)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.</span>copyList (lst, types)](#apidoc.element.thrift.Thrift.copyList)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.</span>copyMap (obj, types)](#apidoc.element.thrift.Thrift.copyMap)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.</span>inherits (constructor, superConstructor)](#apidoc.element.thrift.Thrift.inherits)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.</span>objectLength (obj)](#apidoc.element.thrift.Thrift.objectLength)
1.  object <span class="apidocSignatureSpan">thrift.Thrift.</span>MessageType
1.  object <span class="apidocSignatureSpan">thrift.Thrift.</span>TApplicationExceptionType
1.  object <span class="apidocSignatureSpan">thrift.Thrift.</span>TProtocolExceptionType
1.  object <span class="apidocSignatureSpan">thrift.Thrift.</span>Type

#### [module thrift.Thrift.TApplicationException](#apidoc.module.thrift.Thrift.TApplicationException)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.</span>TApplicationException (type, message)](#apidoc.element.thrift.Thrift.TApplicationException.TApplicationException)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.TApplicationException.</span>super_ (message)](#apidoc.element.thrift.Thrift.TApplicationException.super_)

#### [module thrift.Thrift.TApplicationException.prototype](#apidoc.module.thrift.Thrift.TApplicationException.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.TApplicationException.prototype.</span>read (input)](#apidoc.element.thrift.Thrift.TApplicationException.prototype.read)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.TApplicationException.prototype.</span>write (output)](#apidoc.element.thrift.Thrift.TApplicationException.prototype.write)

#### [module thrift.Thrift.TException](#apidoc.module.thrift.Thrift.TException)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.</span>TException (message)](#apidoc.element.thrift.Thrift.TException.TException)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.TException.</span>super_ ()](#apidoc.element.thrift.Thrift.TException.super_)

#### [module thrift.Thrift.TProtocolException](#apidoc.module.thrift.Thrift.TProtocolException)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.</span>TProtocolException (type, message)](#apidoc.element.thrift.Thrift.TProtocolException.TProtocolException)
1.  [function <span class="apidocSignatureSpan">thrift.Thrift.TProtocolException.</span>super_ ()](#apidoc.element.thrift.Thrift.TProtocolException.super_)

#### [module thrift.WSConnection](#apidoc.module.thrift.WSConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>WSConnection (host, port, options)](#apidoc.element.thrift.WSConnection.WSConnection)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.</span>super_ ()](#apidoc.element.thrift.WSConnection.super_)

#### [module thrift.WSConnection.prototype](#apidoc.module.thrift.WSConnection.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__decodeCallback (transport_with_data)](#apidoc.element.thrift.WSConnection.prototype.__decodeCallback)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__onClose (evt)](#apidoc.element.thrift.WSConnection.prototype.__onClose)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__onData (data)](#apidoc.element.thrift.WSConnection.prototype.__onData)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__onError (evt)](#apidoc.element.thrift.WSConnection.prototype.__onError)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__onMessage (evt)](#apidoc.element.thrift.WSConnection.prototype.__onMessage)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__onOpen ()](#apidoc.element.thrift.WSConnection.prototype.__onOpen)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__reset ()](#apidoc.element.thrift.WSConnection.prototype.__reset)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>close ()](#apidoc.element.thrift.WSConnection.prototype.close)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>isOpen ()](#apidoc.element.thrift.WSConnection.prototype.isOpen)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>open ()](#apidoc.element.thrift.WSConnection.prototype.open)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>uri ()](#apidoc.element.thrift.WSConnection.prototype.uri)
1.  [function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>write (data)](#apidoc.element.thrift.WSConnection.prototype.write)

#### [module thrift.XHRConnection](#apidoc.module.thrift.XHRConnection)
1.  [function <span class="apidocSignatureSpan">thrift.</span>XHRConnection (host, port, options)](#apidoc.element.thrift.XHRConnection.XHRConnection)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.</span>super_ ()](#apidoc.element.thrift.XHRConnection.super_)

#### [module thrift.XHRConnection.prototype](#apidoc.module.thrift.XHRConnection.prototype)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>__decodeCallback (transport_with_data)](#apidoc.element.thrift.XHRConnection.prototype.__decodeCallback)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>close ()](#apidoc.element.thrift.XHRConnection.prototype.close)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>flush ()](#apidoc.element.thrift.XHRConnection.prototype.flush)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>getSendBuffer ()](#apidoc.element.thrift.XHRConnection.prototype.getSendBuffer)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>getXmlHttpRequestObject ()](#apidoc.element.thrift.XHRConnection.prototype.getXmlHttpRequestObject)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>isOpen ()](#apidoc.element.thrift.XHRConnection.prototype.isOpen)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>open ()](#apidoc.element.thrift.XHRConnection.prototype.open)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>read (len)](#apidoc.element.thrift.XHRConnection.prototype.read)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>readAll ()](#apidoc.element.thrift.XHRConnection.prototype.readAll)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>setRecvBuffer (buf)](#apidoc.element.thrift.XHRConnection.prototype.setRecvBuffer)
1.  [function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>write (buf)](#apidoc.element.thrift.XHRConnection.prototype.write)



# <a name="apidoc.module.thrift"></a>[module thrift](#apidoc.module.thrift)

#### <a name="apidoc.element.thrift.Connection"></a>[function <span class="apidocSignatureSpan">thrift.</span>Connection (stream, options)](#apidoc.element.thrift.Connection)
- description and source-code
```javascript
Connection = function (stream, options) {
  var self = this;
  EventEmitter.call(this);

  this.seqId2Service = {};
  this.connection = stream;
  this.ssl = (stream.encrypted);
  this.options = options || {};
  this.transport = this.options.transport || TBufferedTransport;
  this.protocol = this.options.protocol || TBinaryProtocol;
  this.offline_queue = [];
  this.connected = false;
  this.initialize_retry_vars();

  this._debug = this.options.debug || false;
  if (this.options.max_attempts &&
      !isNaN(this.options.max_attempts) &&
      this.options.max_attempts > 0) {
     this.max_attempts = +this.options.max_attempts;
  }
  this.retry_max_delay = null;
  if (this.options.retry_max_delay !== undefined &&
      !isNaN(this.options.retry_max_delay) &&
      this.options.retry_max_delay > 0) {
     this.retry_max_delay = this.options.retry_max_delay;
  }
  this.connect_timeout = false;
  if (this.options.connect_timeout &&
      !isNaN(this.options.connect_timeout) &&
      this.options.connect_timeout > 0) {
     this.connect_timeout = +this.options.connect_timeout;
  }

  this.connection.addListener(this.ssl ? "secureConnect" : "connect", function() {
    self.connected = true;

    this.setTimeout(self.options.timeout || 0);
    this.setNoDelay();
    this.frameLeft = 0;
    this.framePos = 0;
    this.frame = null;
    self.initialize_retry_vars();

    self.offline_queue.forEach(function(data) {
      self.connection.write(data);
    });

    self.emit("connect");
  });

  this.connection.addListener("error", function(err) {
    // Only emit the error if no-one else is listening on the connection
    // or if someone is listening on us, because Node turns unhandled
    // 'error' events into exceptions.
    if (self.connection.listeners('error').length === 1 ||
        self.listeners('error').length > 0) {
      self.emit("error", err);
    }
  });

  // Add a close listener
  this.connection.addListener("close", function() {
    self.connection_gone(); // handle close event. try to reconnect
  });

  this.connection.addListener("timeout", function() {
    self.emit("timeout");
  });

  this.connection.addListener("data", self.transport.receiver(function(transport_with_data) {
    var message = new self.protocol(transport_with_data);
    try {
      while (true) {
        var header = message.readMessageBegin();
        var dummy_seqid = header.rseqid * -1;
        var client = self.client;
        //The Multiplexed Protocol stores a hash of seqid to service names
        //  in seqId2Service. If the SeqId is found in the hash we need to
        //  lookup the appropriate client for this call.
        //  The connection.client object is a single client object when not
        //  multiplexing, when using multiplexing it is a service name keyed
        //  hash of client objects.
        //NOTE: The 2 way interdependencies between protocols, transports,
        //  connections and clients in the Node.js implementation are irregular
        //  and make the implementation difficult to extend and maintain. We
        //  should bring this stuff inline with typical thrift I/O stack
        //  operation soon.
        //  --ra
        var service_name = self.seqId2Service[header.rseqid];
        if (service_name) {
          client = self.client[service_name];
          delete self.seqId2Service[header.rseqid];
        }
<span class="apidocCodeCommentSpan">        /*jshint -W083 */
</span>        client._reqs[dummy_seqid] = function(err, success){
          transport_with_data.commitPosition();

          var callback = client._reqs[header.rseqid];
          delete client._reqs[header.rseqid];
          if (callback) {
            callback(err, success);
          }
        };
        /*jshint +W083 */

        if(client['recv_' + header.fname]) {
          client['recv_' + header.fname](message, header.mtype, dummy_seqid);
        } else {
          delete client._reqs[dummy_seqid];
          self.emit("error",
                    new thrift.TApplicationException(thrift.TApplicationExceptionType.WRONG_METHOD_NAME,
                             "Received a response to an ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.HttpConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>HttpConnection (host, port, options)](#apidoc.element.thrift.HttpConnection)
- description and source-code
```javascript
HttpConnection = function (host, port, options) {
  //Initialize the emitter base object
  EventEmitter.call(this);

  //Set configuration
  var self = this;
  this.options = options || {};
  this.host = host;
  this.port = port;
  this.https = this.options.https || false;
  this.transport = this.options.transport || TBufferedTransport;
  this.protocol = this.options.protocol || TBinaryProtocol;

  //Prepare Node.js options
  this.nodeOptions = {
    host: this.host,
    port: this.port || 80,
    path: this.options.path || '/',
    method: 'POST',
    headers: this.options.headers || {},
    responseType: this.options.responseType || null
  };
  for (var attrname in this.options.nodeOptions) {
    this.nodeOptions[attrname] = this.options.nodeOptions[attrname];
  }
<span class="apidocCodeCommentSpan">  /*jshint -W069 */
</span>  if (! this.nodeOptions.headers['Connection']) {
    this.nodeOptions.headers['Connection'] = 'keep-alive';
  }
  /*jshint +W069 */

  //The sequence map is used to map seqIDs back to the
  //  calling client in multiplexed scenarios
  this.seqId2Service = {};

  function decodeCallback(transport_with_data) {
    var proto = new self.protocol(transport_with_data);
    try {
      while (true) {
        var header = proto.readMessageBegin();
        var dummy_seqid = header.rseqid * -1;
        var client = self.client;
        //The Multiplexed Protocol stores a hash of seqid to service names
        //  in seqId2Service. If the SeqId is found in the hash we need to
        //  lookup the appropriate client for this call.
        //  The client var is a single client object when not multiplexing,
        //  when using multiplexing it is a service name keyed hash of client
        //  objects.
        //NOTE: The 2 way interdependencies between protocols, transports,
        //  connections and clients in the Node.js implementation are irregular
        //  and make the implementation difficult to extend and maintain. We
        //  should bring this stuff inline with typical thrift I/O stack
        //  operation soon.
        //  --ra
        var service_name = self.seqId2Service[header.rseqid];
        if (service_name) {
          client = self.client[service_name];
          delete self.seqId2Service[header.rseqid];
        }
        /*jshint -W083 */
        client._reqs[dummy_seqid] = function(err, success){
          transport_with_data.commitPosition();
          var clientCallback = client._reqs[header.rseqid];
          delete client._reqs[header.rseqid];
          if (clientCallback) {
            process.nextTick(function() {
              clientCallback(err, success);
            });
          }
        };
        /*jshint +W083 */
        if(client['recv_' + header.fname]) {
          client['recv_' + header.fname](proto, header.mtype, dummy_seqid);
        } else {
          delete client._reqs[dummy_seqid];
          self.emit("error",
                    new thrift.TApplicationException(
                       thrift.TApplicationExceptionType.WRONG_METHOD_NAME,
                       "Received a response to an unknown RPC function"));
        }
      }
    }
    catch (e) {
      if (e instanceof InputBufferUnderrunError) {
        transport_with_data.rollbackPosition();
      } else {
        self.emit('error', e);
      }
    }
  }


  //Response handler
  //////////////////////////////////////////////////
  this.responseCallback = function(response) {
    var data = [];
    var dataLen = 0;

    response.on('error', function (e) {
      self.emit("error", e);
    });

    // When running directly under node, chunk will be a buffer,
    // however, when running in a Browser (e.g. Browserify), chunk
    // will be a string or an ArrayBuffer.
    response.on('data', function (chunk) {
      if ((typeof chunk == 'string') ||
          (Object.prototype.toString.call(chunk) == '[object Uint8Array]')) {
        // Wrap ArrayBuffer/string in a Buffer so data[i].copy will work
        data.push(new Buffer(chunk));
      } else {
        data.push(chunk);
      }
      dataLen += chunk.length;
    });

    response.on('end', function(){ ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Int64"></a>[function <span class="apidocSignatureSpan">thrift.</span>Int64 (a1, a2)](#apidoc.element.thrift.Int64)
- description and source-code
```javascript
Int64 = function (a1, a2) {
  if (a1 instanceof Buffer) {
    this.buffer = a1;
    this.offset = a2 || 0;
  } else if (Object.prototype.toString.call(a1) == '[object Uint8Array]') {
    // Under Browserify, Buffers can extend Uint8Arrays rather than an
    // instance of Buffer. We could assume the passed in Uint8Array is actually
    // a buffer but that won't handle the case where a raw Uint8Array is passed
    // in. We construct a new Buffer just in case.
    this.buffer = new Buffer(a1);
    this.offset = a2 || 0;
  } else {
    this.buffer = this.buffer || new Buffer(8);
    this.offset = 0;
    this.setValue.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.MultiplexedProcessor"></a>[function <span class="apidocSignatureSpan">thrift.</span>MultiplexedProcessor (stream, options)](#apidoc.element.thrift.MultiplexedProcessor)
- description and source-code
```javascript
function MultiplexedProcessor(stream, options) {
  this.services = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Multiplexer"></a>[function <span class="apidocSignatureSpan">thrift.</span>Multiplexer ()](#apidoc.element.thrift.Multiplexer)
- description and source-code
```javascript
function Multiplexer() {
  this.seqid = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q"></a>[function <span class="apidocSignatureSpan">thrift.</span>Q (value)](#apidoc.element.thrift.Q)
- description and source-code
```javascript
function Q(value) {
    // If the object is already a Promise, return it directly.  This enables
    // the resolve function to both be used to created references from objects,
    // but to tolerably coerce non-promises to promises.
    if (isPromise(value)) {
        return value;
    }

    // assimilate thenables
    if (isPromiseAlike(value)) {
        return coerce(value);
    } else {
        return fulfill(value);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.Promise"></a>[function <span class="apidocSignatureSpan">thrift.</span>Q.Promise (resolver)](#apidoc.element.thrift.Q.Promise)
- description and source-code
```javascript
function promise(resolver) {
    if (typeof resolver !== "function") {
        throw new TypeError("resolver must be a function.");
    }
    var deferred = defer();
    try {
        resolver(deferred.resolve, deferred.reject, deferred.notify);
    } catch (reason) {
        deferred.reject(reason);
    }
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.defer"></a>[function <span class="apidocSignatureSpan">thrift.</span>Q.defer ()](#apidoc.element.thrift.Q.defer)
- description and source-code
```javascript
function defer() {
    // if "messages" is an "Array", that indicates that the promise has not yet
    // been resolved.  If it is "undefined", it has been resolved.  Each
    // element of the messages array is itself an array of complete arguments to
    // forward to the resolved promise.  We coerce the resolution value to a
    // promise using the 'resolve' function because it handles both fully
    // non-thenable values and other thenables gracefully.
    var messages = [], progressListeners = [], resolvedPromise;

    var deferred = object_create(defer.prototype);
    var promise = object_create(Promise.prototype);

    promise.promiseDispatch = function (resolve, op, operands) {
        var args = array_slice(arguments);
        if (messages) {
            messages.push(args);
            if (op === "when" && operands[1]) { // progress operand
                progressListeners.push(operands[1]);
            }
        } else {
            nextTick(function () {
                resolvedPromise.promiseDispatch.apply(resolvedPromise, args);
            });
        }
    };

    // XXX deprecated
    promise.valueOf = function () {
        if (messages) {
            return promise;
        }
        var nearerValue = nearer(resolvedPromise);
        if (isPromise(nearerValue)) {
            resolvedPromise = nearerValue; // shorten chain
        }
        return nearerValue;
    };

    promise.inspect = function () {
        if (!resolvedPromise) {
            return { state: "pending" };
        }
        return resolvedPromise.inspect();
    };

    if (Q.longStackSupport && hasStacks) {
        try {
            throw new Error();
        } catch (e) {
            // NOTE: don't try to use 'Error.captureStackTrace' or transfer the
            // accessor around; that causes memory leaks as per GH-111. Just
            // reify the stack trace as a string ASAP.
            //
            // At the same time, cut off the first line; it's always just
            // "[object Promise]\n", as per the 'toString'.
            promise.stack = e.stack.substring(e.stack.indexOf("\n") + 1);
        }
    }

    // NOTE: we do the checks for 'resolvedPromise' in each method, instead of
    // consolidating them into 'become', since otherwise we'd create new
    // promises with the lines 'become(whatever(value))'. See e.g. GH-252.

    function become(newPromise) {
        resolvedPromise = newPromise;
        promise.source = newPromise;

        array_reduce(messages, function (undefined, message) {
            nextTick(function () {
                newPromise.promiseDispatch.apply(newPromise, message);
            });
        }, void 0);

        messages = void 0;
        progressListeners = void 0;
    }

    deferred.promise = promise;
    deferred.resolve = function (value) {
        if (resolvedPromise) {
            return;
        }

        become(Q(value));
    };

    deferred.fulfill = function (value) {
        if (resolvedPromise) {
            return;
        }

        become(fulfill(value));
    };
    deferred.reject = function (reason) {
        if (resolvedPromise) {
            return;
        }

        become(reject(reason));
    };
    deferred.notify = function (progress) {
        if (resolvedPromise) {
            return;
        }

        array_reduce(progressListeners, function (undefined, progressListener) {
            nextTick(function () {
                progressListener(progress);
            });
        }, void 0);
    };

    return deferred;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise"></a>[function <span class="apidocSignatureSpan">thrift.</span>Q.makePromise (descriptor, fallback, inspect)](#apidoc.element.thrift.Q.makePromise)
- description and source-code
```javascript
function Promise(descriptor, fallback, inspect) {
    if (fallback === void 0) {
        fallback = function (op) {
            return reject(new Error(
                "Promise does not support operation: " + op
            ));
        };
    }
    if (inspect === void 0) {
        inspect = function () {
            return {state: "unknown"};
        };
    }

    var promise = object_create(Promise.prototype);

    promise.promiseDispatch = function (resolve, op, args) {
        var result;
        try {
            if (descriptor[op]) {
                result = descriptor[op].apply(promise, args);
            } else {
                result = fallback.call(promise, op, args);
            }
        } catch (exception) {
            result = reject(exception);
        }
        if (resolve) {
            resolve(result);
        }
    };

    promise.inspect = inspect;

    // XXX deprecated 'valueOf' and 'exception' support
    if (inspect) {
        var inspected = inspect();
        if (inspected.state === "rejected") {
            promise.exception = inspected.reason;
        }

        promise.valueOf = function () {
            var inspected = inspect();
            if (inspected.state === "pending" ||
                inspected.state === "rejected") {
                return promise;
            }
            return inspected.value;
        };
    }

    return promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol"></a>[function <span class="apidocSignatureSpan">thrift.</span>TBinaryProtocol (trans, strictRead, strictWrite)](#apidoc.element.thrift.TBinaryProtocol)
- description and source-code
```javascript
function TBinaryProtocol(trans, strictRead, strictWrite) {
  this.trans = trans;
  this.strictRead = (strictRead !== undefined ? strictRead : false);
  this.strictWrite = (strictWrite !== undefined ? strictWrite : true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport"></a>[function <span class="apidocSignatureSpan">thrift.</span>TBufferedTransport (buffer, callback)](#apidoc.element.thrift.TBufferedTransport)
- description and source-code
```javascript
function TBufferedTransport(buffer, callback) {
  this.defaultReadBufferSize = 1024;
  this.writeBufferSize = 512; // Soft Limit
  this.inBuf = new Buffer(this.defaultReadBufferSize);
  this.readCursor = 0;
  this.writeCursor = 0; // for input buffer
  this.outBuffers = [];
  this.outCount = 0;
  this.onFlush = callback;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol"></a>[function <span class="apidocSignatureSpan">thrift.</span>TCompactProtocol (trans)](#apidoc.element.thrift.TCompactProtocol)
- description and source-code
```javascript
function TCompactProtocol(trans) {
  this.trans = trans;
  this.lastField_ = [];
  this.lastFieldId_ = 0;
  this.string_limit_ = 0;
  this.string_buf_ = null;
  this.string_buf_size_ = 0;
  this.container_limit_ = 0;
  this.booleanField_ = {
    name: null,
    hasBoolValue: false
  };
  this.boolValue_ = {
    hasBoolValue: false,
    boolValue: false
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport"></a>[function <span class="apidocSignatureSpan">thrift.</span>TFramedTransport (buffer, callback)](#apidoc.element.thrift.TFramedTransport)
- description and source-code
```javascript
function TFramedTransport(buffer, callback) {
  this.inBuf = buffer || new Buffer(0);
  this.outBuffers = [];
  this.outCount = 0;
  this.readPos = 0;
  this.onFlush = callback;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol"></a>[function <span class="apidocSignatureSpan">thrift.</span>TJSONProtocol (trans)](#apidoc.element.thrift.TJSONProtocol)
- description and source-code
```javascript
function TJSONProtocol(trans) {
  this.tstack = [];
  this.tpos = [];
  this.trans = trans;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.TApplicationException"></a>[function <span class="apidocSignatureSpan">thrift.</span>Thrift.TApplicationException (type, message)](#apidoc.element.thrift.Thrift.TApplicationException)
- description and source-code
```javascript
function TApplicationException(type, message) {
  TException.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.type = type || TApplicationExceptionType.UNKNOWN;
  this.name = this.constructor.name;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.TException"></a>[function <span class="apidocSignatureSpan">thrift.</span>Thrift.TException (message)](#apidoc.element.thrift.Thrift.TException)
- description and source-code
```javascript
function TException(message) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.TProtocolException"></a>[function <span class="apidocSignatureSpan">thrift.</span>Thrift.TProtocolException (type, message)](#apidoc.element.thrift.Thrift.TProtocolException)
- description and source-code
```javascript
function TProtocolException(type, message) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.type = type;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>WSConnection (host, port, options)](#apidoc.element.thrift.WSConnection)
- description and source-code
```javascript
function WSConnection(host, port, options) {
  //Initialize the emitter base object
  EventEmitter.call(this);

  //Set configuration
  var self = this;
  this.options = options || {};
  this.host = host;
  this.port = port;
  this.secure = this.options.secure || false;
  this.transport = this.options.transport || TBufferedTransport;
  this.protocol = this.options.protocol || TJSONProtocol;
  this.path = this.options.path;
  this.send_pending = [];

  //The sequence map is used to map seqIDs back to the
  //  calling client in multiplexed scenarios
  this.seqId2Service = {};

  //Prepare WebSocket options
  this.wsOptions = {
    host: this.host,
    port: this.port || 80,
    path: this.options.path || '/',
    headers: this.options.headers || {}
  };
  for (var attrname in this.options.wsOptions) {
    this.wsOptions[attrname] = this.options.wsOptions[attrname];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>XHRConnection (host, port, options)](#apidoc.element.thrift.XHRConnection)
- description and source-code
```javascript
function XHRConnection(host, port, options) {
  this.options = options || {};
  this.wpos = 0;
  this.rpos = 0;
  this.useCORS = (options && options.useCORS);
  this.send_buf = '';
  this.recv_buf = '';
  this.transport = options.transport || TBufferedTransport;
  this.protocol = options.protocol || TJSONProtocol;
  this.headers = options.headers || {};

  host = host || window.location.host;
  port = port || window.location.port;
  var prefix = options.https ? 'https://' : 'http://';
  var path = options.path || '/';

  if (port === '') {
    port = undefined;
  }

  if (!port || port === 80 || port === '80') {
    this.url = prefix + host + path;
  } else {
    this.url = prefix + host + ':' + port + path;
  }

  //The sequence map is used to map seqIDs back to the
  //  calling client in multiplexed scenarios
  this.seqId2Service = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createClient"></a>[function <span class="apidocSignatureSpan">thrift.</span>createClient (ServiceClient, connection)](#apidoc.element.thrift.createClient)
- description and source-code
```javascript
function createClient(ServiceClient, connection) {
  // TODO validate required options and throw otherwise
  if (ServiceClient.Client) {
    ServiceClient = ServiceClient.Client;
  }
  // TODO detangle these initialization calls
  // creating "client" requires
  //   - new service client instance
  //
  // New service client instance requires
  //   - new transport instance
  //   - protocol class reference
  //
  // New transport instance requires
  //   - Buffer to use (or none)
  //   - Callback to call on flush

  // Wrap the write method
  var writeCb = function(buf, seqid) {
    connection.write(buf, seqid);
  };
  var transport = new connection.transport(undefined, writeCb);
  var client = new ServiceClient(transport, connection.protocol);
  transport.client = client;
  connection.client = client;
  return client;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>createConnection (host, port, options)](#apidoc.element.thrift.createConnection)
- description and source-code
```javascript
createConnection = function (host, port, options) {
  var stream = net.createConnection(port, host);
  var connection = new Connection(stream, options);
  connection.host = host;
  connection.port = port;

  return connection;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createHttpClient"></a>[function <span class="apidocSignatureSpan">thrift.</span>createHttpClient (ServiceClient, connection)](#apidoc.element.thrift.createHttpClient)
- description and source-code
```javascript
function createClient(ServiceClient, connection) {
  // TODO validate required options and throw otherwise
  if (ServiceClient.Client) {
    ServiceClient = ServiceClient.Client;
  }
  // TODO detangle these initialization calls
  // creating "client" requires
  //   - new service client instance
  //
  // New service client instance requires
  //   - new transport instance
  //   - protocol class reference
  //
  // New transport instance requires
  //   - Buffer to use (or none)
  //   - Callback to call on flush

  // Wrap the write method
  var writeCb = function(buf, seqid) {
    connection.write(buf, seqid);
  };
  var transport = new connection.transport(undefined, writeCb);
  var client = new ServiceClient(transport, connection.protocol);
  transport.client = client;
  connection.client = client;
  return client;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createHttpConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>createHttpConnection (host, port, options)](#apidoc.element.thrift.createHttpConnection)
- description and source-code
```javascript
createHttpConnection = function (host, port, options) {
  return new HttpConnection(host, port, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createMultiplexServer"></a>[function <span class="apidocSignatureSpan">thrift.</span>createMultiplexServer (processor, options)](#apidoc.element.thrift.createMultiplexServer)
- description and source-code
```javascript
createMultiplexServer = function (processor, options) {
  var transport = (options && options.transport) ? options.transport : TBufferedTransport;
  var protocol = (options && options.protocol) ? options.protocol : TBinaryProtocol;

  function serverImpl(stream) {
    var self = this;
    stream.on('error', function(err) {
        self.emit('error', err);
    });
    stream.on('data', transport.receiver(function(transportWithData) {
      var input = new protocol(transportWithData);
      var output = new protocol(new transport(undefined, function(buf) {
        try {
            stream.write(buf);
        } catch (err) {
            self.emit('error', err);
            stream.end();
        }
      }));

      try {
        do {
          processor.process(input, output);
          transportWithData.commitPosition();
        } while (true);
      } catch (err) {
        if (err instanceof InputBufferUnderrunError) {
          //The last data in the buffer was not a complete message, wait for the rest
          transportWithData.rollbackPosition();
        }
        else if (err.message === "Invalid type: undefined") {
          //No more data in the buffer
          //This trap is a bit hackish
          //The next step to improve the node behavior here is to have
          //  the compiler generated process method throw a more explicit
          //  error when the network buffer is empty (regardles of the
          //  protocol/transport stack in use) and replace this heuristic.
          //  Also transports should probably not force upper layers to
          //  manage their buffer positions (i.e. rollbackPosition() and
          //  commitPosition() should be eliminated in lieu of a transport
          //  encapsulated buffer management strategy.)
          transportWithData.rollbackPosition();
        }
        else {
          //Unexpected error
          self.emit('error', err);
          stream.end();
        }
      }
    }));

    stream.on('end', function() {
      stream.end();
    });
  }

  if (options && options.tls) {
    return tls.createServer(options.tls, serverImpl);
  } else {
    return net.createServer(serverImpl);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createSSLConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>createSSLConnection (host, port, options)](#apidoc.element.thrift.createSSLConnection)
- description and source-code
```javascript
createSSLConnection = function (host, port, options) {
  var stream = tls.connect(port, host, options);
  var connection = new Connection(stream, options);
  connection.host = host;
  connection.port = port;

  return connection;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createServer"></a>[function <span class="apidocSignatureSpan">thrift.</span>createServer (processor, handler, options)](#apidoc.element.thrift.createServer)
- description and source-code
```javascript
createServer = function (processor, handler, options) {
  if (processor.Processor) {
    processor = processor.Processor;
  }
  return exports.createMultiplexServer(new processor(handler), options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createStdIOClient"></a>[function <span class="apidocSignatureSpan">thrift.</span>createStdIOClient (ServiceClient, connection)](#apidoc.element.thrift.createStdIOClient)
- description and source-code
```javascript
function createClient(ServiceClient, connection) {
  // TODO validate required options and throw otherwise
  if (ServiceClient.Client) {
    ServiceClient = ServiceClient.Client;
  }
  // TODO detangle these initialization calls
  // creating "client" requires
  //   - new service client instance
  //
  // New service client instance requires
  //   - new transport instance
  //   - protocol class reference
  //
  // New transport instance requires
  //   - Buffer to use (or none)
  //   - Callback to call on flush

  // Wrap the write method
  var writeCb = function(buf, seqid) {
    connection.write(buf, seqid);
  };
  var transport = new connection.transport(undefined, writeCb);
  var client = new ServiceClient(transport, connection.protocol);
  transport.client = client;
  connection.client = client;
  return client;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createStdIOConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>createStdIOConnection (command, options)](#apidoc.element.thrift.createStdIOConnection)
- description and source-code
```javascript
createStdIOConnection = function (command, options){
  return new StdIOConnection(command,options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createWSClient"></a>[function <span class="apidocSignatureSpan">thrift.</span>createWSClient (ServiceClient, connection)](#apidoc.element.thrift.createWSClient)
- description and source-code
```javascript
function createClient(ServiceClient, connection) {
  // TODO validate required options and throw otherwise
  if (ServiceClient.Client) {
    ServiceClient = ServiceClient.Client;
  }
  // TODO detangle these initialization calls
  // creating "client" requires
  //   - new service client instance
  //
  // New service client instance requires
  //   - new transport instance
  //   - protocol class reference
  //
  // New transport instance requires
  //   - Buffer to use (or none)
  //   - Callback to call on flush

  // Wrap the write method
  var writeCb = function(buf, seqid) {
    connection.write(buf, seqid);
  };
  var transport = new connection.transport(undefined, writeCb);
  var client = new ServiceClient(transport, connection.protocol);
  transport.client = client;
  connection.client = client;
  return client;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createWSConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>createWSConnection (host, port, options)](#apidoc.element.thrift.createWSConnection)
- description and source-code
```javascript
createWSConnection = function (host, port, options) {
  return new WSConnection(host, port, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createWebServer"></a>[function <span class="apidocSignatureSpan">thrift.</span>createWebServer (options)](#apidoc.element.thrift.createWebServer)
- description and source-code
```javascript
createWebServer = function (options) {
  var baseDir = options.files;
  var contentTypesByExtension = {
    '.txt': 'text/plain',
    '.html': 'text/html',
    '.css': 'text/css',
    '.xml': 'application/xml',
    '.json': 'application/json',
    '.js': 'application/javascript',
    '.jpg': 'image/jpeg',
    '.jpeg': 'image/jpeg',
    '.gif': 'image/gif',
    '.png': 'image/png',
    '.svg': 'image/svg+xml'
  };

  //Setup all of the services
  var services = options.services;
  for (var uri in services) {
    var svcObj = services[uri];

    //Setup the processor
    if (svcObj.processor instanceof MultiplexedProcessor) {
      //Multiplex processors have pre embedded processor/handler pairs, save as is
      svcObj.processor = svcObj.processor;
    } else {
      //For historical reasons Node.js supports processors passed in directly or via the
      //  IDL Compiler generated class housing the processor. Also, the options property
      //  for a Processor has been called both cls and processor at different times. We
      //  support any of the four possibilities here.
      var processor = (svcObj.processor) ? (svcObj.processor.Processor || svcObj.processor) :
                                           (svcObj.cls.Processor || svcObj.cls);
      //Processors can be supplied as constructed objects with handlers already embedded,
      //  if a handler is provided we construct a new processor, if not we use the processor
      //  object directly
      if (svcObj.handler) {
        svcObj.processor = new processor(svcObj.handler);
      } else {
        svcObj.processor = processor;
      }
    }
    svcObj.transport = svcObj.transport ? svcObj.transport : TBufferedTransport;
    svcObj.protocol = svcObj.protocol ? svcObj.protocol : TBinaryProtocol;
  }

  //Verify CORS requirements
  function VerifyCORSAndSetHeaders(request, response) {
    if (request.headers.origin && options.cors) {
      if (options.cors["*"] || options.cors[request.headers.origin]) {
        //Allow, origin allowed
        response.setHeader("access-control-allow-origin", request.headers.origin);
        response.setHeader("access-control-allow-methods", "GET, POST, OPTIONS");
        response.setHeader("access-control-allow-headers", "content-type, accept");
        response.setHeader("access-control-max-age", "60");
        return true;
      } else {
        //Disallow, origin denied
        return false;
      }
    }
    //Allow, CORS is not in use
    return true;
  }


  //Handle OPTIONS method (CORS)
  ///////////////////////////////////////////////////
  function processOptions(request, response) {
    if (VerifyCORSAndSetHeaders(request, response)) {
      response.writeHead("204", "No Content", {"content-length": 0});
    } else {
      response.writeHead("403", "Origin " + request.headers.origin + " not allowed", {});
    }
    response.end();
  }


  //Handle POST methods (TXHRTransport)
  ///////////////////////////////////////////////////
  function processPost(request, response) {
    //Lookup service
    var uri = url.parse(request.url).pathname;
    var svc = services[uri];
    if (!svc) {
      response.writeHead("403", "No Apache Thrift Service at " + uri, {});
      response.end();
      return;
    }

    //Verify CORS requirements
    if (!VerifyCORSAndSetHeaders(request, response)) {
      response.writeHead("403", "Origin " + request.headers.origin + " not allowed", {});
      response.end();
      return;
    }

    //Process XHR payload
    request.on('data', svc.transport.receiver(function(transportWithData) {
      var input = new svc.protocol(transportWithData);
      var output = new svc.protocol(new svc.transport(undefined, function(buf) {
        try {
          response.writeHead(200);
          response.end(buf);
        } catch (err) {
          response.writeHead(500);
          response.end();
        }
      }));

      try {
        svc.processor.process(input, output);
        transportWithData.commitPosition();
      } catch (err) {
        if (err instanceof InputBufferUnderrunError) {
          transportWithData.rollba ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createXHRClient"></a>[function <span class="apidocSignatureSpan">thrift.</span>createXHRClient (ServiceClient, connection)](#apidoc.element.thrift.createXHRClient)
- description and source-code
```javascript
function createClient(ServiceClient, connection) {
  // TODO validate required options and throw otherwise
  if (ServiceClient.Client) {
    ServiceClient = ServiceClient.Client;
  }
  // TODO detangle these initialization calls
  // creating "client" requires
  //   - new service client instance
  //
  // New service client instance requires
  //   - new transport instance
  //   - protocol class reference
  //
  // New transport instance requires
  //   - Buffer to use (or none)
  //   - Callback to call on flush

  // Wrap the write method
  var writeCb = function(buf, seqid) {
    connection.write(buf, seqid);
  };
  var transport = new connection.transport(undefined, writeCb);
  var client = new ServiceClient(transport, connection.protocol);
  transport.client = client;
  connection.client = client;
  return client;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.createXHRConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>createXHRConnection (host, port, options)](#apidoc.element.thrift.createXHRConnection)
- description and source-code
```javascript
createXHRConnection = function (host, port, options) {
  return new XHRConnection(host, port, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Connection"></a>[module thrift.Connection](#apidoc.module.thrift.Connection)

#### <a name="apidoc.element.thrift.Connection.Connection"></a>[function <span class="apidocSignatureSpan">thrift.</span>Connection (stream, options)](#apidoc.element.thrift.Connection.Connection)
- description and source-code
```javascript
Connection = function (stream, options) {
  var self = this;
  EventEmitter.call(this);

  this.seqId2Service = {};
  this.connection = stream;
  this.ssl = (stream.encrypted);
  this.options = options || {};
  this.transport = this.options.transport || TBufferedTransport;
  this.protocol = this.options.protocol || TBinaryProtocol;
  this.offline_queue = [];
  this.connected = false;
  this.initialize_retry_vars();

  this._debug = this.options.debug || false;
  if (this.options.max_attempts &&
      !isNaN(this.options.max_attempts) &&
      this.options.max_attempts > 0) {
     this.max_attempts = +this.options.max_attempts;
  }
  this.retry_max_delay = null;
  if (this.options.retry_max_delay !== undefined &&
      !isNaN(this.options.retry_max_delay) &&
      this.options.retry_max_delay > 0) {
     this.retry_max_delay = this.options.retry_max_delay;
  }
  this.connect_timeout = false;
  if (this.options.connect_timeout &&
      !isNaN(this.options.connect_timeout) &&
      this.options.connect_timeout > 0) {
     this.connect_timeout = +this.options.connect_timeout;
  }

  this.connection.addListener(this.ssl ? "secureConnect" : "connect", function() {
    self.connected = true;

    this.setTimeout(self.options.timeout || 0);
    this.setNoDelay();
    this.frameLeft = 0;
    this.framePos = 0;
    this.frame = null;
    self.initialize_retry_vars();

    self.offline_queue.forEach(function(data) {
      self.connection.write(data);
    });

    self.emit("connect");
  });

  this.connection.addListener("error", function(err) {
    // Only emit the error if no-one else is listening on the connection
    // or if someone is listening on us, because Node turns unhandled
    // 'error' events into exceptions.
    if (self.connection.listeners('error').length === 1 ||
        self.listeners('error').length > 0) {
      self.emit("error", err);
    }
  });

  // Add a close listener
  this.connection.addListener("close", function() {
    self.connection_gone(); // handle close event. try to reconnect
  });

  this.connection.addListener("timeout", function() {
    self.emit("timeout");
  });

  this.connection.addListener("data", self.transport.receiver(function(transport_with_data) {
    var message = new self.protocol(transport_with_data);
    try {
      while (true) {
        var header = message.readMessageBegin();
        var dummy_seqid = header.rseqid * -1;
        var client = self.client;
        //The Multiplexed Protocol stores a hash of seqid to service names
        //  in seqId2Service. If the SeqId is found in the hash we need to
        //  lookup the appropriate client for this call.
        //  The connection.client object is a single client object when not
        //  multiplexing, when using multiplexing it is a service name keyed
        //  hash of client objects.
        //NOTE: The 2 way interdependencies between protocols, transports,
        //  connections and clients in the Node.js implementation are irregular
        //  and make the implementation difficult to extend and maintain. We
        //  should bring this stuff inline with typical thrift I/O stack
        //  operation soon.
        //  --ra
        var service_name = self.seqId2Service[header.rseqid];
        if (service_name) {
          client = self.client[service_name];
          delete self.seqId2Service[header.rseqid];
        }
<span class="apidocCodeCommentSpan">        /*jshint -W083 */
</span>        client._reqs[dummy_seqid] = function(err, success){
          transport_with_data.commitPosition();

          var callback = client._reqs[header.rseqid];
          delete client._reqs[header.rseqid];
          if (callback) {
            callback(err, success);
          }
        };
        /*jshint +W083 */

        if(client['recv_' + header.fname]) {
          client['recv_' + header.fname](message, header.mtype, dummy_seqid);
        } else {
          delete client._reqs[dummy_seqid];
          self.emit("error",
                    new thrift.TApplicationException(thrift.TApplicationExceptionType.WRONG_METHOD_NAME,
                             "Received a response to an ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Connection.super_"></a>[function <span class="apidocSignatureSpan">thrift.Connection.</span>super_ ()](#apidoc.element.thrift.Connection.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Connection.prototype"></a>[module thrift.Connection.prototype](#apidoc.module.thrift.Connection.prototype)

#### <a name="apidoc.element.thrift.Connection.prototype.connection_gone"></a>[function <span class="apidocSignatureSpan">thrift.Connection.prototype.</span>connection_gone ()](#apidoc.element.thrift.Connection.prototype.connection_gone)
- description and source-code
```javascript
connection_gone = function () {
  var self = this;
  this.connected = false;

  // If a retry is already in progress, just let that happen
  if (this.retry_timer) {
    return;
  }
  // We cannot reconnect a secure socket.
  if (!this.max_attempts || this.ssl) {
    self.emit("close");
    return;
  }

  if (this.retry_max_delay !== null && this.retry_delay >= this.retry_max_delay) {
    this.retry_delay = this.retry_max_delay;
  } else {
    this.retry_delay = Math.floor(this.retry_delay * this.retry_backoff);
  }

  if (self._debug) {
    console.log("Retry connection in " + this.retry_delay + " ms");
  }

  if (this.max_attempts && this.attempts >= this.max_attempts) {
    this.retry_timer = null;
    console.error("thrift: Couldn't get thrift connection after " + this.max_attempts + " attempts.");
    self.emit("close");
    return;
  }

  this.attempts += 1;
  this.emit("reconnecting", {
    delay: self.retry_delay,
    attempt: self.attempts
  });

  this.retry_timer = setTimeout(function () {
    if (self._debug) {
       console.log("Retrying connection...");
	}

    self.retry_totaltime += self.retry_delay;

    if (self.connect_timeout && self.retry_totaltime >= self.connect_timeout) {
       self.retry_timer = null;
       console.error("thrift: Couldn't get thrift connection after " + self.retry_totaltime + "ms.");
       self.emit("close");
       return;
    }

    self.connection.connect(self.port, self.host);
    self.retry_timer = null;
  }, this.retry_delay);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Connection.prototype.destroy"></a>[function <span class="apidocSignatureSpan">thrift.Connection.prototype.</span>destroy ()](#apidoc.element.thrift.Connection.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  this.connection.destroy();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Connection.prototype.end"></a>[function <span class="apidocSignatureSpan">thrift.Connection.prototype.</span>end ()](#apidoc.element.thrift.Connection.prototype.end)
- description and source-code
```javascript
end = function () {
  this.connection.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Connection.prototype.initialize_retry_vars"></a>[function <span class="apidocSignatureSpan">thrift.Connection.prototype.</span>initialize_retry_vars ()](#apidoc.element.thrift.Connection.prototype.initialize_retry_vars)
- description and source-code
```javascript
initialize_retry_vars = function () {
  this.retry_timer = null;
  this.retry_totaltime = 0;
  this.retry_delay = 150;
  this.retry_backoff = 1.7;
  this.attempts = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Connection.prototype.write"></a>[function <span class="apidocSignatureSpan">thrift.Connection.prototype.</span>write (data)](#apidoc.element.thrift.Connection.prototype.write)
- description and source-code
```javascript
write = function (data) {
  if (!this.connected) {
    this.offline_queue.push(data);
    return;
  }
  this.connection.write(data);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.HttpConnection"></a>[module thrift.HttpConnection](#apidoc.module.thrift.HttpConnection)

#### <a name="apidoc.element.thrift.HttpConnection.HttpConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>HttpConnection (host, port, options)](#apidoc.element.thrift.HttpConnection.HttpConnection)
- description and source-code
```javascript
HttpConnection = function (host, port, options) {
  //Initialize the emitter base object
  EventEmitter.call(this);

  //Set configuration
  var self = this;
  this.options = options || {};
  this.host = host;
  this.port = port;
  this.https = this.options.https || false;
  this.transport = this.options.transport || TBufferedTransport;
  this.protocol = this.options.protocol || TBinaryProtocol;

  //Prepare Node.js options
  this.nodeOptions = {
    host: this.host,
    port: this.port || 80,
    path: this.options.path || '/',
    method: 'POST',
    headers: this.options.headers || {},
    responseType: this.options.responseType || null
  };
  for (var attrname in this.options.nodeOptions) {
    this.nodeOptions[attrname] = this.options.nodeOptions[attrname];
  }
<span class="apidocCodeCommentSpan">  /*jshint -W069 */
</span>  if (! this.nodeOptions.headers['Connection']) {
    this.nodeOptions.headers['Connection'] = 'keep-alive';
  }
  /*jshint +W069 */

  //The sequence map is used to map seqIDs back to the
  //  calling client in multiplexed scenarios
  this.seqId2Service = {};

  function decodeCallback(transport_with_data) {
    var proto = new self.protocol(transport_with_data);
    try {
      while (true) {
        var header = proto.readMessageBegin();
        var dummy_seqid = header.rseqid * -1;
        var client = self.client;
        //The Multiplexed Protocol stores a hash of seqid to service names
        //  in seqId2Service. If the SeqId is found in the hash we need to
        //  lookup the appropriate client for this call.
        //  The client var is a single client object when not multiplexing,
        //  when using multiplexing it is a service name keyed hash of client
        //  objects.
        //NOTE: The 2 way interdependencies between protocols, transports,
        //  connections and clients in the Node.js implementation are irregular
        //  and make the implementation difficult to extend and maintain. We
        //  should bring this stuff inline with typical thrift I/O stack
        //  operation soon.
        //  --ra
        var service_name = self.seqId2Service[header.rseqid];
        if (service_name) {
          client = self.client[service_name];
          delete self.seqId2Service[header.rseqid];
        }
        /*jshint -W083 */
        client._reqs[dummy_seqid] = function(err, success){
          transport_with_data.commitPosition();
          var clientCallback = client._reqs[header.rseqid];
          delete client._reqs[header.rseqid];
          if (clientCallback) {
            process.nextTick(function() {
              clientCallback(err, success);
            });
          }
        };
        /*jshint +W083 */
        if(client['recv_' + header.fname]) {
          client['recv_' + header.fname](proto, header.mtype, dummy_seqid);
        } else {
          delete client._reqs[dummy_seqid];
          self.emit("error",
                    new thrift.TApplicationException(
                       thrift.TApplicationExceptionType.WRONG_METHOD_NAME,
                       "Received a response to an unknown RPC function"));
        }
      }
    }
    catch (e) {
      if (e instanceof InputBufferUnderrunError) {
        transport_with_data.rollbackPosition();
      } else {
        self.emit('error', e);
      }
    }
  }


  //Response handler
  //////////////////////////////////////////////////
  this.responseCallback = function(response) {
    var data = [];
    var dataLen = 0;

    response.on('error', function (e) {
      self.emit("error", e);
    });

    // When running directly under node, chunk will be a buffer,
    // however, when running in a Browser (e.g. Browserify), chunk
    // will be a string or an ArrayBuffer.
    response.on('data', function (chunk) {
      if ((typeof chunk == 'string') ||
          (Object.prototype.toString.call(chunk) == '[object Uint8Array]')) {
        // Wrap ArrayBuffer/string in a Buffer so data[i].copy will work
        data.push(new Buffer(chunk));
      } else {
        data.push(chunk);
      }
      dataLen += chunk.length;
    });

    response.on('end', function(){ ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.HttpConnection.super_"></a>[function <span class="apidocSignatureSpan">thrift.HttpConnection.</span>super_ ()](#apidoc.element.thrift.HttpConnection.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.HttpConnection.prototype"></a>[module thrift.HttpConnection.prototype](#apidoc.module.thrift.HttpConnection.prototype)

#### <a name="apidoc.element.thrift.HttpConnection.prototype.write"></a>[function <span class="apidocSignatureSpan">thrift.HttpConnection.prototype.</span>write (data)](#apidoc.element.thrift.HttpConnection.prototype.write)
- description and source-code
```javascript
write = function (data) {
  var self = this;
  self.nodeOptions.headers["Content-length"] = data.length;
  var req = (self.https) ?
      https.request(self.nodeOptions, self.responseCallback) :
      http.request(self.nodeOptions, self.responseCallback);
  req.on('error', function(err) {
    self.emit("error", err);
  });
  req.write(data);
  req.end();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Int64"></a>[module thrift.Int64](#apidoc.module.thrift.Int64)

#### <a name="apidoc.element.thrift.Int64.Int64"></a>[function <span class="apidocSignatureSpan">thrift.</span>Int64 (a1, a2)](#apidoc.element.thrift.Int64.Int64)
- description and source-code
```javascript
Int64 = function (a1, a2) {
  if (a1 instanceof Buffer) {
    this.buffer = a1;
    this.offset = a2 || 0;
  } else if (Object.prototype.toString.call(a1) == '[object Uint8Array]') {
    // Under Browserify, Buffers can extend Uint8Arrays rather than an
    // instance of Buffer. We could assume the passed in Uint8Array is actually
    // a buffer but that won't handle the case where a raw Uint8Array is passed
    // in. We construct a new Buffer just in case.
    this.buffer = new Buffer(a1);
    this.offset = a2 || 0;
  } else {
    this.buffer = this.buffer || new Buffer(8);
    this.offset = 0;
    this.setValue.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Int64.prototype"></a>[module thrift.Int64.prototype](#apidoc.module.thrift.Int64.prototype)

#### <a name="apidoc.element.thrift.Int64.prototype._2scomp"></a>[function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>_2scomp ()](#apidoc.element.thrift.Int64.prototype._2scomp)
- description and source-code
```javascript
_2scomp = function () {
  var b = this.buffer, o = this.offset, carry = 1;
  for (var i = o + 7; i >= o; i--) {
    var v = (b[i] ^ 0xff) + carry;
    b[i] = v & 0xff;
    carry = v >> 8;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Int64.prototype.copy"></a>[function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>copy (targetBuffer, targetOffset)](#apidoc.element.thrift.Int64.prototype.copy)
- description and source-code
```javascript
copy = function (targetBuffer, targetOffset) {
  this.buffer.copy(targetBuffer, targetOffset || 0, this.offset, this.offset + 8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Int64.prototype.inspect"></a>[function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>inspect ()](#apidoc.element.thrift.Int64.prototype.inspect)
- description and source-code
```javascript
inspect = function () {
  return '[Int64 value:' + this + ' octets:' + this.toOctetString(' ') + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Int64.prototype.setValue"></a>[function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>setValue (hi, lo)](#apidoc.element.thrift.Int64.prototype.setValue)
- description and source-code
```javascript
setValue = function (hi, lo) {
  var negate = false;
  if (arguments.length == 1) {
    if (typeof(hi) == 'number') {
      // Simplify bitfield retrieval by using abs() value.  We restore sign
      // later
      negate = hi < 0;
      hi = Math.abs(hi);
      lo = hi % VAL32;
      hi = hi / VAL32;
      if (hi > VAL32) throw new RangeError(hi  + ' is outside Int64 range');
      hi = hi | 0;
    } else if (typeof(hi) == 'string') {
      hi = (hi + '').replace(/^0x/, '');
      lo = hi.substr(-8);
      hi = hi.length > 8 ? hi.substr(0, hi.length - 8) : '';
      hi = parseInt(hi, 16);
      lo = parseInt(lo, 16);
    } else {
      throw new Error(hi + ' must be a Number or String');
    }
  }

  // Technically we should throw if hi or lo is outside int32 range here, but
  // it's not worth the effort. Anything past the 32'nd bit is ignored.

  // Copy bytes to buffer
  var b = this.buffer, o = this.offset;
  for (var i = 7; i >= 0; i--) {
    b[o+i] = lo & 0xff;
    lo = i == 4 ? hi : lo >>> 8;
  }

  // Restore sign of passed argument
  if (negate) this._2scomp();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Int64.prototype.toBuffer"></a>[function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>toBuffer (rawBuffer)](#apidoc.element.thrift.Int64.prototype.toBuffer)
- description and source-code
```javascript
toBuffer = function (rawBuffer) {
  if (rawBuffer && this.offset === 0) return this.buffer;

  var out = new Buffer(8);
  this.buffer.copy(out, 0, this.offset, this.offset + 8);
  return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Int64.prototype.toNumber"></a>[function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>toNumber (allowImprecise)](#apidoc.element.thrift.Int64.prototype.toNumber)
- description and source-code
```javascript
toNumber = function (allowImprecise) {
  var b = this.buffer, o = this.offset;

  // Running sum of octets, doing a 2's complement
  var negate = b[o] & 0x80, x = 0, carry = 1;
  for (var i = 7, m = 1; i >= 0; i--, m *= 256) {
    var v = b[o+i];

    // 2's complement for negative numbers
    if (negate) {
      v = (v ^ 0xff) + carry;
      carry = v >> 8;
      v = v & 0xff;
    }

    x += v * m;
  }

  // Return Infinity if we've lost integer precision
  if (!allowImprecise && x >= Int64.MAX_INT) {
    return negate ? -Infinity : Infinity;
  }

  return negate ? -x : x;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Int64.prototype.toOctetString"></a>[function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>toOctetString (sep)](#apidoc.element.thrift.Int64.prototype.toOctetString)
- description and source-code
```javascript
toOctetString = function (sep) {
  var out = new Array(8);
  var b = this.buffer, o = this.offset;
  for (var i = 0; i < 8; i++) {
    out[i] = _HEX[b[o+i]];
  }
  return out.join(sep || '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Int64.prototype.toString"></a>[function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>toString (radix)](#apidoc.element.thrift.Int64.prototype.toString)
- description and source-code
```javascript
toString = function (radix) {
  return this.valueOf().toString(radix || 10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Int64.prototype.valueOf"></a>[function <span class="apidocSignatureSpan">thrift.Int64.prototype.</span>valueOf ()](#apidoc.element.thrift.Int64.prototype.valueOf)
- description and source-code
```javascript
valueOf = function () {
  return this.toNumber(false);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.MultiplexedProcessor"></a>[module thrift.MultiplexedProcessor](#apidoc.module.thrift.MultiplexedProcessor)

#### <a name="apidoc.element.thrift.MultiplexedProcessor.MultiplexedProcessor"></a>[function <span class="apidocSignatureSpan">thrift.</span>MultiplexedProcessor (stream, options)](#apidoc.element.thrift.MultiplexedProcessor.MultiplexedProcessor)
- description and source-code
```javascript
function MultiplexedProcessor(stream, options) {
  this.services = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.MultiplexedProcessor.prototype"></a>[module thrift.MultiplexedProcessor.prototype](#apidoc.module.thrift.MultiplexedProcessor.prototype)

#### <a name="apidoc.element.thrift.MultiplexedProcessor.prototype.process"></a>[function <span class="apidocSignatureSpan">thrift.MultiplexedProcessor.prototype.</span>process (inp, out)](#apidoc.element.thrift.MultiplexedProcessor.prototype.process)
- description and source-code
```javascript
process = function (inp, out) {
  var begin = inp.readMessageBegin();

  if (begin.mtype != Thrift.MessageType.CALL && begin.mtype != Thrift.MessageType.ONEWAY) {
    throw new Thrift.TException('TMultiplexedProcessor: Unexpected message type');
  }

  var p = begin.fname.split(':');
  var sname = p[0];
  var fname = p[1];

  if (! (sname in this.services)) {
    throw new Thrift.TException('TMultiplexedProcessor: Unknown service: ' + sname);
  }

  //construct a proxy object which stubs the readMessageBegin
  //for the service
  var inpProxy = {};

  for (var attr in inp) {
    inpProxy[attr] = inp[attr];
  }

  inpProxy.readMessageBegin = function() {
    return {
      fname: fname,
      mtype: begin.mtype,
      rseqid: begin.rseqid
    };
  };

  this.services[sname].process(inpProxy, out);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.MultiplexedProcessor.prototype.registerProcessor"></a>[function <span class="apidocSignatureSpan">thrift.MultiplexedProcessor.prototype.</span>registerProcessor (name, handler)](#apidoc.element.thrift.MultiplexedProcessor.prototype.registerProcessor)
- description and source-code
```javascript
registerProcessor = function (name, handler) {
  this.services[name] = handler;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Multiplexer"></a>[module thrift.Multiplexer](#apidoc.module.thrift.Multiplexer)

#### <a name="apidoc.element.thrift.Multiplexer.Multiplexer"></a>[function <span class="apidocSignatureSpan">thrift.</span>Multiplexer ()](#apidoc.element.thrift.Multiplexer.Multiplexer)
- description and source-code
```javascript
function Multiplexer() {
  this.seqid = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Multiplexer.prototype"></a>[module thrift.Multiplexer.prototype](#apidoc.module.thrift.Multiplexer.prototype)

#### <a name="apidoc.element.thrift.Multiplexer.prototype.createClient"></a>[function <span class="apidocSignatureSpan">thrift.Multiplexer.prototype.</span>createClient (serviceName, ServiceClient, connection)](#apidoc.element.thrift.Multiplexer.prototype.createClient)
- description and source-code
```javascript
createClient = function (serviceName, ServiceClient, connection) {
  if (ServiceClient.Client) {
    ServiceClient = ServiceClient.Client;
  }
  var self = this;
  ServiceClient.prototype.new_seqid = function() {
    self.seqid += 1;
    return self.seqid;
  };
  var writeCb = function(buf, seqid) {
    connection.write(buf,seqid);
  };
  var transport = new connection.transport(undefined, writeCb);
  var protocolWrapper = new Wrapper(serviceName, connection.protocol, connection);
  var client = new ServiceClient(transport, protocolWrapper);

  if (typeof connection.client !== 'object') {
    connection.client = {};
  }
  connection.client[serviceName] = client;

  return client;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Q"></a>[module thrift.Q](#apidoc.module.thrift.Q)

#### <a name="apidoc.element.thrift.Q.Q"></a>[function <span class="apidocSignatureSpan">thrift.</span>Q (value)](#apidoc.element.thrift.Q.Q)
- description and source-code
```javascript
function Q(value) {
    // If the object is already a Promise, return it directly.  This enables
    // the resolve function to both be used to created references from objects,
    // but to tolerably coerce non-promises to promises.
    if (isPromise(value)) {
        return value;
    }

    // assimilate thenables
    if (isPromiseAlike(value)) {
        return coerce(value);
    } else {
        return fulfill(value);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.Promise"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>Promise (resolver)](#apidoc.element.thrift.Q.Promise)
- description and source-code
```javascript
function promise(resolver) {
    if (typeof resolver !== "function") {
        throw new TypeError("resolver must be a function.");
    }
    var deferred = defer();
    try {
        resolver(deferred.resolve, deferred.reject, deferred.notify);
    } catch (reason) {
        deferred.reject(reason);
    }
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.all"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>all (promises)](#apidoc.element.thrift.Q.all)
- description and source-code
```javascript
function all(promises) {
    return when(promises, function (promises) {
        var countDown = 0;
        var deferred = defer();
        array_reduce(promises, function (undefined, promise, index) {
            var snapshot;
            if (
                isPromise(promise) &&
                (snapshot = promise.inspect()).state === "fulfilled"
            ) {
                promises[index] = snapshot.value;
            } else {
                ++countDown;
                when(
                    promise,
                    function (value) {
                        promises[index] = value;
                        if (--countDown === 0) {
                            deferred.resolve(promises);
                        }
                    },
                    deferred.reject,
                    function (progress) {
                        deferred.notify({ index: index, value: progress });
                    }
                );
            }
        }, void 0);
        if (countDown === 0) {
            deferred.resolve(promises);
        }
        return deferred.promise;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.allResolved"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>allResolved ()](#apidoc.element.thrift.Q.allResolved)
- description and source-code
```javascript
allResolved = function () {
    if (typeof console !== "undefined" &&
        typeof console.warn === "function") {
        console.warn(name + " is deprecated, use " + alternative +
                     " instead.", new Error("").stack);
    }
    return callback.apply(callback, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.allSettled"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>allSettled (promises)](#apidoc.element.thrift.Q.allSettled)
- description and source-code
```javascript
function allSettled(promises) {
    return Q(promises).allSettled();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.async"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>async (makeGenerator)](#apidoc.element.thrift.Q.async)
- description and source-code
```javascript
function async(makeGenerator) {
    return function () {
        // when verb is "send", arg is a value
        // when verb is "throw", arg is an exception
        function continuer(verb, arg) {
            var result;

            // Until V8 3.19 / Chromium 29 is released, SpiderMonkey is the only
            // engine that has a deployed base of browsers that support generators.
            // However, SM's generators use the Python-inspired semantics of
            // outdated ES6 drafts.  We would like to support ES6, but we'd also
            // like to make it possible to use generators in deployed browsers, so
            // we also support Python-style generators.  At some point we can remove
            // this block.

            if (typeof StopIteration === "undefined") {
                // ES6 Generators
                try {
                    result = generator[verb](arg);
                } catch (exception) {
                    return reject(exception);
                }
                if (result.done) {
                    return result.value;
                } else {
                    return when(result.value, callback, errback);
                }
            } else {
                // SpiderMonkey Generators
                // FIXME: Remove this case when SM does ES6 generators.
                try {
                    result = generator[verb](arg);
                } catch (exception) {
                    if (isStopIteration(exception)) {
                        return exception.value;
                    } else {
                        return reject(exception);
                    }
                }
                return when(result, callback, errback);
            }
        }
        var generator = makeGenerator.apply(this, arguments);
        var callback = continuer.bind(continuer, "next");
        var errback = continuer.bind(continuer, "throw");
        return callback();
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.catch"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>catch (object, rejected)](#apidoc.element.thrift.Q.catch)
- description and source-code
```javascript
catch = function (object, rejected) {
    return Q(object).then(void 0, rejected);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.defer"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>defer ()](#apidoc.element.thrift.Q.defer)
- description and source-code
```javascript
function defer() {
    // if "messages" is an "Array", that indicates that the promise has not yet
    // been resolved.  If it is "undefined", it has been resolved.  Each
    // element of the messages array is itself an array of complete arguments to
    // forward to the resolved promise.  We coerce the resolution value to a
    // promise using the 'resolve' function because it handles both fully
    // non-thenable values and other thenables gracefully.
    var messages = [], progressListeners = [], resolvedPromise;

    var deferred = object_create(defer.prototype);
    var promise = object_create(Promise.prototype);

    promise.promiseDispatch = function (resolve, op, operands) {
        var args = array_slice(arguments);
        if (messages) {
            messages.push(args);
            if (op === "when" && operands[1]) { // progress operand
                progressListeners.push(operands[1]);
            }
        } else {
            nextTick(function () {
                resolvedPromise.promiseDispatch.apply(resolvedPromise, args);
            });
        }
    };

    // XXX deprecated
    promise.valueOf = function () {
        if (messages) {
            return promise;
        }
        var nearerValue = nearer(resolvedPromise);
        if (isPromise(nearerValue)) {
            resolvedPromise = nearerValue; // shorten chain
        }
        return nearerValue;
    };

    promise.inspect = function () {
        if (!resolvedPromise) {
            return { state: "pending" };
        }
        return resolvedPromise.inspect();
    };

    if (Q.longStackSupport && hasStacks) {
        try {
            throw new Error();
        } catch (e) {
            // NOTE: don't try to use 'Error.captureStackTrace' or transfer the
            // accessor around; that causes memory leaks as per GH-111. Just
            // reify the stack trace as a string ASAP.
            //
            // At the same time, cut off the first line; it's always just
            // "[object Promise]\n", as per the 'toString'.
            promise.stack = e.stack.substring(e.stack.indexOf("\n") + 1);
        }
    }

    // NOTE: we do the checks for 'resolvedPromise' in each method, instead of
    // consolidating them into 'become', since otherwise we'd create new
    // promises with the lines 'become(whatever(value))'. See e.g. GH-252.

    function become(newPromise) {
        resolvedPromise = newPromise;
        promise.source = newPromise;

        array_reduce(messages, function (undefined, message) {
            nextTick(function () {
                newPromise.promiseDispatch.apply(newPromise, message);
            });
        }, void 0);

        messages = void 0;
        progressListeners = void 0;
    }

    deferred.promise = promise;
    deferred.resolve = function (value) {
        if (resolvedPromise) {
            return;
        }

        become(Q(value));
    };

    deferred.fulfill = function (value) {
        if (resolvedPromise) {
            return;
        }

        become(fulfill(value));
    };
    deferred.reject = function (reason) {
        if (resolvedPromise) {
            return;
        }

        become(reject(reason));
    };
    deferred.notify = function (progress) {
        if (resolvedPromise) {
            return;
        }

        array_reduce(progressListeners, function (undefined, progressListener) {
            nextTick(function () {
                progressListener(progress);
            });
        }, void 0);
    };

    return deferred;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.del"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>del (object, key)](#apidoc.element.thrift.Q.del)
- description and source-code
```javascript
del = function (object, key) {
    return Q(object).dispatch("delete", [key]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.delay"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>delay (object, timeout)](#apidoc.element.thrift.Q.delay)
- description and source-code
```javascript
delay = function (object, timeout) {
    if (timeout === void 0) {
        timeout = object;
        object = void 0;
    }
    return Q(object).delay(timeout);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.delete"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>delete (object, key)](#apidoc.element.thrift.Q.delete)
- description and source-code
```javascript
delete = function (object, key) {
    return Q(object).dispatch("delete", [key]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.denodeify"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>denodeify (callback)](#apidoc.element.thrift.Q.denodeify)
- description and source-code
```javascript
denodeify = function (callback) {
    var baseArgs = array_slice(arguments, 1);
    return function () {
        var nodeArgs = baseArgs.concat(array_slice(arguments));
        var deferred = defer();
        nodeArgs.push(deferred.makeNodeResolver());
        Q(callback).fapply(nodeArgs).fail(deferred.reject);
        return deferred.promise;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.dispatch"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>dispatch (object, op, args)](#apidoc.element.thrift.Q.dispatch)
- description and source-code
```javascript
function dispatch(object, op, args) {
    return Q(object).dispatch(op, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.done"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>done (object, fulfilled, rejected, progress)](#apidoc.element.thrift.Q.done)
- description and source-code
```javascript
done = function (object, fulfilled, rejected, progress) {
    return Q(object).done(fulfilled, rejected, progress);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.fail"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>fail (object, rejected)](#apidoc.element.thrift.Q.fail)
- description and source-code
```javascript
fail = function (object, rejected) {
    return Q(object).then(void 0, rejected);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.fapply"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>fapply (object, args)](#apidoc.element.thrift.Q.fapply)
- description and source-code
```javascript
fapply = function (object, args) {
    return Q(object).dispatch("apply", [void 0, args]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.fbind"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>fbind (object)](#apidoc.element.thrift.Q.fbind)
- description and source-code
```javascript
fbind = function (object) {
    var promise = Q(object);
    var args = array_slice(arguments, 1);
    return function fbound() {
        return promise.dispatch("apply", [
            this,
            args.concat(array_slice(arguments))
        ]);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.fcall"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>fcall (object)](#apidoc.element.thrift.Q.fcall)
- description and source-code
```javascript
fcall = function (object) {
    return Q(object).dispatch("apply", [void 0, array_slice(arguments, 1)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.fin"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>fin (object, callback)](#apidoc.element.thrift.Q.fin)
- description and source-code
```javascript
fin = function (object, callback) {
    return Q(object)["finally"](callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.finally"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>finally (object, callback)](#apidoc.element.thrift.Q.finally)
- description and source-code
```javascript
finally = function (object, callback) {
    return Q(object)["finally"](callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.fulfill"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>fulfill (value)](#apidoc.element.thrift.Q.fulfill)
- description and source-code
```javascript
function fulfill(value) {
    return Promise({
        "when": function () {
            return value;
        },
        "get": function (name) {
            return value[name];
        },
        "set": function (name, rhs) {
            value[name] = rhs;
        },
        "delete": function (name) {
            delete value[name];
        },
        "post": function (name, args) {
            // Mark Miller proposes that post with no name should apply a
            // promised function.
            if (name === null || name === void 0) {
                return value.apply(void 0, args);
            } else {
                return value[name].apply(value, args);
            }
        },
        "apply": function (thisp, args) {
            return value.apply(thisp, args);
        },
        "keys": function () {
            return object_keys(value);
        }
    }, void 0, function inspect() {
        return { state: "fulfilled", value: value };
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.get"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>get (object, key)](#apidoc.element.thrift.Q.get)
- description and source-code
```javascript
get = function (object, key) {
    return Q(object).dispatch("get", [key]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.getUnhandledReasons"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>getUnhandledReasons ()](#apidoc.element.thrift.Q.getUnhandledReasons)
- description and source-code
```javascript
getUnhandledReasons = function () {
    // Make a copy so that consumers can't interfere with our internal state.
    return unhandledReasons.slice();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.invoke"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>invoke (object, name)](#apidoc.element.thrift.Q.invoke)
- description and source-code
```javascript
invoke = function (object, name) {
    return Q(object).dispatch("post", [name, array_slice(arguments, 2)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.isFulfilled"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>isFulfilled (object)](#apidoc.element.thrift.Q.isFulfilled)
- description and source-code
```javascript
function isFulfilled(object) {
    return !isPromise(object) || object.inspect().state === "fulfilled";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.isPending"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>isPending (object)](#apidoc.element.thrift.Q.isPending)
- description and source-code
```javascript
function isPending(object) {
    return isPromise(object) && object.inspect().state === "pending";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.isPromise"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>isPromise (object)](#apidoc.element.thrift.Q.isPromise)
- description and source-code
```javascript
function isPromise(object) {
    return isObject(object) &&
        typeof object.promiseDispatch === "function" &&
        typeof object.inspect === "function";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.isPromiseAlike"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>isPromiseAlike (object)](#apidoc.element.thrift.Q.isPromiseAlike)
- description and source-code
```javascript
function isPromiseAlike(object) {
    return isObject(object) && typeof object.then === "function";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.isRejected"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>isRejected (object)](#apidoc.element.thrift.Q.isRejected)
- description and source-code
```javascript
function isRejected(object) {
    return isPromise(object) && object.inspect().state === "rejected";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.join"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>join (x, y)](#apidoc.element.thrift.Q.join)
- description and source-code
```javascript
join = function (x, y) {
    return Q(x).join(y);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.keys"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>keys (object)](#apidoc.element.thrift.Q.keys)
- description and source-code
```javascript
keys = function (object) {
    return Q(object).dispatch("keys", []);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>makePromise (descriptor, fallback, inspect)](#apidoc.element.thrift.Q.makePromise)
- description and source-code
```javascript
function Promise(descriptor, fallback, inspect) {
    if (fallback === void 0) {
        fallback = function (op) {
            return reject(new Error(
                "Promise does not support operation: " + op
            ));
        };
    }
    if (inspect === void 0) {
        inspect = function () {
            return {state: "unknown"};
        };
    }

    var promise = object_create(Promise.prototype);

    promise.promiseDispatch = function (resolve, op, args) {
        var result;
        try {
            if (descriptor[op]) {
                result = descriptor[op].apply(promise, args);
            } else {
                result = fallback.call(promise, op, args);
            }
        } catch (exception) {
            result = reject(exception);
        }
        if (resolve) {
            resolve(result);
        }
    };

    promise.inspect = inspect;

    // XXX deprecated 'valueOf' and 'exception' support
    if (inspect) {
        var inspected = inspect();
        if (inspected.state === "rejected") {
            promise.exception = inspected.reason;
        }

        promise.valueOf = function () {
            var inspected = inspect();
            if (inspected.state === "pending" ||
                inspected.state === "rejected") {
                return promise;
            }
            return inspected.value;
        };
    }

    return promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.mapply"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>mapply (object, name, args)](#apidoc.element.thrift.Q.mapply)
- description and source-code
```javascript
mapply = function (object, name, args) {
    return Q(object).dispatch("post", [name, args]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.master"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>master (object)](#apidoc.element.thrift.Q.master)
- description and source-code
```javascript
function master(object) {
    return Promise({
        "isDef": function () {}
    }, function fallback(op, args) {
        return dispatch(object, op, args);
    }, function () {
        return Q(object).inspect();
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.mcall"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>mcall (object, name)](#apidoc.element.thrift.Q.mcall)
- description and source-code
```javascript
mcall = function (object, name) {
    return Q(object).dispatch("post", [name, array_slice(arguments, 2)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.nbind"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>nbind (callback, thisp)](#apidoc.element.thrift.Q.nbind)
- description and source-code
```javascript
nbind = function (callback, thisp) {
    var baseArgs = array_slice(arguments, 2);
    return function () {
        var nodeArgs = baseArgs.concat(array_slice(arguments));
        var deferred = defer();
        nodeArgs.push(deferred.makeNodeResolver());
        function bound() {
            return callback.apply(thisp, arguments);
        }
        Q(bound).fapply(nodeArgs).fail(deferred.reject);
        return deferred.promise;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.nearer"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>nearer (value)](#apidoc.element.thrift.Q.nearer)
- description and source-code
```javascript
function nearer(value) {
    if (isPromise(value)) {
        var inspected = value.inspect();
        if (inspected.state === "fulfilled") {
            return inspected.value;
        }
    }
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.nextTick"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>nextTick (task)](#apidoc.element.thrift.Q.nextTick)
- description and source-code
```javascript
nextTick = function (task) {
    tail = tail.next = {
        task: task,
        domain: isNodeJS && process.domain,
        next: null
    };

    if (!flushing) {
        flushing = true;
        requestTick();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.nfapply"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>nfapply (callback, args)](#apidoc.element.thrift.Q.nfapply)
- description and source-code
```javascript
nfapply = function (callback, args) {
    return Q(callback).nfapply(args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.nfbind"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>nfbind (callback)](#apidoc.element.thrift.Q.nfbind)
- description and source-code
```javascript
nfbind = function (callback) {
    var baseArgs = array_slice(arguments, 1);
    return function () {
        var nodeArgs = baseArgs.concat(array_slice(arguments));
        var deferred = defer();
        nodeArgs.push(deferred.makeNodeResolver());
        Q(callback).fapply(nodeArgs).fail(deferred.reject);
        return deferred.promise;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.nfcall"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>nfcall (callback)](#apidoc.element.thrift.Q.nfcall)
- description and source-code
```javascript
nfcall = function (callback) {
    var args = array_slice(arguments, 1);
    return Q(callback).nfapply(args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.ninvoke"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>ninvoke (object, name)](#apidoc.element.thrift.Q.ninvoke)
- description and source-code
```javascript
ninvoke = function (object, name) {
    var nodeArgs = array_slice(arguments, 2);
    var deferred = defer();
    nodeArgs.push(deferred.makeNodeResolver());
    Q(object).dispatch("post", [name, nodeArgs]).fail(deferred.reject);
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.nmapply"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>nmapply (object, name, args)](#apidoc.element.thrift.Q.nmapply)
- description and source-code
```javascript
nmapply = function (object, name, args) {
    return Q(object).npost(name, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.nmcall"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>nmcall (object, name)](#apidoc.element.thrift.Q.nmcall)
- description and source-code
```javascript
nmcall = function (object, name) {
    var nodeArgs = array_slice(arguments, 2);
    var deferred = defer();
    nodeArgs.push(deferred.makeNodeResolver());
    Q(object).dispatch("post", [name, nodeArgs]).fail(deferred.reject);
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.nodeify"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>nodeify (object, nodeback)](#apidoc.element.thrift.Q.nodeify)
- description and source-code
```javascript
function nodeify(object, nodeback) {
    return Q(object).nodeify(nodeback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.npost"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>npost (object, name, args)](#apidoc.element.thrift.Q.npost)
- description and source-code
```javascript
npost = function (object, name, args) {
    return Q(object).npost(name, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.nsend"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>nsend (object, name)](#apidoc.element.thrift.Q.nsend)
- description and source-code
```javascript
nsend = function (object, name) {
    var nodeArgs = array_slice(arguments, 2);
    var deferred = defer();
    nodeArgs.push(deferred.makeNodeResolver());
    Q(object).dispatch("post", [name, nodeArgs]).fail(deferred.reject);
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.passByCopy"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>passByCopy (object)](#apidoc.element.thrift.Q.passByCopy)
- description and source-code
```javascript
passByCopy = function (object) {
    //freeze(object);
    //passByCopies.set(object, true);
    return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.post"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>post (object, name, args)](#apidoc.element.thrift.Q.post)
- description and source-code
```javascript
post = function (object, name, args) {
    return Q(object).dispatch("post", [name, args]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.progress"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>progress (object, progressed)](#apidoc.element.thrift.Q.progress)
- description and source-code
```javascript
function progress(object, progressed) {
    return Q(object).then(void 0, void 0, progressed);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.promise"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>promise (resolver)](#apidoc.element.thrift.Q.promise)
- description and source-code
```javascript
function promise(resolver) {
    if (typeof resolver !== "function") {
        throw new TypeError("resolver must be a function.");
    }
    var deferred = defer();
    try {
        resolver(deferred.resolve, deferred.reject, deferred.notify);
    } catch (reason) {
        deferred.reject(reason);
    }
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.promised"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>promised (callback)](#apidoc.element.thrift.Q.promised)
- description and source-code
```javascript
function promised(callback) {
    return function () {
        return spread([this, all(arguments)], function (self, args) {
            return callback.apply(self, args);
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.race"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>race (answerPs)](#apidoc.element.thrift.Q.race)
- description and source-code
```javascript
function race(answerPs) {
    return promise(function(resolve, reject) {
        // Switch to this once we can assume at least ES5
        // answerPs.forEach(function(answerP) {
        //     Q(answerP).then(resolve, reject);
        // });
        // Use this in the meantime
        for (var i = 0, len = answerPs.length; i < len; i++) {
            Q(answerPs[i]).then(resolve, reject);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.reject"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>reject (reason)](#apidoc.element.thrift.Q.reject)
- description and source-code
```javascript
function reject(reason) {
    var rejection = Promise({
        "when": function (rejected) {
            // note that the error has been handled
            if (rejected) {
                untrackRejection(this);
            }
            return rejected ? rejected(reason) : this;
        }
    }, function fallback() {
        return this;
    }, function inspect() {
        return { state: "rejected", reason: reason };
    });

    // Note that the reason has not been handled.
    trackRejection(rejection, reason);

    return rejection;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.resetUnhandledRejections"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>resetUnhandledRejections ()](#apidoc.element.thrift.Q.resetUnhandledRejections)
- description and source-code
```javascript
function resetUnhandledRejections() {
    unhandledReasons.length = 0;
    unhandledRejections.length = 0;

    if (!trackUnhandledRejections) {
        trackUnhandledRejections = true;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.resolve"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>resolve (value)](#apidoc.element.thrift.Q.resolve)
- description and source-code
```javascript
function Q(value) {
    // If the object is already a Promise, return it directly.  This enables
    // the resolve function to both be used to created references from objects,
    // but to tolerably coerce non-promises to promises.
    if (isPromise(value)) {
        return value;
    }

    // assimilate thenables
    if (isPromiseAlike(value)) {
        return coerce(value);
    } else {
        return fulfill(value);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.return"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>return (value)](#apidoc.element.thrift.Q.return)
- description and source-code
```javascript
function _return(value) {
    throw new QReturnValue(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.send"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>send (object, name)](#apidoc.element.thrift.Q.send)
- description and source-code
```javascript
send = function (object, name) {
    return Q(object).dispatch("post", [name, array_slice(arguments, 2)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.set"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>set (object, key, value)](#apidoc.element.thrift.Q.set)
- description and source-code
```javascript
set = function (object, key, value) {
    return Q(object).dispatch("set", [key, value]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.spawn"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>spawn (makeGenerator)](#apidoc.element.thrift.Q.spawn)
- description and source-code
```javascript
function spawn(makeGenerator) {
    Q.done(Q.async(makeGenerator)());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.spread"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>spread (value, fulfilled, rejected)](#apidoc.element.thrift.Q.spread)
- description and source-code
```javascript
function spread(value, fulfilled, rejected) {
    return Q(value).spread(fulfilled, rejected);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.stopUnhandledRejectionTracking"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>stopUnhandledRejectionTracking ()](#apidoc.element.thrift.Q.stopUnhandledRejectionTracking)
- description and source-code
```javascript
stopUnhandledRejectionTracking = function () {
    resetUnhandledRejections();
    trackUnhandledRejections = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.thenReject"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>thenReject (promise, reason)](#apidoc.element.thrift.Q.thenReject)
- description and source-code
```javascript
thenReject = function (promise, reason) {
    return Q(promise).thenReject(reason);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.thenResolve"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>thenResolve (promise, value)](#apidoc.element.thrift.Q.thenResolve)
- description and source-code
```javascript
thenResolve = function (promise, value) {
    return Q(promise).thenResolve(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.timeout"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>timeout (object, ms, message)](#apidoc.element.thrift.Q.timeout)
- description and source-code
```javascript
timeout = function (object, ms, message) {
    return Q(object).timeout(ms, message);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.try"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>try (object)](#apidoc.element.thrift.Q.try)
- description and source-code
```javascript
try = function (object) {
    return Q(object).dispatch("apply", [void 0, array_slice(arguments, 1)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.when"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>when (value, fulfilled, rejected, progressed)](#apidoc.element.thrift.Q.when)
- description and source-code
```javascript
function when(value, fulfilled, rejected, progressed) {
    return Q(value).then(fulfilled, rejected, progressed);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Q.Promise"></a>[module thrift.Q.Promise](#apidoc.module.thrift.Q.Promise)

#### <a name="apidoc.element.thrift.Q.Promise.Promise"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>Promise (resolver)](#apidoc.element.thrift.Q.Promise.Promise)
- description and source-code
```javascript
function promise(resolver) {
    if (typeof resolver !== "function") {
        throw new TypeError("resolver must be a function.");
    }
    var deferred = defer();
    try {
        resolver(deferred.resolve, deferred.reject, deferred.notify);
    } catch (reason) {
        deferred.reject(reason);
    }
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.Promise.all"></a>[function <span class="apidocSignatureSpan">thrift.Q.Promise.</span>all (promises)](#apidoc.element.thrift.Q.Promise.all)
- description and source-code
```javascript
function all(promises) {
    return when(promises, function (promises) {
        var countDown = 0;
        var deferred = defer();
        array_reduce(promises, function (undefined, promise, index) {
            var snapshot;
            if (
                isPromise(promise) &&
                (snapshot = promise.inspect()).state === "fulfilled"
            ) {
                promises[index] = snapshot.value;
            } else {
                ++countDown;
                when(
                    promise,
                    function (value) {
                        promises[index] = value;
                        if (--countDown === 0) {
                            deferred.resolve(promises);
                        }
                    },
                    deferred.reject,
                    function (progress) {
                        deferred.notify({ index: index, value: progress });
                    }
                );
            }
        }, void 0);
        if (countDown === 0) {
            deferred.resolve(promises);
        }
        return deferred.promise;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.Promise.race"></a>[function <span class="apidocSignatureSpan">thrift.Q.Promise.</span>race (answerPs)](#apidoc.element.thrift.Q.Promise.race)
- description and source-code
```javascript
function race(answerPs) {
    return promise(function(resolve, reject) {
        // Switch to this once we can assume at least ES5
        // answerPs.forEach(function(answerP) {
        //     Q(answerP).then(resolve, reject);
        // });
        // Use this in the meantime
        for (var i = 0, len = answerPs.length; i < len; i++) {
            Q(answerPs[i]).then(resolve, reject);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.Promise.reject"></a>[function <span class="apidocSignatureSpan">thrift.Q.Promise.</span>reject (reason)](#apidoc.element.thrift.Q.Promise.reject)
- description and source-code
```javascript
function reject(reason) {
    var rejection = Promise({
        "when": function (rejected) {
            // note that the error has been handled
            if (rejected) {
                untrackRejection(this);
            }
            return rejected ? rejected(reason) : this;
        }
    }, function fallback() {
        return this;
    }, function inspect() {
        return { state: "rejected", reason: reason };
    });

    // Note that the reason has not been handled.
    trackRejection(rejection, reason);

    return rejection;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.Promise.resolve"></a>[function <span class="apidocSignatureSpan">thrift.Q.Promise.</span>resolve (value)](#apidoc.element.thrift.Q.Promise.resolve)
- description and source-code
```javascript
function Q(value) {
    // If the object is already a Promise, return it directly.  This enables
    // the resolve function to both be used to created references from objects,
    // but to tolerably coerce non-promises to promises.
    if (isPromise(value)) {
        return value;
    }

    // assimilate thenables
    if (isPromiseAlike(value)) {
        return coerce(value);
    } else {
        return fulfill(value);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Q.defer"></a>[module thrift.Q.defer](#apidoc.module.thrift.Q.defer)

#### <a name="apidoc.element.thrift.Q.defer.defer"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>defer ()](#apidoc.element.thrift.Q.defer.defer)
- description and source-code
```javascript
function defer() {
    // if "messages" is an "Array", that indicates that the promise has not yet
    // been resolved.  If it is "undefined", it has been resolved.  Each
    // element of the messages array is itself an array of complete arguments to
    // forward to the resolved promise.  We coerce the resolution value to a
    // promise using the 'resolve' function because it handles both fully
    // non-thenable values and other thenables gracefully.
    var messages = [], progressListeners = [], resolvedPromise;

    var deferred = object_create(defer.prototype);
    var promise = object_create(Promise.prototype);

    promise.promiseDispatch = function (resolve, op, operands) {
        var args = array_slice(arguments);
        if (messages) {
            messages.push(args);
            if (op === "when" && operands[1]) { // progress operand
                progressListeners.push(operands[1]);
            }
        } else {
            nextTick(function () {
                resolvedPromise.promiseDispatch.apply(resolvedPromise, args);
            });
        }
    };

    // XXX deprecated
    promise.valueOf = function () {
        if (messages) {
            return promise;
        }
        var nearerValue = nearer(resolvedPromise);
        if (isPromise(nearerValue)) {
            resolvedPromise = nearerValue; // shorten chain
        }
        return nearerValue;
    };

    promise.inspect = function () {
        if (!resolvedPromise) {
            return { state: "pending" };
        }
        return resolvedPromise.inspect();
    };

    if (Q.longStackSupport && hasStacks) {
        try {
            throw new Error();
        } catch (e) {
            // NOTE: don't try to use 'Error.captureStackTrace' or transfer the
            // accessor around; that causes memory leaks as per GH-111. Just
            // reify the stack trace as a string ASAP.
            //
            // At the same time, cut off the first line; it's always just
            // "[object Promise]\n", as per the 'toString'.
            promise.stack = e.stack.substring(e.stack.indexOf("\n") + 1);
        }
    }

    // NOTE: we do the checks for 'resolvedPromise' in each method, instead of
    // consolidating them into 'become', since otherwise we'd create new
    // promises with the lines 'become(whatever(value))'. See e.g. GH-252.

    function become(newPromise) {
        resolvedPromise = newPromise;
        promise.source = newPromise;

        array_reduce(messages, function (undefined, message) {
            nextTick(function () {
                newPromise.promiseDispatch.apply(newPromise, message);
            });
        }, void 0);

        messages = void 0;
        progressListeners = void 0;
    }

    deferred.promise = promise;
    deferred.resolve = function (value) {
        if (resolvedPromise) {
            return;
        }

        become(Q(value));
    };

    deferred.fulfill = function (value) {
        if (resolvedPromise) {
            return;
        }

        become(fulfill(value));
    };
    deferred.reject = function (reason) {
        if (resolvedPromise) {
            return;
        }

        become(reject(reason));
    };
    deferred.notify = function (progress) {
        if (resolvedPromise) {
            return;
        }

        array_reduce(progressListeners, function (undefined, progressListener) {
            nextTick(function () {
                progressListener(progress);
            });
        }, void 0);
    };

    return deferred;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Q.defer.prototype"></a>[module thrift.Q.defer.prototype](#apidoc.module.thrift.Q.defer.prototype)

#### <a name="apidoc.element.thrift.Q.defer.prototype.makeNodeResolver"></a>[function <span class="apidocSignatureSpan">thrift.Q.defer.prototype.</span>makeNodeResolver ()](#apidoc.element.thrift.Q.defer.prototype.makeNodeResolver)
- description and source-code
```javascript
makeNodeResolver = function () {
    var self = this;
    return function (error, value) {
        if (error) {
            self.reject(error);
        } else if (arguments.length > 2) {
            self.resolve(array_slice(arguments, 1));
        } else {
            self.resolve(value);
        }
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Q.makePromise"></a>[module thrift.Q.makePromise](#apidoc.module.thrift.Q.makePromise)

#### <a name="apidoc.element.thrift.Q.makePromise.makePromise"></a>[function <span class="apidocSignatureSpan">thrift.Q.</span>makePromise (descriptor, fallback, inspect)](#apidoc.element.thrift.Q.makePromise.makePromise)
- description and source-code
```javascript
function Promise(descriptor, fallback, inspect) {
    if (fallback === void 0) {
        fallback = function (op) {
            return reject(new Error(
                "Promise does not support operation: " + op
            ));
        };
    }
    if (inspect === void 0) {
        inspect = function () {
            return {state: "unknown"};
        };
    }

    var promise = object_create(Promise.prototype);

    promise.promiseDispatch = function (resolve, op, args) {
        var result;
        try {
            if (descriptor[op]) {
                result = descriptor[op].apply(promise, args);
            } else {
                result = fallback.call(promise, op, args);
            }
        } catch (exception) {
            result = reject(exception);
        }
        if (resolve) {
            resolve(result);
        }
    };

    promise.inspect = inspect;

    // XXX deprecated 'valueOf' and 'exception' support
    if (inspect) {
        var inspected = inspect();
        if (inspected.state === "rejected") {
            promise.exception = inspected.reason;
        }

        promise.valueOf = function () {
            var inspected = inspect();
            if (inspected.state === "pending" ||
                inspected.state === "rejected") {
                return promise;
            }
            return inspected.value;
        };
    }

    return promise;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Q.makePromise.prototype"></a>[module thrift.Q.makePromise.prototype](#apidoc.module.thrift.Q.makePromise.prototype)

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.all"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>all ()](#apidoc.element.thrift.Q.makePromise.prototype.all)
- description and source-code
```javascript
all = function () {
    return all(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.allResolved"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>allResolved ()](#apidoc.element.thrift.Q.makePromise.prototype.allResolved)
- description and source-code
```javascript
allResolved = function () {
    return allResolved(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.allSettled"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>allSettled ()](#apidoc.element.thrift.Q.makePromise.prototype.allSettled)
- description and source-code
```javascript
allSettled = function () {
    return this.then(function (promises) {
        return all(array_map(promises, function (promise) {
            promise = Q(promise);
            function regardless() {
                return promise.inspect();
            }
            return promise.then(regardless, regardless);
        }));
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.catch"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>catch (rejected)](#apidoc.element.thrift.Q.makePromise.prototype.catch)
- description and source-code
```javascript
catch = function (rejected) {
    return this.then(void 0, rejected);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.del"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>del (key)](#apidoc.element.thrift.Q.makePromise.prototype.del)
- description and source-code
```javascript
del = function (key) {
    return this.dispatch("delete", [key]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.delay"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>delay (timeout)](#apidoc.element.thrift.Q.makePromise.prototype.delay)
- description and source-code
```javascript
delay = function (timeout) {
    return this.then(function (value) {
        var deferred = defer();
        setTimeout(function () {
            deferred.resolve(value);
        }, timeout);
        return deferred.promise;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.delete"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>delete (key)](#apidoc.element.thrift.Q.makePromise.prototype.delete)
- description and source-code
```javascript
delete = function (key) {
    return this.dispatch("delete", [key]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.denodeify"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>denodeify ()](#apidoc.element.thrift.Q.makePromise.prototype.denodeify)
- description and source-code
```javascript
denodeify = function () {
    var args = array_slice(arguments);
    args.unshift(this);
    return Q.denodeify.apply(void 0, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>dispatch (op, args)](#apidoc.element.thrift.Q.makePromise.prototype.dispatch)
- description and source-code
```javascript
dispatch = function (op, args) {
    var self = this;
    var deferred = defer();
    nextTick(function () {
        self.promiseDispatch(deferred.resolve, op, args);
    });
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.done"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>done (fulfilled, rejected, progress)](#apidoc.element.thrift.Q.makePromise.prototype.done)
- description and source-code
```javascript
done = function (fulfilled, rejected, progress) {
    var onUnhandledError = function (error) {
        // forward to a future turn so that ''when''
        // does not catch it and turn it into a rejection.
        nextTick(function () {
            makeStackTraceLong(error, promise);
            if (Q.onerror) {
                Q.onerror(error);
            } else {
                throw error;
            }
        });
    };

    // Avoid unnecessary 'nextTick'ing via an unnecessary 'when'.
    var promise = fulfilled || rejected || progress ?
        this.then(fulfilled, rejected, progress) :
        this;

    if (typeof process === "object" && process && process.domain) {
        onUnhandledError = process.domain.bind(onUnhandledError);
    }

    promise.then(void 0, onUnhandledError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.fail"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>fail (rejected)](#apidoc.element.thrift.Q.makePromise.prototype.fail)
- description and source-code
```javascript
fail = function (rejected) {
    return this.then(void 0, rejected);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.fapply"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>fapply (args)](#apidoc.element.thrift.Q.makePromise.prototype.fapply)
- description and source-code
```javascript
fapply = function (args) {
    return this.dispatch("apply", [void 0, args]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.fbind"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>fbind ()](#apidoc.element.thrift.Q.makePromise.prototype.fbind)
- description and source-code
```javascript
fbind = function () {
    var promise = this;
    var args = array_slice(arguments);
    return function fbound() {
        return promise.dispatch("apply", [
            this,
            args.concat(array_slice(arguments))
        ]);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.fcall"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>fcall ()](#apidoc.element.thrift.Q.makePromise.prototype.fcall)
- description and source-code
```javascript
fcall = function () {
    return this.dispatch("apply", [void 0, array_slice(arguments)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.fin"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>fin (callback)](#apidoc.element.thrift.Q.makePromise.prototype.fin)
- description and source-code
```javascript
fin = function (callback) {
    callback = Q(callback);
    return this.then(function (value) {
        return callback.fcall().then(function () {
            return value;
        });
    }, function (reason) {
        // TODO attempt to recycle the rejection with "this".
        return callback.fcall().then(function () {
            throw reason;
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.finally"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>finally (callback)](#apidoc.element.thrift.Q.makePromise.prototype.finally)
- description and source-code
```javascript
finally = function (callback) {
    callback = Q(callback);
    return this.then(function (value) {
        return callback.fcall().then(function () {
            return value;
        });
    }, function (reason) {
        // TODO attempt to recycle the rejection with "this".
        return callback.fcall().then(function () {
            throw reason;
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.get"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>get (key)](#apidoc.element.thrift.Q.makePromise.prototype.get)
- description and source-code
```javascript
get = function (key) {
    return this.dispatch("get", [key]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.invoke"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>invoke (name)](#apidoc.element.thrift.Q.makePromise.prototype.invoke)
- description and source-code
```javascript
invoke = function (name) {
    return this.dispatch("post", [name, array_slice(arguments, 1)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.isFulfilled"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>isFulfilled ()](#apidoc.element.thrift.Q.makePromise.prototype.isFulfilled)
- description and source-code
```javascript
isFulfilled = function () {
    return this.inspect().state === "fulfilled";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.isPending"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>isPending ()](#apidoc.element.thrift.Q.makePromise.prototype.isPending)
- description and source-code
```javascript
isPending = function () {
    return this.inspect().state === "pending";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.isRejected"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>isRejected ()](#apidoc.element.thrift.Q.makePromise.prototype.isRejected)
- description and source-code
```javascript
isRejected = function () {
    return this.inspect().state === "rejected";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.join"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>join (that)](#apidoc.element.thrift.Q.makePromise.prototype.join)
- description and source-code
```javascript
join = function (that) {
    return Q([this, that]).spread(function (x, y) {
        if (x === y) {
            // TODO: "===" should be Object.is or equiv
            return x;
        } else {
            throw new Error("Can't join: not the same: " + x + " " + y);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.keys"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>keys ()](#apidoc.element.thrift.Q.makePromise.prototype.keys)
- description and source-code
```javascript
keys = function () {
    return this.dispatch("keys", []);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.mapply"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>mapply (name, args)](#apidoc.element.thrift.Q.makePromise.prototype.mapply)
- description and source-code
```javascript
mapply = function (name, args) {
    return this.dispatch("post", [name, args]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.mcall"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>mcall (name)](#apidoc.element.thrift.Q.makePromise.prototype.mcall)
- description and source-code
```javascript
mcall = function (name) {
    return this.dispatch("post", [name, array_slice(arguments, 1)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.nbind"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nbind ()](#apidoc.element.thrift.Q.makePromise.prototype.nbind)
- description and source-code
```javascript
nbind = function () {
    var args = array_slice(arguments, 0);
    args.unshift(this);
    return Q.nbind.apply(void 0, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.nfapply"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nfapply (args)](#apidoc.element.thrift.Q.makePromise.prototype.nfapply)
- description and source-code
```javascript
nfapply = function (args) {
    var deferred = defer();
    var nodeArgs = array_slice(args);
    nodeArgs.push(deferred.makeNodeResolver());
    this.fapply(nodeArgs).fail(deferred.reject);
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.nfbind"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nfbind ()](#apidoc.element.thrift.Q.makePromise.prototype.nfbind)
- description and source-code
```javascript
nfbind = function () {
    var args = array_slice(arguments);
    args.unshift(this);
    return Q.denodeify.apply(void 0, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.nfcall"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nfcall ()](#apidoc.element.thrift.Q.makePromise.prototype.nfcall)
- description and source-code
```javascript
nfcall = function () {
    var nodeArgs = array_slice(arguments);
    var deferred = defer();
    nodeArgs.push(deferred.makeNodeResolver());
    this.fapply(nodeArgs).fail(deferred.reject);
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.ninvoke"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>ninvoke (name)](#apidoc.element.thrift.Q.makePromise.prototype.ninvoke)
- description and source-code
```javascript
ninvoke = function (name) {
    var nodeArgs = array_slice(arguments, 1);
    var deferred = defer();
    nodeArgs.push(deferred.makeNodeResolver());
    this.dispatch("post", [name, nodeArgs]).fail(deferred.reject);
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.nmapply"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nmapply (name, args)](#apidoc.element.thrift.Q.makePromise.prototype.nmapply)
- description and source-code
```javascript
nmapply = function (name, args) {
    var nodeArgs = array_slice(args || []);
    var deferred = defer();
    nodeArgs.push(deferred.makeNodeResolver());
    this.dispatch("post", [name, nodeArgs]).fail(deferred.reject);
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.nmcall"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nmcall (name)](#apidoc.element.thrift.Q.makePromise.prototype.nmcall)
- description and source-code
```javascript
nmcall = function (name) {
    var nodeArgs = array_slice(arguments, 1);
    var deferred = defer();
    nodeArgs.push(deferred.makeNodeResolver());
    this.dispatch("post", [name, nodeArgs]).fail(deferred.reject);
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.nodeify"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nodeify (nodeback)](#apidoc.element.thrift.Q.makePromise.prototype.nodeify)
- description and source-code
```javascript
nodeify = function (nodeback) {
    if (nodeback) {
        this.then(function (value) {
            nextTick(function () {
                nodeback(null, value);
            });
        }, function (error) {
            nextTick(function () {
                nodeback(error);
            });
        });
    } else {
        return this;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.npost"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>npost (name, args)](#apidoc.element.thrift.Q.makePromise.prototype.npost)
- description and source-code
```javascript
npost = function (name, args) {
    var nodeArgs = array_slice(args || []);
    var deferred = defer();
    nodeArgs.push(deferred.makeNodeResolver());
    this.dispatch("post", [name, nodeArgs]).fail(deferred.reject);
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.nsend"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>nsend (name)](#apidoc.element.thrift.Q.makePromise.prototype.nsend)
- description and source-code
```javascript
nsend = function (name) {
    var nodeArgs = array_slice(arguments, 1);
    var deferred = defer();
    nodeArgs.push(deferred.makeNodeResolver());
    this.dispatch("post", [name, nodeArgs]).fail(deferred.reject);
    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.passByCopy"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>passByCopy ()](#apidoc.element.thrift.Q.makePromise.prototype.passByCopy)
- description and source-code
```javascript
passByCopy = function () {
    //freeze(object);
    //passByCopies.set(object, true);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.post"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>post (name, args)](#apidoc.element.thrift.Q.makePromise.prototype.post)
- description and source-code
```javascript
post = function (name, args) {
    return this.dispatch("post", [name, args]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.progress"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>progress (progressed)](#apidoc.element.thrift.Q.makePromise.prototype.progress)
- description and source-code
```javascript
progress = function (progressed) {
    return this.then(void 0, void 0, progressed);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.race"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>race ()](#apidoc.element.thrift.Q.makePromise.prototype.race)
- description and source-code
```javascript
race = function () {
    return this.then(Q.race);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.send"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>send (name)](#apidoc.element.thrift.Q.makePromise.prototype.send)
- description and source-code
```javascript
send = function (name) {
    return this.dispatch("post", [name, array_slice(arguments, 1)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.set"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>set (key, value)](#apidoc.element.thrift.Q.makePromise.prototype.set)
- description and source-code
```javascript
set = function (key, value) {
    return this.dispatch("set", [key, value]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.spread"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>spread (fulfilled, rejected)](#apidoc.element.thrift.Q.makePromise.prototype.spread)
- description and source-code
```javascript
spread = function (fulfilled, rejected) {
    return this.all().then(function (array) {
        return fulfilled.apply(void 0, array);
    }, rejected);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.then"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>then (fulfilled, rejected, progressed)](#apidoc.element.thrift.Q.makePromise.prototype.then)
- description and source-code
```javascript
then = function (fulfilled, rejected, progressed) {
    var self = this;
    var deferred = defer();
    var done = false;   // ensure the untrusted promise makes at most a
                        // single call to one of the callbacks

    function _fulfilled(value) {
        try {
            return typeof fulfilled === "function" ? fulfilled(value) : value;
        } catch (exception) {
            return reject(exception);
        }
    }

    function _rejected(exception) {
        if (typeof rejected === "function") {
            makeStackTraceLong(exception, self);
            try {
                return rejected(exception);
            } catch (newException) {
                return reject(newException);
            }
        }
        return reject(exception);
    }

    function _progressed(value) {
        return typeof progressed === "function" ? progressed(value) : value;
    }

    nextTick(function () {
        self.promiseDispatch(function (value) {
            if (done) {
                return;
            }
            done = true;

            deferred.resolve(_fulfilled(value));
        }, "when", [function (exception) {
            if (done) {
                return;
            }
            done = true;

            deferred.resolve(_rejected(exception));
        }]);
    });

    // Progress propagator need to be attached in the current tick.
    self.promiseDispatch(void 0, "when", [void 0, function (value) {
        var newValue;
        var threw = false;
        try {
            newValue = _progressed(value);
        } catch (e) {
            threw = true;
            if (Q.onerror) {
                Q.onerror(e);
            } else {
                throw e;
            }
        }

        if (!threw) {
            deferred.notify(newValue);
        }
    }]);

    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.thenReject"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>thenReject (reason)](#apidoc.element.thrift.Q.makePromise.prototype.thenReject)
- description and source-code
```javascript
thenReject = function (reason) {
    return this.then(function () { throw reason; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.thenResolve"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>thenResolve (value)](#apidoc.element.thrift.Q.makePromise.prototype.thenResolve)
- description and source-code
```javascript
thenResolve = function (value) {
    return this.then(function () { return value; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.timeout"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>timeout (ms, message)](#apidoc.element.thrift.Q.makePromise.prototype.timeout)
- description and source-code
```javascript
timeout = function (ms, message) {
    var deferred = defer();
    var timeoutId = setTimeout(function () {
        deferred.reject(new Error(message || "Timed out after " + ms + " ms"));
    }, ms);

    this.then(function (value) {
        clearTimeout(timeoutId);
        deferred.resolve(value);
    }, function (exception) {
        clearTimeout(timeoutId);
        deferred.reject(exception);
    }, deferred.notify);

    return deferred.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Q.makePromise.prototype.toString"></a>[function <span class="apidocSignatureSpan">thrift.Q.makePromise.prototype.</span>toString ()](#apidoc.element.thrift.Q.makePromise.prototype.toString)
- description and source-code
```javascript
toString = function () {
    return "[object Promise]";
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.TBinaryProtocol"></a>[module thrift.TBinaryProtocol](#apidoc.module.thrift.TBinaryProtocol)

#### <a name="apidoc.element.thrift.TBinaryProtocol.TBinaryProtocol"></a>[function <span class="apidocSignatureSpan">thrift.</span>TBinaryProtocol (trans, strictRead, strictWrite)](#apidoc.element.thrift.TBinaryProtocol.TBinaryProtocol)
- description and source-code
```javascript
function TBinaryProtocol(trans, strictRead, strictWrite) {
  this.trans = trans;
  this.strictRead = (strictRead !== undefined ? strictRead : false);
  this.strictWrite = (strictWrite !== undefined ? strictWrite : true);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.TBinaryProtocol.prototype"></a>[module thrift.TBinaryProtocol.prototype](#apidoc.module.thrift.TBinaryProtocol.prototype)

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.flush"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>flush ()](#apidoc.element.thrift.TBinaryProtocol.prototype.flush)
- description and source-code
```javascript
flush = function () {
  return this.trans.flush();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.getTransport"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>getTransport ()](#apidoc.element.thrift.TBinaryProtocol.prototype.getTransport)
- description and source-code
```javascript
getTransport = function () {
  return this.trans;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readBinary"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readBinary ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readBinary)
- description and source-code
```javascript
readBinary = function () {
  var len = this.readI32();
  if (len === 0) {
    return new Buffer(0);
  }

  if (len < 0) {
    throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.NEGATIVE_SIZE, "Negative binary size");
  }
  return this.trans.read(len);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readBool"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readBool ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readBool)
- description and source-code
```javascript
readBool = function () {
  var b = this.readByte();
  if (b === 0) {
    return false;
  }
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readByte"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readByte ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readByte)
- description and source-code
```javascript
readByte = function () {
  return this.trans.readByte();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readDouble"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readDouble ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readDouble)
- description and source-code
```javascript
readDouble = function () {
  return this.trans.readDouble();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readFieldBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readFieldBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readFieldBegin)
- description and source-code
```javascript
readFieldBegin = function () {
  var type = this.readByte();
  if (type == Type.STOP) {
    return {fname: null, ftype: type, fid: 0};
  }
  var id = this.readI16();
  return {fname: null, ftype: type, fid: id};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readFieldEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readFieldEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readFieldEnd)
- description and source-code
```javascript
readFieldEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readI16"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readI16 ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readI16)
- description and source-code
```javascript
readI16 = function () {
  return this.trans.readI16();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readI32"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readI32 ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readI32)
- description and source-code
```javascript
readI32 = function () {
  return this.trans.readI32();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readI64"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readI64 ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readI64)
- description and source-code
```javascript
readI64 = function () {
  var buff = this.trans.read(8);
  return new Int64(buff);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readListBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readListBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readListBegin)
- description and source-code
```javascript
readListBegin = function () {
  var etype = this.readByte();
  var size = this.readI32();
  return {etype: etype, size: size};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readListEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readListEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readListEnd)
- description and source-code
```javascript
readListEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readMapBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readMapBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readMapBegin)
- description and source-code
```javascript
readMapBegin = function () {
  var ktype = this.readByte();
  var vtype = this.readByte();
  var size = this.readI32();
  return {ktype: ktype, vtype: vtype, size: size};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readMapEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readMapEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readMapEnd)
- description and source-code
```javascript
readMapEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readMessageBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readMessageBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readMessageBegin)
- description and source-code
```javascript
readMessageBegin = function () {
  var sz = this.readI32();
  var type, name, seqid;

  if (sz < 0) {
    var version = sz & VERSION_MASK;
    if (version != VERSION_1) {
      console.log("BAD: " + version);
      throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.BAD_VERSION, "Bad version in readMessageBegin: " + sz);
    }
    type = sz & TYPE_MASK;
    name = this.readString();
    seqid = this.readI32();
  } else {
    if (this.strictRead) {
      throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.BAD_VERSION, "No protocol version header");
    }
    name = this.trans.read(sz);
    type = this.readByte();
    seqid = this.readI32();
  }
  return {fname: name, mtype: type, rseqid: seqid};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readMessageEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readMessageEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readMessageEnd)
- description and source-code
```javascript
readMessageEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readSetBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readSetBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readSetBegin)
- description and source-code
```javascript
readSetBegin = function () {
  var etype = this.readByte();
  var size = this.readI32();
  return {etype: etype, size: size};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readSetEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readSetEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readSetEnd)
- description and source-code
```javascript
readSetEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readString"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readString ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readString)
- description and source-code
```javascript
readString = function () {
  var len = this.readI32();
  if (len === 0) {
    return "";
  }

  if (len < 0) {
    throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.NEGATIVE_SIZE, "Negative string size");
  }
  return this.trans.readString(len);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readStructBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readStructBegin ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readStructBegin)
- description and source-code
```javascript
readStructBegin = function () {
  return {fname: ''};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.readStructEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>readStructEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.readStructEnd)
- description and source-code
```javascript
readStructEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.skip"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>skip (type)](#apidoc.element.thrift.TBinaryProtocol.prototype.skip)
- description and source-code
```javascript
skip = function (type) {
  switch (type) {
    case Type.STOP:
      return;
    case Type.BOOL:
      this.readBool();
      break;
    case Type.BYTE:
      this.readByte();
      break;
    case Type.I16:
      this.readI16();
      break;
    case Type.I32:
      this.readI32();
      break;
    case Type.I64:
      this.readI64();
      break;
    case Type.DOUBLE:
      this.readDouble();
      break;
    case Type.STRING:
      this.readString();
      break;
    case Type.STRUCT:
      this.readStructBegin();
      while (true) {
        var r = this.readFieldBegin();
        if (r.ftype === Type.STOP) {
          break;
        }
        this.skip(r.ftype);
        this.readFieldEnd();
      }
      this.readStructEnd();
      break;
    case Type.MAP:
      var mapBegin = this.readMapBegin();
      for (var i = 0; i < mapBegin.size; ++i) {
        this.skip(mapBegin.ktype);
        this.skip(mapBegin.vtype);
      }
      this.readMapEnd();
      break;
    case Type.SET:
      var setBegin = this.readSetBegin();
      for (var i2 = 0; i2 < setBegin.size; ++i2) {
        this.skip(setBegin.etype);
      }
      this.readSetEnd();
      break;
    case Type.LIST:
      var listBegin = this.readListBegin();
      for (var i3 = 0; i3 < listBegin.size; ++i3) {
        this.skip(listBegin.etype);
      }
      this.readListEnd();
      break;
    default:
      throw new  Error("Invalid type: " + type);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeBinary"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeBinary (arg)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeBinary)
- description and source-code
```javascript
writeBinary = function (arg) {
  this.writeStringOrBinary('writeBinary', 'binary', arg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeBool"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeBool (bool)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeBool)
- description and source-code
```javascript
writeBool = function (bool) {
  if (bool) {
    this.writeByte(1);
  } else {
    this.writeByte(0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeByte"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeByte (b)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeByte)
- description and source-code
```javascript
writeByte = function (b) {
  this.trans.write(new Buffer([b]));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeDouble"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeDouble (dub)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeDouble)
- description and source-code
```javascript
writeDouble = function (dub) {
  this.trans.write(binary.writeDouble(new Buffer(8), dub));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeFieldBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeFieldBegin (name, type, id)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeFieldBegin)
- description and source-code
```javascript
writeFieldBegin = function (name, type, id) {
  this.writeByte(type);
  this.writeI16(id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeFieldEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeFieldEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeFieldEnd)
- description and source-code
```javascript
writeFieldEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeFieldStop"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeFieldStop ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeFieldStop)
- description and source-code
```javascript
writeFieldStop = function () {
  this.writeByte(Type.STOP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeI16"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeI16 (i16)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeI16)
- description and source-code
```javascript
writeI16 = function (i16) {
  this.trans.write(binary.writeI16(new Buffer(2), i16));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeI32"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeI32 (i32)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeI32)
- description and source-code
```javascript
writeI32 = function (i32) {
  this.trans.write(binary.writeI32(new Buffer(4), i32));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeI64"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeI64 (i64)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeI64)
- description and source-code
```javascript
writeI64 = function (i64) {
  if (i64.buffer) {
    this.trans.write(i64.buffer);
  } else {
    this.trans.write(new Int64(i64).buffer);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeListBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeListBegin (etype, size)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeListBegin)
- description and source-code
```javascript
writeListBegin = function (etype, size) {
  this.writeByte(etype);
  this.writeI32(size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeListEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeListEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeListEnd)
- description and source-code
```javascript
writeListEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeMapBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeMapBegin (ktype, vtype, size)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeMapBegin)
- description and source-code
```javascript
writeMapBegin = function (ktype, vtype, size) {
  this.writeByte(ktype);
  this.writeByte(vtype);
  this.writeI32(size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeMapEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeMapEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeMapEnd)
- description and source-code
```javascript
writeMapEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeMessageBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeMessageBegin (name, type, seqid)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeMessageBegin)
- description and source-code
```javascript
writeMessageBegin = function (name, type, seqid) {
    if (this.strictWrite) {
      this.writeI32(VERSION_1 | type);
      this.writeString(name);
      this.writeI32(seqid);
    } else {
      this.writeString(name);
      this.writeByte(type);
      this.writeI32(seqid);
    }
    // Record client seqid to find callback again
    if (this._seqid) {
      // TODO better logging log warning
      log.warning('SeqId already set', { 'name': name });
    } else {
      this._seqid = seqid;
      this.trans.setCurrSeqId(seqid);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeMessageEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeMessageEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeMessageEnd)
- description and source-code
```javascript
writeMessageEnd = function () {
    if (this._seqid) {
        this._seqid = null;
    } else {
        log.warning('No seqid to unset');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeSetBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeSetBegin (etype, size)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeSetBegin)
- description and source-code
```javascript
writeSetBegin = function (etype, size) {
  this.writeByte(etype);
  this.writeI32(size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeSetEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeSetEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeSetEnd)
- description and source-code
```javascript
writeSetEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeString"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeString (arg)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeString)
- description and source-code
```javascript
writeString = function (arg) {
  this.writeStringOrBinary('writeString', 'utf8', arg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeStringOrBinary"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeStringOrBinary (name, encoding, arg)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeStringOrBinary)
- description and source-code
```javascript
writeStringOrBinary = function (name, encoding, arg) {
  if (typeof(arg) === 'string') {
    this.writeI32(Buffer.byteLength(arg, encoding));
    this.trans.write(new Buffer(arg, encoding));
  } else if ((arg instanceof Buffer) ||
             (Object.prototype.toString.call(arg) == '[object Uint8Array]')) {
    // Buffers in Node.js under Browserify may extend UInt8Array instead of
    // defining a new object. We detect them here so we can write them
    // correctly
    this.writeI32(arg.length);
    this.trans.write(arg);
  } else {
    throw new Error(name + ' called without a string/Buffer argument: ' + arg);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeStructBegin"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeStructBegin (name)](#apidoc.element.thrift.TBinaryProtocol.prototype.writeStructBegin)
- description and source-code
```javascript
writeStructBegin = function (name) {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBinaryProtocol.prototype.writeStructEnd"></a>[function <span class="apidocSignatureSpan">thrift.TBinaryProtocol.prototype.</span>writeStructEnd ()](#apidoc.element.thrift.TBinaryProtocol.prototype.writeStructEnd)
- description and source-code
```javascript
writeStructEnd = function () {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.TBufferedTransport"></a>[module thrift.TBufferedTransport](#apidoc.module.thrift.TBufferedTransport)

#### <a name="apidoc.element.thrift.TBufferedTransport.TBufferedTransport"></a>[function <span class="apidocSignatureSpan">thrift.</span>TBufferedTransport (buffer, callback)](#apidoc.element.thrift.TBufferedTransport.TBufferedTransport)
- description and source-code
```javascript
function TBufferedTransport(buffer, callback) {
  this.defaultReadBufferSize = 1024;
  this.writeBufferSize = 512; // Soft Limit
  this.inBuf = new Buffer(this.defaultReadBufferSize);
  this.readCursor = 0;
  this.writeCursor = 0; // for input buffer
  this.outBuffers = [];
  this.outCount = 0;
  this.onFlush = callback;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.receiver"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.</span>receiver (callback, seqid)](#apidoc.element.thrift.TBufferedTransport.receiver)
- description and source-code
```javascript
receiver = function (callback, seqid) {
  var reader = new TBufferedTransport();

  return function(data) {
    if (reader.writeCursor + data.length > reader.inBuf.length) {
      var buf = new Buffer(reader.writeCursor + data.length);
      reader.inBuf.copy(buf, 0, 0, reader.writeCursor);
      reader.inBuf = buf;
    }
    data.copy(reader.inBuf, reader.writeCursor, 0);
    reader.writeCursor += data.length;

    callback(reader, seqid);
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.TBufferedTransport.prototype"></a>[module thrift.TBufferedTransport.prototype](#apidoc.module.thrift.TBufferedTransport.prototype)

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.borrow"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>borrow ()](#apidoc.element.thrift.TBufferedTransport.prototype.borrow)
- description and source-code
```javascript
borrow = function () {
  var obj = {buf: this.inBuf, readIndex: this.readCursor, writeIndex: this.writeCursor};
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.close"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>close ()](#apidoc.element.thrift.TBufferedTransport.prototype.close)
- description and source-code
```javascript
close = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.commitPosition"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>commitPosition ()](#apidoc.element.thrift.TBufferedTransport.prototype.commitPosition)
- description and source-code
```javascript
commitPosition = function (){
  var unreadSize = this.writeCursor - this.readCursor;
  var bufSize = (unreadSize * 2 > this.defaultReadBufferSize) ?
    unreadSize * 2 : this.defaultReadBufferSize;
  var buf = new Buffer(bufSize);
  if (unreadSize > 0) {
    this.inBuf.copy(buf, 0, this.readCursor, this.writeCursor);
  }
  this.readCursor = 0;
  this.writeCursor = unreadSize;
  this.inBuf = buf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.consume"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>consume (bytesConsumed)](#apidoc.element.thrift.TBufferedTransport.prototype.consume)
- description and source-code
```javascript
consume = function (bytesConsumed) {
  this.readCursor += bytesConsumed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.ensureAvailable"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>ensureAvailable (len)](#apidoc.element.thrift.TBufferedTransport.prototype.ensureAvailable)
- description and source-code
```javascript
ensureAvailable = function (len) {
  if (this.readCursor + len > this.writeCursor) {
    throw new InputBufferUnderrunError();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.flush"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>flush ()](#apidoc.element.thrift.TBufferedTransport.prototype.flush)
- description and source-code
```javascript
flush = function () {
  // If the seqid of the callback is available pass it to the onFlush
  // Then remove the current seqid
  var seqid = this._seqid;
  this._seqid = null;

  if (this.outCount < 1) {
    return;
  }

  var msg = new Buffer(this.outCount),
      pos = 0;
  this.outBuffers.forEach(function(buf) {
    buf.copy(msg, pos, 0);
    pos += buf.length;
  });

  if (this.onFlush) {
    // Passing seqid through this call to get it to the connection
    this.onFlush(msg, seqid);
  }

  this.outBuffers = [];
  this.outCount = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.isOpen"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>isOpen ()](#apidoc.element.thrift.TBufferedTransport.prototype.isOpen)
- description and source-code
```javascript
isOpen = function () {
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.open"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>open ()](#apidoc.element.thrift.TBufferedTransport.prototype.open)
- description and source-code
```javascript
open = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.read"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>read (len)](#apidoc.element.thrift.TBufferedTransport.prototype.read)
- description and source-code
```javascript
read = function (len) {
  this.ensureAvailable(len);
  var buf = new Buffer(len);
  this.inBuf.copy(buf, 0, this.readCursor, this.readCursor + len);
  this.readCursor += len;
  return buf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.readByte"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>readByte ()](#apidoc.element.thrift.TBufferedTransport.prototype.readByte)
- description and source-code
```javascript
readByte = function () {
  this.ensureAvailable(1);
  return binary.readByte(this.inBuf[this.readCursor++]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.readDouble"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>readDouble ()](#apidoc.element.thrift.TBufferedTransport.prototype.readDouble)
- description and source-code
```javascript
readDouble = function () {
  this.ensureAvailable(8);
  var d = binary.readDouble(this.inBuf, this.readCursor);
  this.readCursor += 8;
  return d;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.readI16"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>readI16 ()](#apidoc.element.thrift.TBufferedTransport.prototype.readI16)
- description and source-code
```javascript
readI16 = function () {
  this.ensureAvailable(2);
  var i16 = binary.readI16(this.inBuf, this.readCursor);
  this.readCursor += 2;
  return i16;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.readI32"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>readI32 ()](#apidoc.element.thrift.TBufferedTransport.prototype.readI32)
- description and source-code
```javascript
readI32 = function () {
  this.ensureAvailable(4);
  var i32 = binary.readI32(this.inBuf, this.readCursor);
  this.readCursor += 4;
  return i32;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.readString"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>readString (len)](#apidoc.element.thrift.TBufferedTransport.prototype.readString)
- description and source-code
```javascript
readString = function (len) {
  this.ensureAvailable(len);
  var str = this.inBuf.toString('utf8', this.readCursor, this.readCursor + len);
  this.readCursor += len;
  return str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.rollbackPosition"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>rollbackPosition ()](#apidoc.element.thrift.TBufferedTransport.prototype.rollbackPosition)
- description and source-code
```javascript
rollbackPosition = function (){
  this.readCursor = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.setCurrSeqId"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>setCurrSeqId (seqid)](#apidoc.element.thrift.TBufferedTransport.prototype.setCurrSeqId)
- description and source-code
```javascript
setCurrSeqId = function (seqid) {
  this._seqid = seqid;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TBufferedTransport.prototype.write"></a>[function <span class="apidocSignatureSpan">thrift.TBufferedTransport.prototype.</span>write (buf)](#apidoc.element.thrift.TBufferedTransport.prototype.write)
- description and source-code
```javascript
write = function (buf) {
  if (typeof(buf) === "string") {
    buf = new Buffer(buf, 'utf8');
  }
  this.outBuffers.push(buf);
  this.outCount += buf.length;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.TCompactProtocol"></a>[module thrift.TCompactProtocol](#apidoc.module.thrift.TCompactProtocol)

#### <a name="apidoc.element.thrift.TCompactProtocol.TCompactProtocol"></a>[function <span class="apidocSignatureSpan">thrift.</span>TCompactProtocol (trans)](#apidoc.element.thrift.TCompactProtocol.TCompactProtocol)
- description and source-code
```javascript
function TCompactProtocol(trans) {
  this.trans = trans;
  this.lastField_ = [];
  this.lastFieldId_ = 0;
  this.string_limit_ = 0;
  this.string_buf_ = null;
  this.string_buf_size_ = 0;
  this.container_limit_ = 0;
  this.booleanField_ = {
    name: null,
    hasBoolValue: false
  };
  this.boolValue_ = {
    hasBoolValue: false,
    boolValue: false
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.TCompactProtocol.prototype"></a>[module thrift.TCompactProtocol.prototype](#apidoc.module.thrift.TCompactProtocol.prototype)

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.flush"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>flush ()](#apidoc.element.thrift.TCompactProtocol.prototype.flush)
- description and source-code
```javascript
flush = function () {
  return this.trans.flush();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.getCompactType"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>getCompactType (ttype)](#apidoc.element.thrift.TCompactProtocol.prototype.getCompactType)
- description and source-code
```javascript
getCompactType = function (ttype) {
  return TCompactProtocol.TTypeToCType[ttype];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.getTType"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>getTType (type)](#apidoc.element.thrift.TCompactProtocol.prototype.getTType)
- description and source-code
```javascript
getTType = function (type) {
  switch (type) {
    case Type.STOP:
      return Type.STOP;
    case TCompactProtocol.Types.CT_BOOLEAN_FALSE:
    case TCompactProtocol.Types.CT_BOOLEAN_TRUE:
      return Type.BOOL;
    case TCompactProtocol.Types.CT_BYTE:
      return Type.BYTE;
    case TCompactProtocol.Types.CT_I16:
      return Type.I16;
    case TCompactProtocol.Types.CT_I32:
      return Type.I32;
    case TCompactProtocol.Types.CT_I64:
      return Type.I64;
    case TCompactProtocol.Types.CT_DOUBLE:
      return Type.DOUBLE;
    case TCompactProtocol.Types.CT_BINARY:
      return Type.STRING;
    case TCompactProtocol.Types.CT_LIST:
      return Type.LIST;
    case TCompactProtocol.Types.CT_SET:
      return Type.SET;
    case TCompactProtocol.Types.CT_MAP:
      return Type.MAP;
    case TCompactProtocol.Types.CT_STRUCT:
      return Type.STRUCT;
    default:
      throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.INVALID_DATA, "Unknown type: " + type);
  }
  return Type.STOP;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.getTransport"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>getTransport ()](#apidoc.element.thrift.TCompactProtocol.prototype.getTransport)
- description and source-code
```javascript
getTransport = function () {
  return this.trans;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.i32ToZigzag"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>i32ToZigzag (n)](#apidoc.element.thrift.TCompactProtocol.prototype.i32ToZigzag)
- description and source-code
```javascript
i32ToZigzag = function (n) {
  return (n << 1) ^ ((n & 0x80000000) ? 0xFFFFFFFF : 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.i64ToZigzag"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>i64ToZigzag (l)](#apidoc.element.thrift.TCompactProtocol.prototype.i64ToZigzag)
- description and source-code
```javascript
i64ToZigzag = function (l) {
  if (typeof l === 'string') {
    l = new Int64(parseInt(l, 10));
  } else if (typeof l === 'number') {
    l = new Int64(l);
  }
  if (! (l instanceof Int64)) {
    throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.INVALID_DATA, "Expected Int64 or Number, found: " + l);
  }
  var hi = l.buffer.readUInt32BE(0, true);
  var lo = l.buffer.readUInt32BE(4, true);
  var sign = hi >>> 31;
  hi = ((hi << 1) | (lo >>> 31)) ^ ((!!sign) ? 0xFFFFFFFF : 0);
  lo = (lo << 1) ^ ((!!sign) ? 0xFFFFFFFF : 0);
  return new Int64(hi, lo);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readBinary"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readBinary ()](#apidoc.element.thrift.TCompactProtocol.prototype.readBinary)
- description and source-code
```javascript
readBinary = function () {
  var size = this.readVarint32();
  if (size === 0) {
    return new Buffer(0);
  }

  if (size < 0) {
    throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.NEGATIVE_SIZE, "Negative binary size");
  }
  return this.trans.read(size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readBool"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readBool ()](#apidoc.element.thrift.TCompactProtocol.prototype.readBool)
- description and source-code
```javascript
readBool = function () {
  var value = false;
  var rsize = 0;
  if (this.boolValue_.hasBoolValue === true) {
    value = this.boolValue_.boolValue;
    this.boolValue_.hasBoolValue = false;
  } else {
    var res = this.trans.readByte();
    rsize = res.rsize;
    value = (res.value == TCompactProtocol.Types.CT_BOOLEAN_TRUE);
  }
  return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readByte"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readByte ()](#apidoc.element.thrift.TCompactProtocol.prototype.readByte)
- description and source-code
```javascript
readByte = function () {
  return this.trans.readByte();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readDouble"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readDouble ()](#apidoc.element.thrift.TCompactProtocol.prototype.readDouble)
- description and source-code
```javascript
readDouble = function () {
  var buff = this.trans.read(8);
  var off = 0;

  var signed = buff[off + 7] & 0x80;
  var e = (buff[off+6] & 0xF0) >> 4;
  e += (buff[off+7] & 0x7F) << 4;

  var m = buff[off];
  m += buff[off+1] << 8;
  m += buff[off+2] << 16;
  m += buff[off+3] * POW_24;
  m += buff[off+4] * POW_32;
  m += buff[off+5] * POW_40;
  m += (buff[off+6] & 0x0F) * POW_48;

  switch (e) {
    case 0:
      e = -1022;
      break;
    case 2047:
      return m ? NaN : (signed ? -Infinity : Infinity);
    default:
      m += POW_52;
      e -= 1023;
  }

  if (signed) {
    m *= -1;
  }

  return m * Math.pow(2, e - 52);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readFieldBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readFieldBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readFieldBegin)
- description and source-code
```javascript
readFieldBegin = function () {
  var fieldId = 0;
  var b = this.trans.readByte(b);
  var type = (b & 0x0f);

  if (type == TCompactProtocol.Types.CT_STOP) {
    return {fname: null, ftype: Thrift.Type.STOP, fid: 0};
  }

  //Mask off the 4 MSB of the type header to check for field id delta.
  var modifier = ((b & 0x000000f0) >>> 4);
  if (modifier === 0) {
    //If not a delta read the field id.
    fieldId = this.readI16();
  } else {
    //Recover the field id from the delta
    fieldId = (this.lastFieldId_ + modifier);
  }
  var fieldType = this.getTType(type);

  //Boolean are encoded with the type
  if (type == TCompactProtocol.Types.CT_BOOLEAN_TRUE ||
      type == TCompactProtocol.Types.CT_BOOLEAN_FALSE) {
    this.boolValue_.hasBoolValue = true;
    this.boolValue_.boolValue =
      (type == TCompactProtocol.Types.CT_BOOLEAN_TRUE ? true : false);
  }

  //Save the new field for the next delta computation.
  this.lastFieldId_ = fieldId;
  return {fname: null, ftype: fieldType, fid: fieldId};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readFieldEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readFieldEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readFieldEnd)
- description and source-code
```javascript
readFieldEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readI16"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readI16 ()](#apidoc.element.thrift.TCompactProtocol.prototype.readI16)
- description and source-code
```javascript
readI16 = function () {
  return this.readI32();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readI32"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readI32 ()](#apidoc.element.thrift.TCompactProtocol.prototype.readI32)
- description and source-code
```javascript
readI32 = function () {
  return this.zigzagToI32(this.readVarint32());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readI64"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readI64 ()](#apidoc.element.thrift.TCompactProtocol.prototype.readI64)
- description and source-code
```javascript
readI64 = function () {
  return this.zigzagToI64(this.readVarint64());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readListBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readListBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readListBegin)
- description and source-code
```javascript
readListBegin = function () {
  var size_and_type = this.trans.readByte();

  var lsize = (size_and_type >>> 4) & 0x0000000f;
  if (lsize == 15) {
    lsize = this.readVarint32();
  }

  if (lsize < 0) {
    throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.NEGATIVE_SIZE, "Negative list size");
  }

  var elemType = this.getTType(size_and_type & 0x0000000f);

  return {etype: elemType, size: lsize};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readListEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readListEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readListEnd)
- description and source-code
```javascript
readListEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readMapBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readMapBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readMapBegin)
- description and source-code
```javascript
readMapBegin = function () {
  var msize = this.readVarint32();
  if (msize < 0) {
    throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.NEGATIVE_SIZE, "Negative map size");
  }

  var kvType = 0;
  if (msize !== 0) {
    kvType = this.trans.readByte();
  }

  var keyType = this.getTType((kvType & 0xf0) >>> 4);
  var valType = this.getTType(kvType & 0xf);
  return {ktype: keyType, vtype: valType, size: msize};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readMapEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readMapEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readMapEnd)
- description and source-code
```javascript
readMapEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readMessageBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readMessageBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readMessageBegin)
- description and source-code
```javascript
readMessageBegin = function () {
  //Read protocol ID
  var protocolId = this.trans.readByte();
  if (protocolId != TCompactProtocol.PROTOCOL_ID) {
    throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.BAD_VERSION, "Bad protocol identifier " + protocolId);
  }

  //Read Version and Type
  var versionAndType = this.trans.readByte();
  var version = (versionAndType & TCompactProtocol.VERSION_MASK);
  if (version != TCompactProtocol.VERSION_N) {
    throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.BAD_VERSION, "Bad protocol version " + version);
  }
  var type = ((versionAndType >> TCompactProtocol.TYPE_SHIFT_AMOUNT) & TCompactProtocol.TYPE_BITS);

  //Read SeqId
  var seqid = this.readVarint32();

  //Read name
  var name = this.readString();

  return {fname: name, mtype: type, rseqid: seqid};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readMessageEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readMessageEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readMessageEnd)
- description and source-code
```javascript
readMessageEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readSetBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readSetBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readSetBegin)
- description and source-code
```javascript
readSetBegin = function () {
  return this.readListBegin();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readSetEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readSetEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readSetEnd)
- description and source-code
```javascript
readSetEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readString"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readString ()](#apidoc.element.thrift.TCompactProtocol.prototype.readString)
- description and source-code
```javascript
readString = function () {
  var size = this.readVarint32();
  // Catch empty string case
  if (size === 0) {
    return "";
  }

  // Catch error cases
  if (size < 0) {
    throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.NEGATIVE_SIZE, "Negative string size");
  }
  return this.trans.readString(size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readStructBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readStructBegin ()](#apidoc.element.thrift.TCompactProtocol.prototype.readStructBegin)
- description and source-code
```javascript
readStructBegin = function () {
  this.lastField_.push(this.lastFieldId_);
  this.lastFieldId_ = 0;
  return {fname: ''};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readStructEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readStructEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.readStructEnd)
- description and source-code
```javascript
readStructEnd = function () {
  this.lastFieldId_ = this.lastField_.pop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readVarint32"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readVarint32 ()](#apidoc.element.thrift.TCompactProtocol.prototype.readVarint32)
- description and source-code
```javascript
readVarint32 = function () {
  return this.readVarint64().toNumber();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.readVarint64"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>readVarint64 ()](#apidoc.element.thrift.TCompactProtocol.prototype.readVarint64)
- description and source-code
```javascript
readVarint64 = function () {
  var rsize = 0;
  var lo = 0;
  var hi = 0;
  var shift = 0;
  while (true) {
    var b = this.trans.readByte();
    rsize ++;
    if (shift <= 25) {
      lo = lo | ((b & 0x7f) << shift);
    } else if (25 < shift && shift < 32) {
      lo = lo | ((b & 0x7f) << shift);
      hi = hi | ((b & 0x7f) >>> (32-shift));
    } else {
      hi = hi | ((b & 0x7f) << (shift-32));
    }
    shift += 7;
    if (!(b & 0x80)) {
      break;
    }
    if (rsize >= 10) {
      throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.INVALID_DATA, "Variable-length int over 10 bytes.");
    }
  }
  return new Int64(hi, lo);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.skip"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>skip (type)](#apidoc.element.thrift.TCompactProtocol.prototype.skip)
- description and source-code
```javascript
skip = function (type) {
  switch (type) {
    case Type.STOP:
      return;
    case Type.BOOL:
      this.readBool();
      break;
    case Type.BYTE:
      this.readByte();
      break;
    case Type.I16:
      this.readI16();
      break;
    case Type.I32:
      this.readI32();
      break;
    case Type.I64:
      this.readI64();
      break;
    case Type.DOUBLE:
      this.readDouble();
      break;
    case Type.STRING:
      this.readString();
      break;
    case Type.STRUCT:
      this.readStructBegin();
      while (true) {
        var r = this.readFieldBegin();
        if (r.ftype === Type.STOP) {
          break;
        }
        this.skip(r.ftype);
        this.readFieldEnd();
      }
      this.readStructEnd();
      break;
    case Type.MAP:
      var mapBegin = this.readMapBegin();
      for (var i = 0; i < mapBegin.size; ++i) {
        this.skip(mapBegin.ktype);
        this.skip(mapBegin.vtype);
      }
      this.readMapEnd();
      break;
    case Type.SET:
      var setBegin = this.readSetBegin();
      for (var i2 = 0; i2 < setBegin.size; ++i2) {
        this.skip(setBegin.etype);
      }
      this.readSetEnd();
      break;
    case Type.LIST:
      var listBegin = this.readListBegin();
      for (var i3 = 0; i3 < listBegin.size; ++i3) {
        this.skip(listBegin.etype);
      }
      this.readListEnd();
      break;
    default:
      throw new  Error("Invalid type: " + type);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeBinary"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeBinary (arg)](#apidoc.element.thrift.TCompactProtocol.prototype.writeBinary)
- description and source-code
```javascript
writeBinary = function (arg) {
  this.writeStringOrBinary('writeBinary', 'binary', arg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeBool"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeBool (value)](#apidoc.element.thrift.TCompactProtocol.prototype.writeBool)
- description and source-code
```javascript
writeBool = function (value) {
  if (this.booleanField_.name !== null) {
    // we haven't written the field header yet
    this.writeFieldBeginInternal(this.booleanField_.name,
                                 this.booleanField_.fieldType,
                                 this.booleanField_.fieldId,
                                 (value ? TCompactProtocol.Types.CT_BOOLEAN_TRUE
                                          : TCompactProtocol.Types.CT_BOOLEAN_FALSE));
    this.booleanField_.name = null;
  } else {
    // we're not part of a field, so just write the value
    this.writeByte((value ? TCompactProtocol.Types.CT_BOOLEAN_TRUE
                            : TCompactProtocol.Types.CT_BOOLEAN_FALSE));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeByte"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeByte (b)](#apidoc.element.thrift.TCompactProtocol.prototype.writeByte)
- description and source-code
```javascript
writeByte = function (b) {
  this.trans.write(new Buffer([b]));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeCollectionBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeCollectionBegin (elemType, size)](#apidoc.element.thrift.TCompactProtocol.prototype.writeCollectionBegin)
- description and source-code
```javascript
writeCollectionBegin = function (elemType, size) {
  if (size <= 14) {
    //Combine size and type in one byte if possible
    this.writeByte(size << 4 | this.getCompactType(elemType));
  } else {
    this.writeByte(0xf0 | this.getCompactType(elemType));
    this.writeVarint32(size);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeDouble"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeDouble (v)](#apidoc.element.thrift.TCompactProtocol.prototype.writeDouble)
- description and source-code
```javascript
writeDouble = function (v) {
  var buff = new Buffer(8);
  var m, e, c;

  buff[7] = (v < 0 ? 0x80 : 0x00);

  v = Math.abs(v);
  if (v !== v) {
    // NaN, use QNaN IEEE format
    m = 2251799813685248;
    e = 2047;
  } else if (v === Infinity) {
    m = 0;
    e = 2047;
  } else {
    e = Math.floor(Math.log(v) / Math.LN2);
    c = Math.pow(2, -e);
    if (v * c < 1) {
      e--;
      c *= 2;
    }

    if (e + 1023 >= 2047)
    {
      // Overflow
      m = 0;
      e = 2047;
    }
    else if (e + 1023 >= 1)
    {
      // Normalized - term order matters, as Math.pow(2, 52-e) and v*Math.pow(2, 52) can overflow
      m = (v*c-1) * POW_52;
      e += 1023;
    }
    else
    {
      // Denormalized - also catches the '0' case, somewhat by chance
      m = (v * POW_1022) * POW_52;
      e = 0;
    }
  }

  buff[6] = (e << 4) & 0xf0;
  buff[7] |= (e >> 4) & 0x7f;

  buff[0] = m & 0xff;
  m = Math.floor(m / POW_8);
  buff[1] = m & 0xff;
  m = Math.floor(m / POW_8);
  buff[2] = m & 0xff;
  m = Math.floor(m / POW_8);
  buff[3] = m & 0xff;
  m >>= 8;
  buff[4] = m & 0xff;
  m >>= 8;
  buff[5] = m & 0xff;
  m >>= 8;
  buff[6] |= m & 0x0f;

  this.trans.write(buff);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeFieldBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeFieldBegin (name, type, id)](#apidoc.element.thrift.TCompactProtocol.prototype.writeFieldBegin)
- description and source-code
```javascript
writeFieldBegin = function (name, type, id) {
  if (type != Type.BOOL) {
    return this.writeFieldBeginInternal(name, type, id, -1);
  }

  this.booleanField_.name = name;
  this.booleanField_.fieldType = type;
  this.booleanField_.fieldId = id;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeFieldBeginInternal"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeFieldBeginInternal (name, fieldType, fieldId, typeOverride)](#apidoc.element.thrift.TCompactProtocol.prototype.writeFieldBeginInternal)
- description and source-code
```javascript
writeFieldBeginInternal = function (name, fieldType, fieldId, typeOverride) {
  //If there's a type override, use that.
  var typeToWrite = (typeOverride == -1 ? this.getCompactType(fieldType) : typeOverride);
  //Check if we can delta encode the field id
  if (fieldId > this.lastFieldId_ && fieldId - this.lastFieldId_ <= 15) {
    //Include the type delta with the field ID
    this.writeByte((fieldId - this.lastFieldId_) << 4 | typeToWrite);
  } else {
    //Write separate type and ID values
    this.writeByte(typeToWrite);
    this.writeI16(fieldId);
  }
  this.lastFieldId_ = fieldId;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeFieldEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeFieldEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeFieldEnd)
- description and source-code
```javascript
writeFieldEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeFieldStop"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeFieldStop ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeFieldStop)
- description and source-code
```javascript
writeFieldStop = function () {
  this.writeByte(TCompactProtocol.Types.CT_STOP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeI16"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeI16 (i16)](#apidoc.element.thrift.TCompactProtocol.prototype.writeI16)
- description and source-code
```javascript
writeI16 = function (i16) {
  this.writeVarint32(this.i32ToZigzag(i16));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeI32"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeI32 (i32)](#apidoc.element.thrift.TCompactProtocol.prototype.writeI32)
- description and source-code
```javascript
writeI32 = function (i32) {
  this.writeVarint32(this.i32ToZigzag(i32));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeI64"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeI64 (i64)](#apidoc.element.thrift.TCompactProtocol.prototype.writeI64)
- description and source-code
```javascript
writeI64 = function (i64) {
  this.writeVarint64(this.i64ToZigzag(i64));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeListBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeListBegin (elemType, size)](#apidoc.element.thrift.TCompactProtocol.prototype.writeListBegin)
- description and source-code
```javascript
writeListBegin = function (elemType, size) {
  this.writeCollectionBegin(elemType, size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeListEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeListEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeListEnd)
- description and source-code
```javascript
writeListEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeMapBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeMapBegin (keyType, valType, size)](#apidoc.element.thrift.TCompactProtocol.prototype.writeMapBegin)
- description and source-code
```javascript
writeMapBegin = function (keyType, valType, size) {
  if (size === 0) {
    this.writeByte(0);
  } else {
    this.writeVarint32(size);
    this.writeByte(this.getCompactType(keyType) << 4 | this.getCompactType(valType));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeMapEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeMapEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeMapEnd)
- description and source-code
```javascript
writeMapEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeMessageBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeMessageBegin (name, type, seqid)](#apidoc.element.thrift.TCompactProtocol.prototype.writeMessageBegin)
- description and source-code
```javascript
writeMessageBegin = function (name, type, seqid) {
  this.writeByte(TCompactProtocol.PROTOCOL_ID);
  this.writeByte((TCompactProtocol.VERSION_N & TCompactProtocol.VERSION_MASK) |
                     ((type << TCompactProtocol.TYPE_SHIFT_AMOUNT) & TCompactProtocol.TYPE_MASK));
  this.writeVarint32(seqid);
  this.writeString(name);

  // Record client seqid to find callback again
  if (this._seqid) {
    // TODO better logging log warning
    log.warning('SeqId already set', { 'name': name });
  } else {
    this._seqid = seqid;
    this.trans.setCurrSeqId(seqid);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeMessageEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeMessageEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeMessageEnd)
- description and source-code
```javascript
writeMessageEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeSetBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeSetBegin (elemType, size)](#apidoc.element.thrift.TCompactProtocol.prototype.writeSetBegin)
- description and source-code
```javascript
writeSetBegin = function (elemType, size) {
  this.writeCollectionBegin(elemType, size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeSetEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeSetEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeSetEnd)
- description and source-code
```javascript
writeSetEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeString"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeString (arg)](#apidoc.element.thrift.TCompactProtocol.prototype.writeString)
- description and source-code
```javascript
writeString = function (arg) {
  this.writeStringOrBinary('writeString', 'utf8', arg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeStringOrBinary"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeStringOrBinary (name, encoding, arg)](#apidoc.element.thrift.TCompactProtocol.prototype.writeStringOrBinary)
- description and source-code
```javascript
writeStringOrBinary = function (name, encoding, arg) {
  if (typeof arg === 'string') {
    this.writeVarint32(Buffer.byteLength(arg, encoding)) ;
    this.trans.write(new Buffer(arg, encoding));
  } else if (arg instanceof Buffer ||
             Object.prototype.toString.call(arg) == '[object Uint8Array]') {
    // Buffers in Node.js under Browserify may extend UInt8Array instead of
    // defining a new object. We detect them here so we can write them
    // correctly
    this.writeVarint32(arg.length);
    this.trans.write(arg);
  } else {
    throw new Error(name + ' called without a string/Buffer argument: ' + arg);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeStructBegin"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeStructBegin (name)](#apidoc.element.thrift.TCompactProtocol.prototype.writeStructBegin)
- description and source-code
```javascript
writeStructBegin = function (name) {
  this.lastField_.push(this.lastFieldId_);
  this.lastFieldId_ = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeStructEnd"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeStructEnd ()](#apidoc.element.thrift.TCompactProtocol.prototype.writeStructEnd)
- description and source-code
```javascript
writeStructEnd = function () {
  this.lastFieldId_ = this.lastField_.pop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeVarint32"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeVarint32 (n)](#apidoc.element.thrift.TCompactProtocol.prototype.writeVarint32)
- description and source-code
```javascript
writeVarint32 = function (n) {
  var buf = new Buffer(5);
  var wsize = 0;
  while (true) {
    if ((n & ~0x7F) === 0) {
      buf[wsize++] = n;
      break;
    } else {
      buf[wsize++] = ((n & 0x7F) | 0x80);
      n = n >>> 7;
    }
  }
  var wbuf = new Buffer(wsize);
  buf.copy(wbuf,0,0,wsize);
  this.trans.write(wbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.writeVarint64"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>writeVarint64 (n)](#apidoc.element.thrift.TCompactProtocol.prototype.writeVarint64)
- description and source-code
```javascript
writeVarint64 = function (n) {
  if (typeof n === "number"){
    n = new Int64(n);
  }
  if (! (n instanceof Int64)) {
    throw new Thrift.TProtocolException(Thrift.TProtocolExceptionType.INVALID_DATA, "Expected Int64 or Number, found: " + n);
  }

  var buf = new Buffer(10);
  var wsize = 0;
  var hi = n.buffer.readUInt32BE(0, true);
  var lo = n.buffer.readUInt32BE(4, true);
  var mask = 0;
  while (true) {
    if (((lo & ~0x7F) === 0) && (hi === 0)) {
      buf[wsize++] = lo;
      break;
    } else {
      buf[wsize++] = ((lo & 0x7F) | 0x80);
      mask = hi << 25;
      lo = lo >>> 7;
      hi = hi >>> 7;
      lo = lo | mask;
    }
  }
  var wbuf = new Buffer(wsize);
  buf.copy(wbuf,0,0,wsize);
  this.trans.write(wbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.zigzagToI32"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>zigzagToI32 (n)](#apidoc.element.thrift.TCompactProtocol.prototype.zigzagToI32)
- description and source-code
```javascript
zigzagToI32 = function (n) {
  return (n >>> 1) ^ (-1 * (n & 1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TCompactProtocol.prototype.zigzagToI64"></a>[function <span class="apidocSignatureSpan">thrift.TCompactProtocol.prototype.</span>zigzagToI64 (n)](#apidoc.element.thrift.TCompactProtocol.prototype.zigzagToI64)
- description and source-code
```javascript
zigzagToI64 = function (n) {
  var hi = n.buffer.readUInt32BE(0, true);
  var lo = n.buffer.readUInt32BE(4, true);

  var neg = new Int64(hi & 0, lo & 1);
  neg._2scomp();
  var hi_neg = neg.buffer.readUInt32BE(0, true);
  var lo_neg = neg.buffer.readUInt32BE(4, true);

  var hi_lo = (hi << 31);
  hi = (hi >>> 1) ^ (hi_neg);
  lo = ((lo >>> 1) | hi_lo) ^ (lo_neg);
  return new Int64(hi, lo);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.TFramedTransport"></a>[module thrift.TFramedTransport](#apidoc.module.thrift.TFramedTransport)

#### <a name="apidoc.element.thrift.TFramedTransport.TFramedTransport"></a>[function <span class="apidocSignatureSpan">thrift.</span>TFramedTransport (buffer, callback)](#apidoc.element.thrift.TFramedTransport.TFramedTransport)
- description and source-code
```javascript
function TFramedTransport(buffer, callback) {
  this.inBuf = buffer || new Buffer(0);
  this.outBuffers = [];
  this.outCount = 0;
  this.readPos = 0;
  this.onFlush = callback;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.receiver"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.</span>receiver (callback, seqid)](#apidoc.element.thrift.TFramedTransport.receiver)
- description and source-code
```javascript
receiver = function (callback, seqid) {
  var residual = null;

  return function(data) {
    // Prepend any residual data from our previous read
    if (residual) {
      data = Buffer.concat([residual, data]);
      residual = null;
    }

    // framed transport
    while (data.length) {
      if (data.length < 4) {
        // Not enough bytes to continue, save and resume on next packet
        residual = data;
        return;
      }
      var frameSize = binary.readI32(data, 0);
      if (data.length < 4 + frameSize) {
        // Not enough bytes to continue, save and resume on next packet
        residual = data;
        return;
      }

      var frame = data.slice(4, 4 + frameSize);
      residual = data.slice(4 + frameSize);

      callback(new TFramedTransport(frame), seqid);

      data = residual;
      residual = null;
    }
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.TFramedTransport.prototype"></a>[module thrift.TFramedTransport.prototype](#apidoc.module.thrift.TFramedTransport.prototype)

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.borrow"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>borrow ()](#apidoc.element.thrift.TFramedTransport.prototype.borrow)
- description and source-code
```javascript
borrow = function () {
  return {
    buf: this.inBuf,
    readIndex: this.readPos,
    writeIndex: this.inBuf.length
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.close"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>close ()](#apidoc.element.thrift.TFramedTransport.prototype.close)
- description and source-code
```javascript
close = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.commitPosition"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>commitPosition ()](#apidoc.element.thrift.TFramedTransport.prototype.commitPosition)
- description and source-code
```javascript
commitPosition = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.consume"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>consume (bytesConsumed)](#apidoc.element.thrift.TFramedTransport.prototype.consume)
- description and source-code
```javascript
consume = function (bytesConsumed) {
  this.readPos += bytesConsumed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.ensureAvailable"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>ensureAvailable (len)](#apidoc.element.thrift.TFramedTransport.prototype.ensureAvailable)
- description and source-code
```javascript
ensureAvailable = function (len) {
  if (this.readPos + len > this.inBuf.length) {
    throw new InputBufferUnderrunError();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.flush"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>flush ()](#apidoc.element.thrift.TFramedTransport.prototype.flush)
- description and source-code
```javascript
flush = function () {
  // If the seqid of the callback is available pass it to the onFlush
  // Then remove the current seqid
  var seqid = this._seqid;
  this._seqid = null;

  var out = new Buffer(this.outCount),
      pos = 0;
  this.outBuffers.forEach(function(buf) {
    buf.copy(out, pos, 0);
    pos += buf.length;
  });

  if (this.onFlush) {
    // TODO: optimize this better, allocate one buffer instead of both:
    var msg = new Buffer(out.length + 4);
    binary.writeI32(msg, out.length);
    out.copy(msg, 4, 0, out.length);
    if (this.onFlush) {
      // Passing seqid through this call to get it to the connection
      this.onFlush(msg, seqid);
    }
  }

  this.outBuffers = [];
  this.outCount = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.isOpen"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>isOpen ()](#apidoc.element.thrift.TFramedTransport.prototype.isOpen)
- description and source-code
```javascript
isOpen = function () {
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.open"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>open ()](#apidoc.element.thrift.TFramedTransport.prototype.open)
- description and source-code
```javascript
open = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.read"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>read (len)](#apidoc.element.thrift.TFramedTransport.prototype.read)
- description and source-code
```javascript
read = function (len) { // this function will be used for each frames.
  this.ensureAvailable(len);
  var end = this.readPos + len;

  if (this.inBuf.length < end) {
    throw new Error('read(' + len + ') failed - not enough data');
  }

  var buf = this.inBuf.slice(this.readPos, end);
  this.readPos = end;
  return buf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.readByte"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>readByte ()](#apidoc.element.thrift.TFramedTransport.prototype.readByte)
- description and source-code
```javascript
readByte = function () {
  this.ensureAvailable(1);
  return binary.readByte(this.inBuf[this.readPos++]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.readDouble"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>readDouble ()](#apidoc.element.thrift.TFramedTransport.prototype.readDouble)
- description and source-code
```javascript
readDouble = function () {
  this.ensureAvailable(8);
  var d = binary.readDouble(this.inBuf, this.readPos);
  this.readPos += 8;
  return d;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.readI16"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>readI16 ()](#apidoc.element.thrift.TFramedTransport.prototype.readI16)
- description and source-code
```javascript
readI16 = function () {
  this.ensureAvailable(2);
  var i16 = binary.readI16(this.inBuf, this.readPos);
  this.readPos += 2;
  return i16;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.readI32"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>readI32 ()](#apidoc.element.thrift.TFramedTransport.prototype.readI32)
- description and source-code
```javascript
readI32 = function () {
  this.ensureAvailable(4);
  var i32 = binary.readI32(this.inBuf, this.readPos);
  this.readPos += 4;
  return i32;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.readString"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>readString (len)](#apidoc.element.thrift.TFramedTransport.prototype.readString)
- description and source-code
```javascript
readString = function (len) {
  this.ensureAvailable(len);
  var str = this.inBuf.toString('utf8', this.readPos, this.readPos + len);
  this.readPos += len;
  return str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.rollbackPosition"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>rollbackPosition ()](#apidoc.element.thrift.TFramedTransport.prototype.rollbackPosition)
- description and source-code
```javascript
rollbackPosition = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.setCurrSeqId"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>setCurrSeqId (seqid)](#apidoc.element.thrift.TFramedTransport.prototype.setCurrSeqId)
- description and source-code
```javascript
setCurrSeqId = function (seqid) {
  this._seqid = seqid;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TFramedTransport.prototype.write"></a>[function <span class="apidocSignatureSpan">thrift.TFramedTransport.prototype.</span>write (buf, encoding)](#apidoc.element.thrift.TFramedTransport.prototype.write)
- description and source-code
```javascript
write = function (buf, encoding) {
  if (typeof(buf) === "string") {
    buf = new Buffer(buf, encoding || 'utf8');
  }
  this.outBuffers.push(buf);
  this.outCount += buf.length;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.TJSONProtocol"></a>[module thrift.TJSONProtocol](#apidoc.module.thrift.TJSONProtocol)

#### <a name="apidoc.element.thrift.TJSONProtocol.TJSONProtocol"></a>[function <span class="apidocSignatureSpan">thrift.</span>TJSONProtocol (trans)](#apidoc.element.thrift.TJSONProtocol.TJSONProtocol)
- description and source-code
```javascript
function TJSONProtocol(trans) {
  this.tstack = [];
  this.tpos = [];
  this.trans = trans;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.TJSONProtocol.prototype"></a>[module thrift.TJSONProtocol.prototype](#apidoc.module.thrift.TJSONProtocol.prototype)

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.flush"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>flush ()](#apidoc.element.thrift.TJSONProtocol.prototype.flush)
- description and source-code
```javascript
flush = function () {
  this.writeToTransportIfStackIsFlushable();
  return this.trans.flush();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.getTransport"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>getTransport ()](#apidoc.element.thrift.TJSONProtocol.prototype.getTransport)
- description and source-code
```javascript
getTransport = function () {
  return this.trans;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readBinary"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readBinary ()](#apidoc.element.thrift.TJSONProtocol.prototype.readBinary)
- description and source-code
```javascript
readBinary = function () {
  return new Buffer(this.readValue(), 'base64');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readBool"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readBool ()](#apidoc.element.thrift.TJSONProtocol.prototype.readBool)
- description and source-code
```javascript
readBool = function () {
  return this.readValue() == '1';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readByte"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readByte ()](#apidoc.element.thrift.TJSONProtocol.prototype.readByte)
- description and source-code
```javascript
readByte = function () {
  return this.readI32();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readDouble"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readDouble ()](#apidoc.element.thrift.TJSONProtocol.prototype.readDouble)
- description and source-code
```javascript
readDouble = function () {
  return this.readI32();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readFieldBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readFieldBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readFieldBegin)
- description and source-code
```javascript
readFieldBegin = function () {
  var r = {};

  var fid = -1;
  var ftype = Type.STOP;

  //get a fieldId
  for (var f in (this.rstack[this.rstack.length - 1])) {
    if (f === null) {
      continue;
    }

    fid = parseInt(f, 10);
    this.rpos.push(this.rstack.length);

    var field = this.rstack[this.rstack.length - 1][fid];

    //remove so we don't see it again
    delete this.rstack[this.rstack.length - 1][fid];

    this.rstack.push(field);

    break;
  }

  if (fid != -1) {
    //should only be 1 of these but this is the only
    //way to match a key
    for (var i in (this.rstack[this.rstack.length - 1])) {
      if (TJSONProtocol.RType[i] === null) {
        continue;
      }

      ftype = TJSONProtocol.RType[i];
      this.rstack[this.rstack.length - 1] = this.rstack[this.rstack.length - 1][i];
    }
  }

  r.fname = '';
  r.ftype = ftype;
  r.fid = fid;

  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readFieldEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readFieldEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readFieldEnd)
- description and source-code
```javascript
readFieldEnd = function () {
  var pos = this.rpos.pop();

  //get back to the right place in the stack
  while (this.rstack.length > pos) {
    this.rstack.pop();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readI16"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readI16 ()](#apidoc.element.thrift.TJSONProtocol.prototype.readI16)
- description and source-code
```javascript
readI16 = function () {
  return this.readI32();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readI32"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readI32 (f)](#apidoc.element.thrift.TJSONProtocol.prototype.readI32)
- description and source-code
```javascript
readI32 = function (f) {
  return +this.readValue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readI64"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readI64 ()](#apidoc.element.thrift.TJSONProtocol.prototype.readI64)
- description and source-code
```javascript
readI64 = function () {
  var n = this.readValue()
  if (typeof n === 'string') {
    // Assuming no one is sending in 1.11111e+33 format
    return Int64Util.fromDecimalString(n);
  } else {
    return new Int64(n);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readListBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readListBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readListBegin)
- description and source-code
```javascript
readListBegin = function () {
  var list = this.rstack[this.rstack.length - 1];

  var r = {};
  r.etype = TJSONProtocol.RType[list.shift()];
  r.size = list.shift();

  this.rpos.push(this.rstack.length);
  this.rstack.push(list.shift());

  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readListEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readListEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readListEnd)
- description and source-code
```javascript
readListEnd = function () {
  var pos = this.rpos.pop() - 2;
  var st = this.rstack;
  st.pop();
  if (st instanceof Array && st.length > pos && st[pos].length > 0) {
    st.push(st[pos].shift());
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readMapBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readMapBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readMapBegin)
- description and source-code
```javascript
readMapBegin = function () {
  var map = this.rstack.pop();
  var first = map.shift();
  if (first instanceof Array) {
    this.rstack.push(map);
    map = first;
    first = map.shift();
  }

  var r = {};
  r.ktype = TJSONProtocol.RType[first];
  r.vtype = TJSONProtocol.RType[map.shift()];
  r.size = map.shift();


  this.rpos.push(this.rstack.length);
  this.rstack.push(map.shift());

  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readMapEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readMapEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readMapEnd)
- description and source-code
```javascript
readMapEnd = function () {
  this.readFieldEnd();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readMessageBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readMessageBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readMessageBegin)
- description and source-code
```javascript
readMessageBegin = function () {
  this.rstack = [];
  this.rpos = [];

  //Borrow the inbound transport buffer and ensure data is present/consistent
  var transBuf = this.trans.borrow();
  if (transBuf.readIndex >= transBuf.writeIndex) {
    throw new InputBufferUnderrunError();
  }
  var cursor = transBuf.readIndex;

  if (transBuf.buf[cursor] !== 0x5B) { //[
    throw new Error("Malformed JSON input, no opening bracket");
  }

  //Parse a single message (there may be several in the buffer)
  //  TODO: Handle characters using multiple code units
  cursor++;
  var openBracketCount = 1;
  var inString = false;
  for (; cursor < transBuf.writeIndex; cursor++) {
    var chr = transBuf.buf[cursor];
    //we use hexa charcode here because data[i] returns an int and not a char
    if (inString) {
      if (chr === 0x22) { //"
        inString = false;
      } else if (chr === 0x5C) { //\
        //escaped character, skip
        cursor += 1;
      }
    } else {
      if (chr === 0x5B) { //[
        openBracketCount += 1;
      } else if (chr === 0x5D) { //]
        openBracketCount -= 1;
        if (openBracketCount === 0) {
          //end of json message detected
          break;
        }
      } else if (chr === 0x22) { //"
        inString = true;
      }
    }
  }

  if (openBracketCount !== 0) {
    // Missing closing bracket. Can be buffer underrun.
    throw new InputBufferUnderrunError();
  }

  //Reconstitute the JSON object and conume the necessary bytes
  this.robj = json_parse(transBuf.buf.slice(transBuf.readIndex, cursor+1).toString());
  this.trans.consume(cursor + 1 - transBuf.readIndex);

  //Verify the protocol version
  var version = this.robj.shift();
  if (version != TJSONProtocol.Version) {
    throw new Error('Wrong thrift protocol version: ' + version);
  }

  //Objectify the thrift message {name/type/sequence-number} for return
  // and then save the JSON object in rstack
  var r = {};
  r.fname = this.robj.shift();
  r.mtype = this.robj.shift();
  r.rseqid = this.robj.shift();
  this.rstack.push(this.robj.shift());
  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readMessageEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readMessageEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readMessageEnd)
- description and source-code
```javascript
readMessageEnd = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readSetBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readSetBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readSetBegin)
- description and source-code
```javascript
readSetBegin = function () {
  return this.readListBegin();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readSetEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readSetEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readSetEnd)
- description and source-code
```javascript
readSetEnd = function () {
  return this.readListEnd();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readString"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readString ()](#apidoc.element.thrift.TJSONProtocol.prototype.readString)
- description and source-code
```javascript
readString = function () {
  return this.readValue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readStructBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readStructBegin ()](#apidoc.element.thrift.TJSONProtocol.prototype.readStructBegin)
- description and source-code
```javascript
readStructBegin = function () {
  var r = {};
  r.fname = '';

  //incase this is an array of structs
  if (this.rstack[this.rstack.length - 1] instanceof Array) {
    this.rstack.push(this.rstack[this.rstack.length - 1].shift());
  }

  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readStructEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readStructEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.readStructEnd)
- description and source-code
```javascript
readStructEnd = function () {
  this.rstack.pop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.readValue"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>readValue (f)](#apidoc.element.thrift.TJSONProtocol.prototype.readValue)
- description and source-code
```javascript
readValue = function (f) {
  if (f === undefined) {
    f = this.rstack[this.rstack.length - 1];
  }

  var r = {};

  if (f instanceof Array) {
    if (f.length === 0) {
      r.value = undefined;
    } else {
      r.value = f.shift();
    }
  } else if (!(f instanceof Int64) && f instanceof Object) {
    for (var i in f) {
      if (i === null) {
        continue;
      }
      this.rstack.push(f[i]);
      delete f[i];

      r.value = i;
      break;
    }
  } else {
    r.value = f;
    this.rstack.pop();
  }

  return r.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.skip"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>skip (type)](#apidoc.element.thrift.TJSONProtocol.prototype.skip)
- description and source-code
```javascript
skip = function (type) {
  throw new Error('skip not supported yet');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeBinary"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeBinary (arg)](#apidoc.element.thrift.TJSONProtocol.prototype.writeBinary)
- description and source-code
```javascript
writeBinary = function (arg) {
  if (typeof arg === 'string') {
    var buf = new Buffer(arg, 'binary');
  } else if (arg instanceof Buffer ||
             Object.prototype.toString.call(arg) == '[object Uint8Array]')  {
    var buf = arg;
  } else {
    throw new Error('writeBinary called without a string/Buffer argument: ' + arg);
  }
  this.tstack.push('"' + buf.toString('base64') + '"');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeBool"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeBool (bool)](#apidoc.element.thrift.TJSONProtocol.prototype.writeBool)
- description and source-code
```javascript
writeBool = function (bool) {
  this.tstack.push(bool ? 1 : 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeByte"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeByte (byte)](#apidoc.element.thrift.TJSONProtocol.prototype.writeByte)
- description and source-code
```javascript
writeByte = function (byte) {
  this.tstack.push(byte);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeDouble"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeDouble (dub)](#apidoc.element.thrift.TJSONProtocol.prototype.writeDouble)
- description and source-code
```javascript
writeDouble = function (dub) {
  this.tstack.push(dub);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeFieldBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeFieldBegin (name, fieldType, fieldId)](#apidoc.element.thrift.TJSONProtocol.prototype.writeFieldBegin)
- description and source-code
```javascript
writeFieldBegin = function (name, fieldType, fieldId) {
  this.tpos.push(this.tstack.length);
  this.tstack.push({ 'fieldId': '"' +
    fieldId + '"', 'fieldType': TJSONProtocol.Type[fieldType]
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeFieldEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeFieldEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeFieldEnd)
- description and source-code
```javascript
writeFieldEnd = function () {
  var value = this.tstack.pop();
  var fieldInfo = this.tstack.pop();

  if (':' + value === ":[object Object]") {
    this.tstack[this.tstack.length - 1][fieldInfo.fieldId] = '{' +
      fieldInfo.fieldType + ':' + JSON.stringify(value) + '}';
  } else {
    this.tstack[this.tstack.length - 1][fieldInfo.fieldId] = '{' +
      fieldInfo.fieldType + ':' + value + '}';
  }
  this.tpos.pop();

  this.writeToTransportIfStackIsFlushable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeFieldStop"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeFieldStop ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeFieldStop)
- description and source-code
```javascript
writeFieldStop = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeI16"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeI16 (i16)](#apidoc.element.thrift.TJSONProtocol.prototype.writeI16)
- description and source-code
```javascript
writeI16 = function (i16) {
  this.tstack.push(i16);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeI32"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeI32 (i32)](#apidoc.element.thrift.TJSONProtocol.prototype.writeI32)
- description and source-code
```javascript
writeI32 = function (i32) {
  this.tstack.push(i32);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeI64"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeI64 (i64)](#apidoc.element.thrift.TJSONProtocol.prototype.writeI64)
- description and source-code
```javascript
writeI64 = function (i64) {
  if (i64 instanceof Int64) {
    this.tstack.push(Int64Util.toDecimalString(i64));
  } else {
    this.tstack.push(i64);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeListBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeListBegin (elemType, size)](#apidoc.element.thrift.TJSONProtocol.prototype.writeListBegin)
- description and source-code
```javascript
writeListBegin = function (elemType, size) {
  this.tpos.push(this.tstack.length);
  this.tstack.push([TJSONProtocol.Type[elemType], size]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeListEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeListEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeListEnd)
- description and source-code
```javascript
writeListEnd = function () {
  var p = this.tpos.pop();

  while (this.tstack.length > p + 1) {
    var tmpVal = this.tstack[p + 1];
    this.tstack.splice(p + 1, 1);
    this.tstack[p].push(tmpVal);
  }

  this.tstack[p] = '[' + this.tstack[p].join(',') + ']';

  this.writeToTransportIfStackIsFlushable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeMapBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeMapBegin (keyType, valType, size)](#apidoc.element.thrift.TJSONProtocol.prototype.writeMapBegin)
- description and source-code
```javascript
writeMapBegin = function (keyType, valType, size) {
  //size is invalid, we'll set it on end.
  this.tpos.push(this.tstack.length);
  this.tstack.push([TJSONProtocol.Type[keyType], TJSONProtocol.Type[valType], 0]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeMapEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeMapEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeMapEnd)
- description and source-code
```javascript
writeMapEnd = function () {
  var p = this.tpos.pop();

  if (p == this.tstack.length) {
    return;
  }

  if ((this.tstack.length - p - 1) % 2 !== 0) {
    this.tstack.push('');
  }

  var size = (this.tstack.length - p - 1) / 2;

  this.tstack[p][this.tstack[p].length - 1] = size;

  var map = '}';
  var first = true;
  while (this.tstack.length > p + 1) {
    var v = this.tstack.pop();
    var k = this.tstack.pop();
    if (first) {
      first = false;
    } else {
      map = ',' + map;
    }

    if (! isNaN(k)) { k = '"' + k + '"'; } //json "keys" need to be strings
    map = k + ':' + v + map;
  }
  map = '{' + map;

  this.tstack[p].push(map);
  this.tstack[p] = '[' + this.tstack[p].join(',') + ']';

  this.writeToTransportIfStackIsFlushable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeMessageBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeMessageBegin (name, messageType, seqid)](#apidoc.element.thrift.TJSONProtocol.prototype.writeMessageBegin)
- description and source-code
```javascript
writeMessageBegin = function (name, messageType, seqid) {
  this.tstack.push([TJSONProtocol.Version, '"' + name + '"', messageType, seqid]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeMessageEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeMessageEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeMessageEnd)
- description and source-code
```javascript
writeMessageEnd = function () {
  var obj = this.tstack.pop();

  this.wobj = this.tstack.pop();
  this.wobj.push(obj);

  this.wbuf = '[' + this.wobj.join(',') + ']';

  // we assume there is nothing more to come so we write
  this.trans.write(this.wbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeSetBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeSetBegin (elemType, size)](#apidoc.element.thrift.TJSONProtocol.prototype.writeSetBegin)
- description and source-code
```javascript
writeSetBegin = function (elemType, size) {
    this.tpos.push(this.tstack.length);
    this.tstack.push([TJSONProtocol.Type[elemType], size]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeSetEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeSetEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeSetEnd)
- description and source-code
```javascript
writeSetEnd = function () {
  var p = this.tpos.pop();

  while (this.tstack.length > p + 1) {
    var tmpVal = this.tstack[p + 1];
    this.tstack.splice(p + 1, 1);
    this.tstack[p].push(tmpVal);
  }

  this.tstack[p] = '[' + this.tstack[p].join(',') + ']';

  this.writeToTransportIfStackIsFlushable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeString"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeString (arg)](#apidoc.element.thrift.TJSONProtocol.prototype.writeString)
- description and source-code
```javascript
writeString = function (arg) {
  // We do not encode uri components for wire transfer:
  if (arg === null) {
      this.tstack.push(null);
  } else {
      if (typeof arg === 'string') {
        var str = arg;
      } else if (arg instanceof Buffer) {
        var str = arg.toString('utf8');
      } else {
        throw new Error('writeString called without a string/Buffer argument: ' + arg);
      }

      // concat may be slower than building a byte buffer
      var escapedString = '';
      for (var i = 0; i < str.length; i++) {
          var ch = str.charAt(i);      // a single double quote: "
          if (ch === '\"') {
              escapedString += '\\\"'; // write out as: \"
          } else if (ch === '\\') {    // a single backslash: \
              escapedString += '\\\\'; // write out as: \\
<span class="apidocCodeCommentSpan">          /* Currently escaped forward slashes break TJSONProtocol.
           * As it stands, we can simply pass forward slashes into
           * our strings across the wire without being escaped.
           * I think this is the protocol's bug, not thrift.js
           * } else if(ch === '/') {   // a single forward slash: /
           *  escapedString += '\\/';  // write out as \/
           * }
           */
</span>          } else if (ch === '\b') {    // a single backspace: invisible
              escapedString += '\\b';  // write out as: \b"
          } else if (ch === '\f') {    // a single formfeed: invisible
              escapedString += '\\f';  // write out as: \f"
          } else if (ch === '\n') {    // a single newline: invisible
              escapedString += '\\n';  // write out as: \n"
          } else if (ch === '\r') {    // a single return: invisible
              escapedString += '\\r';  // write out as: \r"
          } else if (ch === '\t') {    // a single tab: invisible
              escapedString += '\\t';  // write out as: \t"
          } else {
              escapedString += ch;     // Else it need not be escaped
          }
      }
      this.tstack.push('"' + escapedString + '"');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeStructBegin"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeStructBegin (name)](#apidoc.element.thrift.TJSONProtocol.prototype.writeStructBegin)
- description and source-code
```javascript
writeStructBegin = function (name) {
  this.tpos.push(this.tstack.length);
  this.tstack.push({});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeStructEnd"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeStructEnd ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeStructEnd)
- description and source-code
```javascript
writeStructEnd = function () {
  var p = this.tpos.pop();
  var struct = this.tstack[p];
  var str = '{';
  var first = true;
  for (var key in struct) {
    if (first) {
      first = false;
    } else {
      str += ',';
    }

    str += key + ':' + struct[key];
  }

  str += '}';
  this.tstack[p] = str;

  this.writeToTransportIfStackIsFlushable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.TJSONProtocol.prototype.writeToTransportIfStackIsFlushable"></a>[function <span class="apidocSignatureSpan">thrift.TJSONProtocol.prototype.</span>writeToTransportIfStackIsFlushable ()](#apidoc.element.thrift.TJSONProtocol.prototype.writeToTransportIfStackIsFlushable)
- description and source-code
```javascript
writeToTransportIfStackIsFlushable = function () {
  if (this.tstack.length === 1) {
    this.trans.write(this.tstack.pop());
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Thrift"></a>[module thrift.Thrift](#apidoc.module.thrift.Thrift)

#### <a name="apidoc.element.thrift.Thrift.TApplicationException"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.</span>TApplicationException (type, message)](#apidoc.element.thrift.Thrift.TApplicationException)
- description and source-code
```javascript
function TApplicationException(type, message) {
  TException.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.type = type || TApplicationExceptionType.UNKNOWN;
  this.name = this.constructor.name;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.TException"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.</span>TException (message)](#apidoc.element.thrift.Thrift.TException)
- description and source-code
```javascript
function TException(message) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.TProtocolException"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.</span>TProtocolException (type, message)](#apidoc.element.thrift.Thrift.TProtocolException)
- description and source-code
```javascript
function TProtocolException(type, message) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.type = type;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.copyList"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.</span>copyList (lst, types)](#apidoc.element.thrift.Thrift.copyList)
- description and source-code
```javascript
copyList = function (lst, types) {

  if (!lst) {return lst; }

  var type;

  if (types.shift === undefined) {
    type = types;
  }
  else {
    type = types[0];
  }
  var Type = type;

  var len = lst.length, result = [], i, val;
  for (i = 0; i < len; i++) {
    val = lst[i];
    if (type === null) {
      result.push(val);
    }
    else if (type === copyMap || type === copyList) {
      result.push(type(val, types.slice(1)));
    }
    else {
      result.push(new Type(val));
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.copyMap"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.</span>copyMap (obj, types)](#apidoc.element.thrift.Thrift.copyMap)
- description and source-code
```javascript
copyMap = function (obj, types){

  if (!obj) {return obj; }

  var type;

  if (types.shift === undefined) {
    type = types;
  }
  else {
    type = types[0];
  }
  var Type = type;

  var result = {}, val;
  for(var prop in obj) {
    if(obj.hasOwnProperty(prop)) {
      val = obj[prop];
      if (type === null) {
        result[prop] = val;
      }
      else if (type === copyMap || type === copyList) {
        result[prop] = type(val, types.slice(1));
      }
      else {
        result[prop] = new Type(val);
      }
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.inherits"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.</span>inherits (constructor, superConstructor)](#apidoc.element.thrift.Thrift.inherits)
- description and source-code
```javascript
inherits = function (constructor, superConstructor) {
  util.inherits(constructor, superConstructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.objectLength"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.</span>objectLength (obj)](#apidoc.element.thrift.Thrift.objectLength)
- description and source-code
```javascript
objectLength = function (obj) {
  return Object.keys(obj).length;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Thrift.TApplicationException"></a>[module thrift.Thrift.TApplicationException](#apidoc.module.thrift.Thrift.TApplicationException)

#### <a name="apidoc.element.thrift.Thrift.TApplicationException.TApplicationException"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.</span>TApplicationException (type, message)](#apidoc.element.thrift.Thrift.TApplicationException.TApplicationException)
- description and source-code
```javascript
function TApplicationException(type, message) {
  TException.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.type = type || TApplicationExceptionType.UNKNOWN;
  this.name = this.constructor.name;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.TApplicationException.super_"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.TApplicationException.</span>super_ (message)](#apidoc.element.thrift.Thrift.TApplicationException.super_)
- description and source-code
```javascript
function TException(message) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Thrift.TApplicationException.prototype"></a>[module thrift.Thrift.TApplicationException.prototype](#apidoc.module.thrift.Thrift.TApplicationException.prototype)

#### <a name="apidoc.element.thrift.Thrift.TApplicationException.prototype.read"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.TApplicationException.prototype.</span>read (input)](#apidoc.element.thrift.Thrift.TApplicationException.prototype.read)
- description and source-code
```javascript
read = function (input) {
  var ftype;
  var ret = input.readStructBegin('TApplicationException');

  while(1){
      ret = input.readFieldBegin();
      if(ret.ftype == Type.STOP)
          break;

      switch(ret.fid){
          case 1:
              if( ret.ftype == Type.STRING ){
                  ret = input.readString();
                  this.message = ret;
              } else {
                  ret = input.skip(ret.ftype);
              }
              break;
          case 2:
              if( ret.ftype == Type.I32 ){
                  ret = input.readI32();
                  this.type = ret;
              } else {
                  ret   = input.skip(ret.ftype);
              }
              break;
          default:
              ret = input.skip(ret.ftype);
              break;
      }
      input.readFieldEnd();
  }
  input.readStructEnd();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.TApplicationException.prototype.write"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.TApplicationException.prototype.</span>write (output)](#apidoc.element.thrift.Thrift.TApplicationException.prototype.write)
- description and source-code
```javascript
write = function (output){
  output.writeStructBegin('TApplicationException');

  if (this.message) {
      output.writeFieldBegin('message', Type.STRING, 1);
      output.writeString(this.message);
      output.writeFieldEnd();
  }

  if (this.code) {
      output.writeFieldBegin('type', Type.I32, 2);
      output.writeI32(this.code);
      output.writeFieldEnd();
  }

  output.writeFieldStop();
  output.writeStructEnd();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Thrift.TException"></a>[module thrift.Thrift.TException](#apidoc.module.thrift.Thrift.TException)

#### <a name="apidoc.element.thrift.Thrift.TException.TException"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.</span>TException (message)](#apidoc.element.thrift.Thrift.TException.TException)
- description and source-code
```javascript
function TException(message) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.TException.super_"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.TException.</span>super_ ()](#apidoc.element.thrift.Thrift.TException.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.Thrift.TProtocolException"></a>[module thrift.Thrift.TProtocolException](#apidoc.module.thrift.Thrift.TProtocolException)

#### <a name="apidoc.element.thrift.Thrift.TProtocolException.TProtocolException"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.</span>TProtocolException (type, message)](#apidoc.element.thrift.Thrift.TProtocolException.TProtocolException)
- description and source-code
```javascript
function TProtocolException(type, message) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.type = type;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.Thrift.TProtocolException.super_"></a>[function <span class="apidocSignatureSpan">thrift.Thrift.TProtocolException.</span>super_ ()](#apidoc.element.thrift.Thrift.TProtocolException.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.WSConnection"></a>[module thrift.WSConnection](#apidoc.module.thrift.WSConnection)

#### <a name="apidoc.element.thrift.WSConnection.WSConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>WSConnection (host, port, options)](#apidoc.element.thrift.WSConnection.WSConnection)
- description and source-code
```javascript
function WSConnection(host, port, options) {
  //Initialize the emitter base object
  EventEmitter.call(this);

  //Set configuration
  var self = this;
  this.options = options || {};
  this.host = host;
  this.port = port;
  this.secure = this.options.secure || false;
  this.transport = this.options.transport || TBufferedTransport;
  this.protocol = this.options.protocol || TJSONProtocol;
  this.path = this.options.path;
  this.send_pending = [];

  //The sequence map is used to map seqIDs back to the
  //  calling client in multiplexed scenarios
  this.seqId2Service = {};

  //Prepare WebSocket options
  this.wsOptions = {
    host: this.host,
    port: this.port || 80,
    path: this.options.path || '/',
    headers: this.options.headers || {}
  };
  for (var attrname in this.options.wsOptions) {
    this.wsOptions[attrname] = this.options.wsOptions[attrname];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.super_"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.</span>super_ ()](#apidoc.element.thrift.WSConnection.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.WSConnection.prototype"></a>[module thrift.WSConnection.prototype](#apidoc.module.thrift.WSConnection.prototype)

#### <a name="apidoc.element.thrift.WSConnection.prototype.__decodeCallback"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__decodeCallback (transport_with_data)](#apidoc.element.thrift.WSConnection.prototype.__decodeCallback)
- description and source-code
```javascript
__decodeCallback = function (transport_with_data) {
  var proto = new this.protocol(transport_with_data);
  try {
    while (true) {
      var header = proto.readMessageBegin();
      var dummy_seqid = header.rseqid * -1;
      var client = this.client;
      //The Multiplexed Protocol stores a hash of seqid to service names
      //  in seqId2Service. If the SeqId is found in the hash we need to
      //  lookup the appropriate client for this call.
      //  The client var is a single client object when not multiplexing,
      //  when using multiplexing it is a service name keyed hash of client
      //  objects.
      //NOTE: The 2 way interdependencies between protocols, transports,
      //  connections and clients in the Node.js implementation are irregular
      //  and make the implementation difficult to extend and maintain. We
      //  should bring this stuff inline with typical thrift I/O stack
      //  operation soon.
      //  --ra
      var service_name = this.seqId2Service[header.rseqid];
      if (service_name) {
        client = this.client[service_name];
        delete this.seqId2Service[header.rseqid];
      }
<span class="apidocCodeCommentSpan">      /*jshint -W083 */
</span>      client._reqs[dummy_seqid] = function(err, success) {
        transport_with_data.commitPosition();
        var clientCallback = client._reqs[header.rseqid];
        delete client._reqs[header.rseqid];
        if (clientCallback) {
          clientCallback(err, success);
        }
      };
      /*jshint +W083 */
      if (client['recv_' + header.fname]) {
        client['recv_' + header.fname](proto, header.mtype, dummy_seqid);
      } else {
        delete client._reqs[dummy_seqid];
        this.emit("error",
          new thrift.TApplicationException(
            thrift.TApplicationExceptionType.WRONG_METHOD_NAME,
            "Received a response to an unknown RPC function"));
      }
    }
  } catch (e) {
    if (e instanceof InputBufferUnderrunError) {
      transport_with_data.rollbackPosition();
    } else {
      throw e;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.__onClose"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__onClose (evt)](#apidoc.element.thrift.WSConnection.prototype.__onClose)
- description and source-code
```javascript
__onClose = function (evt) {
  this.emit("close");
  this.__reset();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.__onData"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__onData (data)](#apidoc.element.thrift.WSConnection.prototype.__onData)
- description and source-code
```javascript
__onData = function (data) {
  if (Object.prototype.toString.call(data) == "[object ArrayBuffer]") {
    data = new Uint8Array(data);
  }
  var buf = new Buffer(data);
  this.transport.receiver(this.__decodeCallback.bind(this))(buf);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.__onError"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__onError (evt)](#apidoc.element.thrift.WSConnection.prototype.__onError)
- description and source-code
```javascript
__onError = function (evt) {
  this.emit("error", evt);
  this.socket.close();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.__onMessage"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__onMessage (evt)](#apidoc.element.thrift.WSConnection.prototype.__onMessage)
- description and source-code
```javascript
__onMessage = function (evt) {
  this.__onData(evt.data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.__onOpen"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__onOpen ()](#apidoc.element.thrift.WSConnection.prototype.__onOpen)
- description and source-code
```javascript
__onOpen = function () {
  var self = this;
  this.emit("open");
  if (this.send_pending.length > 0) {
    //If the user made calls before the connection was fully
    //open, send them now
    this.send_pending.forEach(function(data) {
      self.socket.send(data);
    });
    this.send_pending = [];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.__reset"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>__reset ()](#apidoc.element.thrift.WSConnection.prototype.__reset)
- description and source-code
```javascript
__reset = function () {
  this.socket = null; //The web socket
  this.send_pending = []; //Buffers/Callback pairs waiting to be sent
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.close"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>close ()](#apidoc.element.thrift.WSConnection.prototype.close)
- description and source-code
```javascript
close = function () {
  this.socket.close();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.isOpen"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>isOpen ()](#apidoc.element.thrift.WSConnection.prototype.isOpen)
- description and source-code
```javascript
isOpen = function () {
  return this.socket && this.socket.readyState == this.socket.OPEN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.open"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>open ()](#apidoc.element.thrift.WSConnection.prototype.open)
- description and source-code
```javascript
open = function () {
  //If OPEN/CONNECTING/CLOSING ignore additional opens
  if (this.socket && this.socket.readyState != this.socket.CLOSED) {
    return;
  }
  //If there is no socket or the socket is closed:
  this.socket = new WebSocket(this.uri(), "", this.wsOptions);
  this.socket.binaryType = 'arraybuffer';
  this.socket.onopen = this.__onOpen.bind(this);
  this.socket.onmessage = this.__onMessage.bind(this);
  this.socket.onerror = this.__onError.bind(this);
  this.socket.onclose = this.__onClose.bind(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.uri"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>uri ()](#apidoc.element.thrift.WSConnection.prototype.uri)
- description and source-code
```javascript
uri = function () {
  var schema = this.secure ? 'wss' : 'ws';
  var port = '';
  var path = this.path || '/';
  var host = this.host;

  // avoid port if default for schema
  if (this.port && (('wss' == schema && this.port != 443) ||
    ('ws' == schema && this.port != 80))) {
    port = ':' + this.port;
  }

  return schema + '://' + host + port + path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.WSConnection.prototype.write"></a>[function <span class="apidocSignatureSpan">thrift.WSConnection.prototype.</span>write (data)](#apidoc.element.thrift.WSConnection.prototype.write)
- description and source-code
```javascript
write = function (data) {
  if (this.isOpen()) {
    //Send data and register a callback to invoke the client callback
    this.socket.send(data);
  } else {
    //Queue the send to go out __onOpen
    this.send_pending.push(data);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.XHRConnection"></a>[module thrift.XHRConnection](#apidoc.module.thrift.XHRConnection)

#### <a name="apidoc.element.thrift.XHRConnection.XHRConnection"></a>[function <span class="apidocSignatureSpan">thrift.</span>XHRConnection (host, port, options)](#apidoc.element.thrift.XHRConnection.XHRConnection)
- description and source-code
```javascript
function XHRConnection(host, port, options) {
  this.options = options || {};
  this.wpos = 0;
  this.rpos = 0;
  this.useCORS = (options && options.useCORS);
  this.send_buf = '';
  this.recv_buf = '';
  this.transport = options.transport || TBufferedTransport;
  this.protocol = options.protocol || TJSONProtocol;
  this.headers = options.headers || {};

  host = host || window.location.host;
  port = port || window.location.port;
  var prefix = options.https ? 'https://' : 'http://';
  var path = options.path || '/';

  if (port === '') {
    port = undefined;
  }

  if (!port || port === 80 || port === '80') {
    this.url = prefix + host + path;
  } else {
    this.url = prefix + host + ':' + port + path;
  }

  //The sequence map is used to map seqIDs back to the
  //  calling client in multiplexed scenarios
  this.seqId2Service = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.super_"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.</span>super_ ()](#apidoc.element.thrift.XHRConnection.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thrift.XHRConnection.prototype"></a>[module thrift.XHRConnection.prototype](#apidoc.module.thrift.XHRConnection.prototype)

#### <a name="apidoc.element.thrift.XHRConnection.prototype.__decodeCallback"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>__decodeCallback (transport_with_data)](#apidoc.element.thrift.XHRConnection.prototype.__decodeCallback)
- description and source-code
```javascript
__decodeCallback = function (transport_with_data) {
  var proto = new this.protocol(transport_with_data);
  try {
    while (true) {
      var header = proto.readMessageBegin();
      var dummy_seqid = header.rseqid * -1;
      var client = this.client;
      //The Multiplexed Protocol stores a hash of seqid to service names
      //  in seqId2Service. If the SeqId is found in the hash we need to
      //  lookup the appropriate client for this call.
      //  The client var is a single client object when not multiplexing,
      //  when using multiplexing it is a service name keyed hash of client
      //  objects.
      //NOTE: The 2 way interdependencies between protocols, transports,
      //  connections and clients in the Node.js implementation are irregular
      //  and make the implementation difficult to extend and maintain. We
      //  should bring this stuff inline with typical thrift I/O stack
      //  operation soon.
      //  --ra
      var service_name = this.seqId2Service[header.rseqid];
      if (service_name) {
        client = this.client[service_name];
        delete this.seqId2Service[header.rseqid];
      }
<span class="apidocCodeCommentSpan">      /*jshint -W083 */
</span>      client._reqs[dummy_seqid] = function(err, success) {
        transport_with_data.commitPosition();
        var clientCallback = client._reqs[header.rseqid];
        delete client._reqs[header.rseqid];
        if (clientCallback) {
          clientCallback(err, success);
        }
      };
      /*jshint +W083 */
      if (client['recv_' + header.fname]) {
        client['recv_' + header.fname](proto, header.mtype, dummy_seqid);
      } else {
        delete client._reqs[dummy_seqid];
        this.emit("error",
          new thrift.TApplicationException(
            thrift.TApplicationExceptionType.WRONG_METHOD_NAME,
            "Received a response to an unknown RPC function"));
      }
    }
  } catch (e) {
    if (e instanceof InputBufferUnderrunError) {
      transport_with_data.rollbackPosition();
    } else {
      throw e;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.prototype.close"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>close ()](#apidoc.element.thrift.XHRConnection.prototype.close)
- description and source-code
```javascript
close = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.prototype.flush"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>flush ()](#apidoc.element.thrift.XHRConnection.prototype.flush)
- description and source-code
```javascript
flush = function () {
  var self = this;
  if (this.url === undefined || this.url === '') {
    return this.send_buf;
  }

  var xreq = this.getXmlHttpRequestObject();

  if (xreq.overrideMimeType) {
    xreq.overrideMimeType('application/json');
  }

  xreq.onreadystatechange = function() {
    if (this.readyState == 4 && this.status == 200) {
      self.setRecvBuffer(this.responseText);
    }
  };

  xreq.open('POST', this.url, true);

  Object.keys(this.headers).forEach(function(headerKey) {
    xreq.setRequestHeader(headerKey, self.headers[headerKey]);
  });

  xreq.send(this.send_buf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.prototype.getSendBuffer"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>getSendBuffer ()](#apidoc.element.thrift.XHRConnection.prototype.getSendBuffer)
- description and source-code
```javascript
getSendBuffer = function () {
  return this.send_buf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.prototype.getXmlHttpRequestObject"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>getXmlHttpRequestObject ()](#apidoc.element.thrift.XHRConnection.prototype.getXmlHttpRequestObject)
- description and source-code
```javascript
getXmlHttpRequestObject = function () {
  try { return new XMLHttpRequest(); } catch (e1) { }
  try { return new ActiveXObject('Msxml2.XMLHTTP'); } catch (e2) { }
  try { return new ActiveXObject('Microsoft.XMLHTTP'); } catch (e3) { }

  throw "Your browser doesn't support XHR.";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.prototype.isOpen"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>isOpen ()](#apidoc.element.thrift.XHRConnection.prototype.isOpen)
- description and source-code
```javascript
isOpen = function () {
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.prototype.open"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>open ()](#apidoc.element.thrift.XHRConnection.prototype.open)
- description and source-code
```javascript
open = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.prototype.read"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>read (len)](#apidoc.element.thrift.XHRConnection.prototype.read)
- description and source-code
```javascript
read = function (len) {
  var avail = this.wpos - this.rpos;

  if (avail === 0) {
    return '';
  }

  var give = len;

  if (avail < len) {
    give = avail;
  }

  var ret = this.read_buf.substr(this.rpos, give);
  this.rpos += give;

  //clear buf when complete?
  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.prototype.readAll"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>readAll ()](#apidoc.element.thrift.XHRConnection.prototype.readAll)
- description and source-code
```javascript
readAll = function () {
  return this.recv_buf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.prototype.setRecvBuffer"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>setRecvBuffer (buf)](#apidoc.element.thrift.XHRConnection.prototype.setRecvBuffer)
- description and source-code
```javascript
setRecvBuffer = function (buf) {
  this.recv_buf = buf;
  this.recv_buf_sz = this.recv_buf.length;
  this.wpos = this.recv_buf.length;
  this.rpos = 0;

  if (Object.prototype.toString.call(buf) == "[object ArrayBuffer]") {
    var data = new Uint8Array(buf);
  }
  var thing = new Buffer(data || buf);

  this.transport.receiver(this.__decodeCallback.bind(this))(thing);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thrift.XHRConnection.prototype.write"></a>[function <span class="apidocSignatureSpan">thrift.XHRConnection.prototype.</span>write (buf)](#apidoc.element.thrift.XHRConnection.prototype.write)
- description and source-code
```javascript
write = function (buf) {
  this.send_buf = buf;
  this.flush();
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
