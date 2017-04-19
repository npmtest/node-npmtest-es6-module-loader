# npmtest-es6-module-loader

#### test coverage for  [es6-module-loader (v0.17.11)](https://github.com/ModuleLoader/es6-module-loader)  [![npm package](https://img.shields.io/npm/v/npmtest-es6-module-loader.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-es6-module-loader) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-es6-module-loader.svg)](https://travis-ci.org/npmtest/node-npmtest-es6-module-loader)

#### An ES6 Module Loader shim

[![NPM](https://nodei.co/npm/es6-module-loader.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/es6-module-loader)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-es6-module-loader/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-es6-module-loader/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-es6-module-loader/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-es6-module-loader/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-es6-module-loader/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-es6-module-loader/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-es6-module-loader/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-es6-module-loader/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-es6-module-loader/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-es6-module-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-es6-module-loader/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-es6-module-loader/build/test-report.html](https://npmtest.github.io/node-npmtest-es6-module-loader/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-es6-module-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-es6-module-loader/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-es6-module-loader/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-es6-module-loader/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-es6-module-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-es6-module-loader/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-es6-module-loader/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-es6-module-loader/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Guy Bedford, Luke Hoban, Addy Osmani",
        "url": "https://github.com/ModuleLoader"
    },
    "bugs": {
        "url": "https://github.com/ModuleLoader/es6-module-loader/issues"
    },
    "dependencies": {
        "when": "^3.7.2"
    },
    "deprecated": "This project has been deprecated for \"npm install es-module-loader\" based on the newer loader spec.",
    "description": "An ES6 Module Loader shim",
    "devDependencies": {
        "babel-core": "^5.8.20",
        "expect.js": "^0.3.1",
        "gesalakacula": "^1.0.0",
        "grunt": "~0.4.1",
        "grunt-contrib-concat": "^0.5.0",
        "grunt-contrib-jshint": "~0.6.0",
        "grunt-contrib-uglify": "~0.6.0",
        "karma": "^0.12.35",
        "karma-benchmark": "^0.4.0",
        "karma-benchmark-reporter": "^0.1.1",
        "karma-chrome-launcher": "^0.1.7",
        "karma-coverage": "^0.2.7",
        "karma-expect": "^1.1.0",
        "karma-firefox-launcher": "^0.1.3",
        "karma-mocha": "^0.1.10",
        "karma-mocha-reporter": "^0.3.1",
        "karma-sauce-launcher": "^0.2.10",
        "minimist": "^1.1.0",
        "mocha": "^2.0.1",
        "regenerator": "^0.8.9",
        "traceur": "0.0.93",
        "typescript": "^1.6.2"
    },
    "directories": {},
    "dist": {
        "shasum": "094f042e3b4d3086bcfd17380affabdfc99f35d7",
        "tarball": "https://registry.npmjs.org/es6-module-loader/-/es6-module-loader-0.17.11.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "gitHead": "c08dc756f6bdcf39a190aa4c59c6be8673d0b3d2",
    "homepage": "https://github.com/ModuleLoader/es6-module-loader",
    "keywords": [
        "script",
        "loader",
        "es6",
        "harmony"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "https://github.com/ModuleLoader/es6-module-loader/blob/master/LICENSE-MIT"
        }
    ],
    "maintainers": [
        {
            "name": "addyosmani"
        },
        {
            "name": "guybedford"
        }
    ],
    "name": "es6-module-loader",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/ModuleLoader/es6-module-loader.git"
    },
    "scripts": {
        "test": "npm run test:node && npm run test:browser",
        "test:browser": "npm run test:browser-traceur && npm run test:browser-babel && npm run test:browser-typescript",
        "test:browser-babel": "karma start --single-run --babel",
        "test:browser-traceur": "karma start --single-run",
        "test:browser-typescript": "karma start --single-run --typescript",
        "test:browser:perf": "karma start karma-benchmark.conf.js --single-run",
        "test:node": "mocha test/_node-traceur.js && mocha test/_node-babel.js && mocha test/_node-typescript.js"
    },
    "version": "0.17.11"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
