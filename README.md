# npmtest-testdouble

#### basic test coverage for  [testdouble (v2.1.2)](https://github.com/testdouble/testdouble.js)  [![npm package](https://img.shields.io/npm/v/npmtest-testdouble.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-testdouble) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-testdouble.svg)](https://travis-ci.org/npmtest/node-npmtest-testdouble)

#### A minimal test double library for TDD with JavaScript

[![NPM](https://nodei.co/npm/testdouble.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/testdouble)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-testdouble/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-testdouble/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-testdouble/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-testdouble/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-testdouble/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-testdouble/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-testdouble/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-testdouble/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-testdouble/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-testdouble/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-testdouble/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-testdouble/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-testdouble/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-testdouble/build/test-report.html](https://npmtest.github.io/node-npmtest-testdouble/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-testdouble/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-testdouble/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-testdouble/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-testdouble/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-testdouble/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-testdouble/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-testdouble/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-testdouble/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Justin Searls",
        "url": "http://testdouble.com"
    },
    "babel": {
        "presets": [
            "env"
        ]
    },
    "browser": {
        "./lib/replace/module.js": "./lib/replace/module.browser.js",
        "quibble": "./lib/quibble.browser.js"
    },
    "bugs": {
        "url": "https://github.com/testdouble/testdouble.js/issues"
    },
    "config": {
        "build_file": "dist/testdouble.js",
        "test_bundle": "generated/tests.js",
        "mocha_reporter": "dot"
    },
    "dependencies": {
        "lodash": "^4.15.0",
        "quibble": "^0.5.0",
        "resolve": "^1.3.2",
        "stringify-object-es5": "^2.5.0"
    },
    "description": "A minimal test double library for TDD with JavaScript",
    "devDependencies": {
        "babel-cli": "^6.23.0",
        "babel-preset-env": "^1.2.1",
        "babelify": "^7.3.0",
        "browserify": "^14.1.0",
        "chai": "^3.2.0",
        "codeclimate-test-reporter": "^0.4.1",
        "coffee-script": "^1.10.0",
        "coffeeify": "^2.1.0",
        "headerify": "^1.0.1",
        "is-number": "^3.0.0",
        "mocha": "^3.2.0",
        "mocha-given": "^0.1.3",
        "nyc": "^10.1.2",
        "pryjs": "^1.0.3",
        "require-globify": "^1.4.1",
        "standard": "^9.0.2",
        "testem": "^1.15.0",
        "typescript": "^2.2.1"
    },
    "directories": {
        "doc": "./docs",
        "example": "./examples",
        "lib": "./lib",
        "src": "./src"
    },
    "dist": {
        "shasum": "8a376c5cb9b2c9cea90780b874168aa5b6eeb8a8",
        "tarball": "https://registry.npmjs.org/testdouble/-/testdouble-2.1.2.tgz"
    },
    "engines": {
        "node": ">= 4.0.0"
    },
    "gitHead": "f8dc482b72a10dcc2513b735f224283f8de87a37",
    "homepage": "https://github.com/testdouble/testdouble.js",
    "keywords": [
        "tdd",
        "bdd",
        "mock",
        "stub",
        "spy",
        "test double",
        "double"
    ],
    "license": "MIT",
    "main": "lib/testdouble.js",
    "maintainers": [
        {
            "name": "searls"
        }
    ],
    "name": "testdouble",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/testdouble/testdouble.js.git"
    },
    "scripts": {
        "clean": "rm -rf generated dist lib coverage && yarn run clean:dist",
        "clean:dist": "git checkout -- dist",
        "compile": "yarn run compile:node && yarn run compile:browser && yarn run compile:browser:test",
        "compile:browser": "browserify src/testdouble.js --standalone td --outfile $npm_package_config_build_file -p headerify -t babelify",
        "compile:browser:test": "mkdir -p generated && browserify test/browser-helper.js --outfile $npm_package_config_test_bundle -t babelify -t coffeeify --extension=\".coffee\" -t require-globify --ignore-missing",
        "compile:node": "babel src -d lib",
        "cover": "nyc --reporter=lcov --reporter=text-summary --require babel-core/register _mocha --ui mocha-given --reporter $npm_package_config_mocha_reporter --compilers coffee:coffee-script --recursive test/node-helper.coffee test/src",
        "cover:report": "codeclimate-test-reporter < coverage/lcov.info",
        "postversion": "git push --tags && yarn run version:changelog && git push && npm publish",
        "prepublish": "yarn run compile",
        "preversion": "git pull --rebase && yarn run test:ci",
        "style": "standard \"./src/**/*\" --fix",
        "test": "mocha --ui mocha-given --reporter $npm_package_config_mocha_reporter --compilers js:babel-core/register,coffee:coffee-script --recursive test/node-helper.coffee test/src",
        "test:all": "yarn test && yarn run test:browser && yarn run test:example && yarn run test:typescript",
        "test:browser": "testem ci",
        "test:ci": "yarn run clean && yarn run compile && yarn run style && yarn run test:all && yarn run clean:dist && echo \"All done!\"",
        "test:example": "yarn run test:example:node && yarn run test:example:lineman && yarn run test:example:webpack && yarn run test:example:babel",
        "test:example:babel": "cd examples/babel && yarn install && yarn test && cd ../..",
        "test:example:lineman": "cd examples/lineman && yarn install && yarn test && cd ../..",
        "test:example:node": "cd examples/node && yarn install && yarn test && cd ../..",
        "test:example:webpack": "cd examples/webpack && yarn install && yarn test && cd ../..",
        "test:typescript": "tsc --noEmit -p ./test/src/typescript",
        "version": "yarn run version:write && yarn run compile && git add dist src/version.js",
        "version:changelog": "if command -v github_changelog_generator &>/dev/null; then github_changelog_generator; git commit -m \"Changelog for $npm_package_version\" CHANGELOG.md; else echo Versioning requires you first run 'gem install github_changelog_generator' >&2; fi",
        "version:write": "echo \"export default '$npm_package_version'\" > src/version.js"
    },
    "standard": {
        "globals": [
            "describe",
            "it",
            "expect",
            "td"
        ]
    },
    "typings": "./index.d.ts",
    "version": "2.1.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
