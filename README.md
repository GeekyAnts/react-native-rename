# @geekrishabh/rn-rename [![NPM version](https://img.shields.io/npm/v/@geekrishabh/rn-rename.svg?style=flat)](https://www.npmjs.com/package/@geekrishabh/rn-rename) [![NPM monthly downloads](https://img.shields.io/npm/dm/@geekrishabh/rn-rename.svg?style=flat)](https://npm-stat.com/charts.html?package=@geekrishabh/rn-rename) [![NPM total downloads](https://img.shields.io/npm/dt/@geekrishabh/rn-rename.svg?style=flat)](https://npm-stat.com/charts.html?package=@geekrishabh/rn-rename) 

Rename react-native app with just one command

![react-native-rename](https://cloud.githubusercontent.com/assets/5106887/24444940/cbcb0a58-149a-11e7-9714-2c7bf5254b0d.gif)

> This package assumes that you created your react-native project using `react-native init`.

**Note:** This package does not attempt to properly rename build artifacts such as `ios/build` or Cocoa Pod installation targets. After renaming your project you should clean, build, and reinstall third party dependencies to get it running properly with the new name.

### Usage
```
$ npx @geekrishabh/rn-rename <newName>
```

> With custom Bundle Identifier (Android only. For iOS, please use Xcode)
```
$ npx @geekrishabh/rn-rename <newName> -b <bundleIdentifier>
```

### Example

##### First, Switch to new branch (optional but recommended)
```
$ git checkout -b rename-app
```
##### Then, Rename your app
```
$ npx @geekrishabh/rn-rename "Travel App"
```
> With custom Bundle Identifier
```
$ npx @geekrishabh/rn-rename "Travel App" -b com.geekyants.travelapp
```

### Local installation
With **Yarn**:
```
$ yarn global add @geekrishabh/rn-rename
```
With **npm**:
```
$ npm install @geekrishabh/rn-rename -g
```


