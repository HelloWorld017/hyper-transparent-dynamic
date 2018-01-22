# hyper-transparent-dynamic-windows

## About
Ported version of [hyper-transparent-dynamic](https://github.com/magnus/hyper-transparent-dynamic)

## TroubleShooting
If you have error about `binding not found`, please run following commands in `~/.hyper_plugins`

```
$ npm i && npx electron-rebuild --version 1.7.10
```

## Original Document

Dynamically set the backgroundColor with transparency and apply vibrancy.
Compatible with **any** theme, pulls in existing value and adds alpha.

![hyper-transparent-dynamic-preview](preview.png)

**Note**: _See example below, load `hyper-transparent-dynamic` *after* your theme plugin._
```
module.exports = {
  ...

  config: {
    ...

    hyperTransparentDynamic: {
      alpha: 0.5 // default 50%
    },

    ...
  },

  plugins: [
    'hyper-snazzy',
    'hyper-transparent-dynamic',
  ],

  ...
}
```
