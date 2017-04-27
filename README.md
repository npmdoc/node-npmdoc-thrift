# npmdoc-thrift

#### basic api documentation for  [thrift (v0.10.0)](http://thrift.apache.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-thrift.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-thrift) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-thrift.svg)](https://travis-ci.org/npmdoc/node-npmdoc-thrift)

#### node.js bindings for the Apache Thrift RPC system

[![NPM](https://nodei.co/npm/thrift.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/thrift)

- [https://npmdoc.github.io/node-npmdoc-thrift/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-thrift/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-thrift/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-thrift/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-thrift/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-thrift/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Apache Thrift Developers",
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
            "name": "wadey"
        },
        {
            "name": "jfarrell"
        }
    ],
    "name": "thrift",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "https://git-wip-us.apache.org/repos/asf/thrift.git"
    },
    "scripts": {
        "cover": "lib/nodejs/test/testAll.sh COVER",
        "test": "lib/nodejs/test/testAll.sh"
    },
    "version": "0.10.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
