# apple-music-electron
![preview.png](https://raw.githubusercontent.com/17hoehbr/apple-music-electron/master/preview.png)
![preview_dark.png](https://raw.githubusercontent.com/17hoehbr/apple-music-electron/master/preview_dark.png)
=======
A desktop client for Apple Music using Electron.

Initially created for Linux since iTunes is not available, but also compiled for Windows for those who find iTunes too bloated. Unlike iTunes this app should comply with Windows 10's Dark Mode.

# Usage

Should be pretty straightforward. Since it's just an electron wrapper of Apple's website all features available will obviously be limited to those on Apple music's webplayer (i.e. no playlist creation).

By default electron loads beta.music.apple.com instead of the stable version because it seems to run much smoother in my testing, but if this ever raises any issues it can be disabled by clicking Alt then going to the Settings tab in the top menu that will appear.

Electron should also detect your native desktop theme and automatically apply dark mode if applicable, but this can also be manually toggled in the Settings menu.

# Install

Pre-compiled binaries available on the [release page](https://github.com/17hoehbr/apple-music-electron/releases).

**Debian / Ubuntu:**

Use the Generic Linux instructions instead if you want automatic updates. Will get around to making a PPA eventually.

  * Download latest deb [release](https://github.com/17hoehbr/apple-music-electron/releases)
  
  * Navigate to download directory (ex. /home/USERNAME/Downloads)
  
    * ```$ cd ~/Downloads```
  
    * ```$ dpkg -i apple-music-electron_*.deb```
  
  
**Arch / Manjaro:**
  
  * Install [apple-music-electron](https://aur.archlinux.org/packages/apple-music-electron/) from the AUR

    * ```$ yay -S apple-music-electron```


**Generic Linux:**

May take longer to launch than native packages due to auto updating

  * Use [AppImageLauncher](https://github.com/TheAssassin/AppImageLauncher) to install latest [AppImage release](https://github.com/17hoehbr/apple-music-electron/releases)
  
**Windows:**

  * Download and run [apple-music-electron-Setup-*.exe](https://github.com/17hoehbr/apple-music-electron/releases)
  
  
# Building from source
Requirements: YARN https://classic.yarnpkg.com/en/docs/install

1. Clone project

```$ git clone https://github.com/17hoehbr/apple-music-electron.git```

2. Navigate to folder 

```$ cd apple-music-electron```

3. Install dependencies

```$ yarn install```

4. Compile

```$ yarn dist```

Alternatively you can run the app directly from source using
```$ yarn start```

Additional outputs can be configured by modifying the target value in package.json. All options can be found here https://www.electron.build/configuration/linux

# Donate

I'm a broke college student writing this for fun. No obligation or expectation of donations given how small of a project this is, but a cup of coffee would be appreciated.

Nano (prefered): nano_3fmqtj5x9jqpis6siyekootyerdz3za5jme63a3mdrojp4jewck4xqij1gga

Bitcoin: bc1qsreqdtdkjrx90kwvkznmp2eten7jw0x9nmz7j6

Ethereum: 0xd12f64443549b0C421C1290474572Fd9843667AF

# Credits

Made with [Electron-Builder](https://www.electron.build/).

Icon created by [Tristan Edwards](https://dribbble.com/tristanedwards) and used under the [CC Attribute license](https://creativecommons.org/licenses/by/3.0/). No modifications have been made.

DRM support is provided by a custom version of electron by [castlabs](https://github.com/castlabs/electron-releases/).

Used IsmaelMartinez' unofficial [teams-for-linux client](https://github.com/IsmaelMartinez/teams-for-linux) as a reference for package.json layout.
