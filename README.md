# phaser-ui

Easy to use UI components for the Phaser.io game engine

Currently includes

- ProgressBar
- ProgressPie (radial progress bar)
- Toast (in-game notification)
- ToggleSlider

to use run the following in your game's `package.json` directory:

`npm install --save phaser-ui`

In files where you want to use these, import them at the top. ProgressBar for example:

```
import * as PhaserUi from 'phaser-ui';
var bar = new PhaserUi.ProgressBar(game,...);
```

## Contributing

If you'd like to contribute, thank you!
The UI components all live in `src/`, so if you want to add a file create it there and include it in `index.js`.
Run `npm run test` to build the UI components with Webpack, install it locally to the test game in `test/src`, and start a local server to the test game.

The test directory contains a phaser game that was created with the [phaser-plus](https://github.com/rblopes/generator-phaser-plus) Yeoman generator.
To create a new state run `yo phaser-plus:state` or for a new object run `yo phaser-plus:object`.
Write code here to test components and ensure they are working.
If you modify the 'phaser-ui' source code, you will need to rerun `npm run test`, but the game's source code will live-reload in browser.
