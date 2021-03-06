Livestreamer Twitch GUI
===
[![Supported platforms][badge-platforms]][Releases] [![Latest release][badge-release]][Releases] [![Open issues][badge-issues]][Issues]

**A multi platform [Twitch.tv][Twitch] browser for [Livestreamer][Livestreamer]**

[![Livestreamer Twitch GUI][Preview]][Releases]


## Description

This app is just a graphical user interface (GUI) on top of the [Livestreamer][Livestreamer] command line interface (CLI).  
There are still some features missing at the current stage of development, but the most important ones are working fine.

Livestreamer-Twitch-GUI is a [Node-Webkit][NodeWebkit] application, which means that it is a web application written in JavaScript ([EmberJS][EmberJS]), HTML ([Handlebars][Handlebars]) and CSS ([LessCSS][LessCSS]) and is being run by a [NodeJS][Nodejs] powered version of [Chromium][Chromium].


## When to use

One of the reasons people are having bad viewing experiences on [Twitch.tv][Twitch] is the usage of the flash player on their website. With the current generation of web browsers they sadly almost don't have any other choice but using flash for delivering a simple streaming service. There are some platforms and configurations where flash is causing problems though. These problems are low frame rates when watching streams or videos and also the lack of GPU acceleration leading to high CPU + memory usage which can be a big issue especially for mobile desktop devices.  
With Livestreamer-Twitch-GUI you're not dependent on your browser and flash, so less resources are needed. Also all streams can be watched in the video player of your choice, enabling a smooth video playback.  
Please have in mind, that by using this app you're bypassing any ads run by Twitch (adblock users also do). If you want to support Twitch or a single broadcaster, please consider buying [Twitch Turbo][TwitchTurbo] or subscribing to the broadcaster's channel. Thank you!


## Download

[Here you can find the list of all recent releases.][Releases]

You can also try out the latest unreleased version by cloning this repository and building the application off the master branch.

**Please note**: Livestreamer-Twitch-GUI depends on Livestreamer. Install [Livestreamer][Livestreamer] prior to using this application or you won't be able to launch any streams.

**Windows users**: Do not install Livestreamer via pip. Instead, use the [installation package][Installation package] (requires [Microsoft Visual C++ 2008 Redistributable Package][Microsoft Visual C++ 2008 Redistributable Package]).


## Build

Building the application on your own is simple. Just make sure that the latest stable version of [Node.js][Nodejs] (including [npm][npm]) is installed on your machine.  
Then run the following lines from the path of your cloned repository to install all dependencies and to start the build process. You will then find the built executable inside the `build/releases` folder.

```bash
npm install -g grunt-cli bower # may require administrator privileges
npm install
grunt release
```


## Contributing

Every contribution is welcome! Please read [CONTRIBUTING.md][Contributing] first.



  [Preview]: https://cloud.githubusercontent.com/assets/467294/3655974/53894240-1181-11e4-9605-1b8f058f9420.png "Preview image"
  [Releases]: https://github.com/bastimeyer/livestreamer-twitch-gui/releases "Livestreamer Twitch GUI Releases"
  [Issues]: https://github.com/bastimeyer/livestreamer-twitch-gui/issues "Livestreamer Twitch GUI Issues"
  [Contributing]: https://github.com/bastimeyer/livestreamer-twitch-gui/blob/master/CONTRIBUTING.md
  [Livestreamer]: https://github.com/chrippa/livestreamer "Livestreamer"
  [Twitch]: http://twitch.tv "Twitch.tv"
  [TwitchTurbo]: http://twitch.tv/products/turbo "Twitch Turbo"
  [NodeWebkit]: https://github.com/rogerwang/node-webkit "Node-Webkit"
  [EmberJS]: http://emberjs.com/ "EmberJS"
  [Handlebars]: http://handlebarsjs.com/ "Handlebars.js"
  [LessCSS]: http://lesscss.org/ "LessCSS"
  [Chromium]: https://www.chromium.org/ "Chromium"
  [Microsoft Visual C++ 2008 Redistributable Package]: http://www.microsoft.com/en-us/download/details.aspx?id=29 "Microsoft Visual C++ 2008 Redistributable Package"
  [Installation package]: http://livestreamer.tanuki.se/en/latest/install.html#windows-binaries "Livestreamer installation package"
  [Nodejs]: http://nodejs.org "Node.js"
  [npm]: https://npmjs.org "Node Packaged Modules"
  [badge-platforms]: https://img.shields.io/badge/platform-win%20%7C%20osx%20%7C%20linux-green.svg?style=flat-square "Supported platforms"
  [badge-release]: https://img.shields.io/github/release/bastimeyer/livestreamer-twitch-gui.svg?style=flat-square "Latest release"
  [badge-issues]: https://img.shields.io/github/issues/bastimeyer/livestreamer-twitch-gui.svg?style=flat-square "Open issues"
