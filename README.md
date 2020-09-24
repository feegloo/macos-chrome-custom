Instead of running Google Chrome in terminal with custom flags, you can install this "Chrome" app, add to Dock and use instead of Google Chrome.

Google Chrome needs to be installed separately. This app doesn't change anything about Google Chrome, everything works the same (settings, updates, etc.), except Google Chrome is run with custom flags.

By default app use flag `--disable-features=GlobalMediaControls` to disable annoying extension which controls running music, but you can modify it any way you want. See more: [main.command](https://github.com/feegloo/chrome/blob/master/Chrome.app/Contents/MacOS/main.command)

### Installation

`curl -s https://raw.githubusercontent.com/feegloo/chrome/master/install | bash`

Open "Chrome" app, then allow macOS to run app from "unidentified developer" in System Preferences / Security & Privacy / General

![](https://www.macworld.co.uk/cmsdata/features/3669596/how_to_open_mac_app_unidentified_developer_780.jpg)

### Code

App contains only 3 files:
- [main.command](https://github.com/feegloo/chrome/blob/master/Chrome.app/Contents/MacOS/main.command) shell script executed when you run app
- [cmd.icns](https://github.com/feegloo/chrome/blob/master/Chrome.app/Contents/Resources/cmd.icns) &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; app icon
- [Info.plist](https://github.com/feegloo/chrome/blob/master/Chrome.app/Contents/Info.plist) &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; app descriptor, containing mostly dummy info

App is installed at `/Applications/Chrome.app/`, but you can rename `Chrome.app` in this repo to any app name.

Treat it like a template for macOS app which runs Shell script.
