# react-native-smart-assets

Automatically generate an Images module from your image assets. Converts intelligently (e.g. PDF to @2x, @3x etc).

![](http://i.imgur.com/XS9BGzZ.png) ---Automatically--> ![](http://i.imgur.com/Z3ohY9m.png)

```js
import Images from './Images';

...

<Image source={Images.myIcon} /> // Property name is same as file name. Automatically uses @2x, @3x.
```

# Requirements

- Mac OS X or Linux.
- [GhostScript](http://www.ghostscript.com/) is required to convert PDF assets into pre-rendered PNGs for different DPIs. Mac OS X users can use `brew install gs`.

# Usage

`./convert-assets.sh /assets_directory /output_directory`

A directory named `img` and a script named `Images.js` will be added to the output directory. Existing ones will be removed.
