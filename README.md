# npmtest-lokijs

#### basic test coverage for  [lokijs (v1.4.3)](http://lokijs.org)  [![npm package](https://img.shields.io/npm/v/npmtest-lokijs.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-lokijs) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-lokijs.svg)](https://travis-ci.org/npmtest/node-npmtest-lokijs)

#### Fast document oriented javascript in-memory database

[![NPM](https://nodei.co/npm/lokijs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/lokijs)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-lokijs/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-lokijs/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-lokijs/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-lokijs/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-lokijs/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-lokijs/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-lokijs/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-lokijs/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-lokijs/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-lokijs/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-lokijs/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-lokijs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-lokijs/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-lokijs/build/test-report.html](https://npmtest.github.io/node-npmtest-lokijs/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-lokijs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-lokijs/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-lokijs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-lokijs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-lokijs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-lokijs/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-lokijs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-lokijs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Joe Minichino"
    },
    "bugs": {
        "url": "https://github.com/techfort/LokiJS/issues"
    },
    "contributors": [
        {
            "name": "Dave"
        }
    ],
    "dependencies": {},
    "description": "Fast document oriented javascript in-memory database",
    "devDependencies": {
        "istanbul": "^0.4.4",
        "jasmine": "^2.4.1",
        "jsdoc": "^3.4.0",
        "jshint": "^2.9.2",
        "karma": "^1.1.2",
        "karma-cli": "^1.0.1",
        "karma-coverage": "^1.1.1",
        "karma-jasmine": "^1.0.2",
        "karma-phantomjs-launcher": "^1.0.1",
        "mocha": "^2.5.3",
        "phantomjs": "^1.9.20",
        "rimraf": "^2.5.4",
        "should": "^4.6.5",
        "uglify-js": "^2.7.0"
    },
    "directories": {
        "example": "examples"
    },
    "dist": {
        "shasum": "f2a47ba8d6991c92d6da6a5b35be79b674453abb",
        "tarball": "https://registry.npmjs.org/lokijs/-/lokijs-1.4.3.tgz"
    },
    "gitHead": "65798b65a672bf1ca198df9863319affaf87517b",
    "homepage": "http://lokijs.org",
    "keywords": [
        "javascript",
        "document-oriented",
        "mmdb",
        "json",
        "nosql",
        "lokijs",
        "in-memory"
    ],
    "license": "MIT",
    "main": "src/lokijs.js",
    "maintainers": [
        {
            "name": "techfort"
        }
    ],
    "name": "lokijs",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/techfort/LokiJS.git"
    },
    "scripts": {
        "build": "npm run build:lokijs && npm run build:indexedAdapter",
        "build:indexedAdapter": "uglifyjs src/loki-indexed-adapter.js > build/loki-indexed-adapter.min.js",
        "build:lokijs": "uglifyjs src/lokijs.js > build/lokijs.min.js",
        "clean": "rimraf build/* coverage/* node_modules",
        "jsdoc": "jsdoc -c jsdoc-conf.json",
        "lint": "jshint src",
        "postbuild": "karma start karma.build.conf.js --single-run",
        "pour:beer": "echo New npm version published, one beer for you !",
        "prepublish": "npm run build",
        "pretest": "npm run lint",
        "test": "npm run test:browser && npm run test:node",
        "test:browser": "karma start karma.conf.js --single-run",
        "test:node": "istanbul cover --dir coverage/nodejs node_modules/jasmine/bin/jasmine.js"
    },
    "version": "1.4.3",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
