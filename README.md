# npmtest-react-native-maps

#### basic test coverage for  [react-native-maps (v0.14.0)](https://github.com/airbnb/react-native-maps#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-react-native-maps.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-native-maps) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-native-maps.svg)](https://travis-ci.org/npmtest/node-npmtest-react-native-maps)

#### React Native Mapview component for iOS + Android

[![NPM](https://nodei.co/npm/react-native-maps.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-native-maps)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-native-maps/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-native-maps/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-native-maps/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-native-maps/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-native-maps/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-react-native-maps/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-react-native-maps/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-native-maps/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-native-maps/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-native-maps/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-native-maps/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-native-maps/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-native-maps/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-native-maps/build/test-report.html](https://npmtest.github.io/node-npmtest-react-native-maps/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-native-maps/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-native-maps/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-native-maps/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-native-maps/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-native-maps/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-native-maps/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-native-maps/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-native-maps/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Leland Richardson"
    },
    "bugs": {
        "url": "https://github.com/airbnb/react-native-maps/issues"
    },
    "dependencies": {},
    "description": "React Native Mapview component for iOS + Android",
    "devDependencies": {
        "babel-eslint": "^6.1.2",
        "babel-plugin-module-resolver": "^2.3.0",
        "babel-preset-airbnb": "^1.1.1",
        "babel-preset-react-native": "1.9.0",
        "eslint": "^3.3.1",
        "eslint-config-airbnb": "^10.0.1",
        "eslint-plugin-import": "^1.14.0",
        "eslint-plugin-jsx-a11y": "^2.1.0",
        "eslint-plugin-prefer-object-spread": "^1.1.0",
        "eslint-plugin-react": "^6.1.2",
        "gitbook-cli": "^2.3.0",
        "lodash": "^4.17.2",
        "react": "~15.4.1",
        "react-native": "^0.42.0"
    },
    "directories": {},
    "dist": {
        "shasum": "f0b928f0bef5036472dcd8175f14838884962cad",
        "tarball": "https://registry.npmjs.org/react-native-maps/-/react-native-maps-0.14.0.tgz"
    },
    "gitHead": "4849de52b2af70225c8bf3393fc3452f186acd07",
    "homepage": "https://github.com/airbnb/react-native-maps#readme",
    "keywords": [
        "react",
        "react-native",
        "react-component",
        "map",
        "mapview",
        "google-maps",
        "mapkit"
    ],
    "main": "index.js",
    "maintainers": [
        {
            "name": "airbnb"
        },
        {
            "name": "cdro"
        },
        {
            "name": "gilbox"
        },
        {
            "name": "intelligibabble"
        },
        {
            "name": "jrichardlai"
        },
        {
            "name": "spikebrehm"
        }
    ],
    "name": "react-native-maps",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": ">=15.4.0",
        "react-native": ">=0.40"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/airbnb/react-native-maps.git"
    },
    "rnpm": {
        "android": {
            "sourceDir": "./android"
        }
    },
    "scripts": {
        "build": "npm run build:js && npm run build:android && npm run build:ios",
        "build:android": "./gradlew :react-native-maps:assembleDebug",
        "build:ios": "bundle install --binstubs ./examples/ios && bundle exec pod install --project-directory=./example/ios/",
        "build:js": "exit 0",
        "ci": "npm run lint",
        "lint": "eslint ./",
        "preversion": "./scripts/update-version.js",
        "run:android": "./gradlew installDebug && npm run start:android",
        "run:ios": "react-native run-ios --project-path ./example/ios",
        "run:packager": "./node_modules/react-native/packager/packager.sh",
        "start": "node node_modules/react-native/local-cli/cli.js start",
        "start:android": "adb shell am start -n com.airbnb.android.react.maps.example/.MainActivity"
    },
    "version": "0.14.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
