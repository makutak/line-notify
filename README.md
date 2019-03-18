# LINE-Notify

Send message to LINE from CLI.

## Requirements
* [node](https://nodejs.org/en/) (v8.10.0++)
* [npm](https://www.npmjs.com/) (v5.6.0++)

## Installation

Please clone this repository.
```bash
$ git clone https://github.com/makutak/line-notify.git
```

## QuickStart
#### Generate LINE Notify API token

https://notify-bot.line.me/en/

#### First of all, Please build this app.

``` bash
$ npm run build
```

#### send message with your LINE API token.

```bash
$ node target/main.js -t <YOUR LINE API TOKEN> -m <Message>
```
#### set your LINE API token to config file.
``` bash
$ node target/main.js -s <YOUR LINE API TOKEN>
```
* generated ```config/token.json``` which is your LINE API token's config file.

####  if set token, can send message widthout ```-t``` option.

``` bash
$ node target/main.js -m <Message>
```

## Options

``` bash
Usage: Line Notify [options] action.
Options:
  -h, --help     Show help
  -m, --message  You want to send message.
  -t, --token    Your LINE API Token.
  -s, --set      Your LINE API Token that you want to set config file.
```

## License

Copyright © 2019 t-kouno

This program and the accompanying materials are made available under the
terms of the Eclipse Public License 2.0 which is available at
http://www.eclipse.org/legal/epl-2.0.

This Source Code may also be made available under the following Secondary
Licenses when the conditions for such availability set forth in the Eclipse
Public License, v. 2.0 are satisfied: GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or (at your
option) any later version, with the GNU Classpath Exception which is available
at https://www.gnu.org/software/classpath/license.html.
