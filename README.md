# kiwiirc

> The next generation of the KiwiIRC web based IRC client

### Status
This is an entirely new version of the original Kiwi IRC client. It now uses Vue.js instead of backbone.js for the javascript framework.

It almost has feature parity with the original Kiwi IRC client, the outstanding features being in the issue tracker. The original Kiwi IRC will still be supported for some time with bug and security patches but no extra features will be worked on. Only this new version will be actively developed.

If you're just looking to run Kiwi IRC and not develop or modify it then there are pre-built and ready to use packages here: https://kiwiirc.com/downloads/index.html


### Development dependencies
Before you can build or start to develop on KiwiIRC, make sure to have the
following installed on your system:
* [Nodejs](https://nodejs.org/)
* [yarn](https://yarnpkg.com/)

### Development environment

``` bash
# install dependencies
yarn install

# development web server with hot reload at http://localhost:8080/
yarn run dev
```

Source files are linted automatically and will fail on any linting errors.

### Building for production

``` bash
# install dependencies
$ yarn install

# build for production with minification
$ yarn run build
```

Built files that can be uploaded to your webserver will be placed in the dist/ folder.

### Configuration

By default, the client will load the /static/config.json file on startup which
contains any runtime configuration. When in the development environment this can
be found in [static/config.json](static/config.json)

## Getting started

If you're just looking to run Kiwi IRC and not develop or modify it then there are pre-built and ready to use packages here: https://kiwiirc.com/downloads/index.html

**Just looking to build a theme? Try the online [theme builder](https://kiwiirc.com/nextclient-themebuilder)**

This repository only contains the client side (the website). By default it will connect to IRC networks via kiwiirc.com servers while you are developing locally. To use your own server you either need to be using a websocket capable IRC server (none yet support this) or need to be connecting to a Kiwi IRC server which can be found [here](https://github.com/kiwiirc/webircgateway). 

The client side files built from this repository may be hosted anywhere - Apache, Nginx, the Kiwi IRC server, your CDN.

## Browser support

Kiwi IRC is tested on the below browsers. Other browsers are not checked and may have trouble running Kiwi IRC.
* Chrome
* Chrome Mobile (Android)
* Firefox
* IE10+
* Safari 9+

## Thanks

Providing sponsorship to the Kiwi IRC project helps keep kiwiirc.com free to use and makes the ongoing development possible.
Without these [Sponsors](sponsors.md) development would be much slower so many thanks to these!

## License
~~~
   Copyright 2017 Kiwi IRC

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
~~~
