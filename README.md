# npmtest-angular2-infinite-scroll

#### basic test coverage for  angular2-infinite-scroll (v0.3.42)  [![npm package](https://img.shields.io/npm/v/npmtest-angular2-infinite-scroll.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-angular2-infinite-scroll) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-angular2-infinite-scroll.svg)](https://travis-ci.org/npmtest/node-npmtest-angular2-infinite-scroll)

#### An infinite scroll directive for angular2

[![NPM](https://nodei.co/npm/angular2-infinite-scroll.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/angular2-infinite-scroll)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-angular2-infinite-scroll/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-angular2-infinite-scroll/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/test-report.html](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-angular2-infinite-scroll/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-angular2-infinite-scroll/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-angular2-infinite-scroll/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-angular2-infinite-scroll/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-angular2-infinite-scroll/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "angular2-infinite-scroll",
    "version": "0.3.42",
    "description": "An infinite scroll directive for angular2",
    "main": "angular2-infinite-scroll.js",
    "typings": "./angular2-infinite-scroll.d.ts",
    "repository": "orizens/angular2-infinite-scroll",
    "scripts": {
        "build:test": "tsc --project ./src",
        "clean": "npm run clean:jsfiles && npm run clean:typefiles && npm run clean:metadata",
        "clean:jsfiles": "rimraf src/*.js && rimraf ./*scroll.js",
        "clean:typefiles": "rimraf src/*.d.ts && rimraf ./*scroll.d.ts",
        "clean:node": "rimraf node_modules",
        "clean:metadata": "rimraf ./*metadata.json && rimraf src/ngfactory && rimraf ./src/*.metadata.json",
        "bdd": "NODE_ENV='bdd' karma start karma.conf.js",
        "lite": "lite-server",
        "postversion": "git push origin master",
        "_prepublish": "node ./node_modules/@angular/compiler-cli/src/main.js && node make.js",
        "pretest": "npm run clean",
        "preversion": "npm run clean && npm run prepublish && npm test",
        "setup": "npm run typings -- install",
        "start": "npm run build && npm run lite",
        "test": "karma start karma.conf.js",
        "watch": "tsc --project ./src --watch"
    },
    "keywords": [
        "angular2",
        "scroll",
        "infinite"
    ],
    "author": "Oren Farhi",
    "license": "MIT",
    "devDependencies": {
        "@angular/common": "2.3.1",
        "@angular/compiler": "2.3.1",
        "@angular/compiler-cli": "2.3.1",
        "@angular/core": "2.3.1",
        "@angular/platform-browser": "2.3.1",
        "@angular/platform-browser-dynamic": "2.3.1",
        "@types/core-js": "0.9.32",
        "@types/jasmine": "2.2.33",
        "@types/node": "6.0.38",
        "autodts": "0.0.6",
        "awesome-typescript-loader": "2.2.4",
        "es6-promise": "3.0.2",
        "es6-shim": "0.33.3",
        "istanbul-instrumenter-loader": "^1.0.0",
        "jasmine-core": "2.4.1",
        "karma": "^0.13.22",
        "karma-chrome-launcher": "^1.0.1",
        "karma-cli": "^1.0.0",
        "karma-jasmine": "^1.0.2",
        "karma-mocha-reporter": "2.0.4",
        "karma-phantomjs-launcher": "1.0.0",
        "karma-sourcemap-loader": "^0.3.7",
        "karma-webpack": "^1.8.0",
        "lite-server": "2.2.0",
        "path": "^0.12.7",
        "phantomjs-prebuilt": "^2.1.7",
        "reflect-metadata": "0.1.2",
        "rimraf": "2.5.2",
        "rxjs": "5.0.2",
        "source-map-loader": "^0.1.5",
        "systemjs": "0.19.31",
        "systemjs-builder": "^0.15.16",
        "ts-helpers": "^1.1.1",
        "tslint": "^3.15.1",
        "tslint-loader": "^2.1.5",
        "typescript": "2.0.3",
        "webpack": "2.1.0-beta.21",
        "zone.js": "^0.6.17"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
