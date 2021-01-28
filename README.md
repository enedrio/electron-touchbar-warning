# Quasar App (electron-touchbar-warning)

This is a reproducer of the Touch Bar warning I see, in a quasar based electron app. The warning appears when the q-input element is beeing focused (which initializes new buttons on the touch bar).

Run 
```bash
quasar dev -m electron
```
and click on the input field. You should see the following warning in the log of the main process:
```
2021-01-28 10:16:50.435 Electron[97336:7876261] Warning: Expected min height of view: (<NSPopoverTouchBarItemButton: 0x7fa34ff2fbc0>) to be less than or equal to 30 but got a height of 32.000000. This error will be logged once per view in violation.
```

## Install the dependencies
```bash
yarn
```

### Start the app in development mode (hot-code reloading, error reporting, etc.)
```bash
quasar dev
```

### Lint the files
```bash
yarn run lint
```

### Build the app for production
```bash
quasar build
```

### Customize the configuration
See [Configuring quasar.conf.js](https://quasar.dev/quasar-cli/quasar-conf-js).
