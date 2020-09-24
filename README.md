Instead of running Google Chrome in terminal with custom flags, you can install this app, add to Dock and use instead of Google Chrome.

Google Chrome needs to be installed separately. This app doesn't change anything about Google Chrome, everything works the same (settings, history, etc.), except Google Chrome is run with custom flags.

By default app use flag `--disable-features=GlobalMediaControls` to disable annoying extension which controls running music, but you can modify it any way you want. See more: [main.command](https://github.com/feegloo/chrome/blob/master/Chrome.app/Contents/MacOS/main.command)

### Installation

`curl -s https://raw.githubusercontent.com/feegloo/chrome/master/install | bash`
