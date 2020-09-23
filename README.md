# Red Tetris

Creating a multi-player tetris using node react and socket io

### Install

Install [node](https://nodejs.org/en/) first. After that:

```
$ npm install
```

#### Launch Server

```
$ npm run  srv-dev
> red_tetrisboilerplate@0.0.1 srv-dev /home/eric/JS/red_tetris_boilerplate
> DEBUG=tetris:* babel-watch -w src src/server/main.js
```

It launches a node.js server listening for socket.io connections, that is wired to receive `ping` messages and answered to … `pong`.

#### Launch Client

```
$ npm run client-dev
> red_tetrisboilerplate@0.0.1 client-dev /home/eric/JS/red_tetris_boilerplate
> webpack-dev-server --colors --hot --inline --host 0.0.0.0 --port 8080
```


Point your browser to `http://0.0.0.0:8080/` it will load client side application. You should see `Soon, will be here a fantastic Tetris ...`, open your console and check you have :

```
[HMR] Waiting for update signal from WDS...
bundle.js:28328  action @ 14:29:58.602 ALERT_POP 
bundle.js:28340  prev state Object
bundle.js:28344  action Object
bundle.js:28352  next state Object
bundle.js:616 [WDS] Hot Module Replacement enabled.
```

URL is not yet editable in `params.js`, change it directly inside `package.json`.

As you can guess we are using webpack `hot reload` module, try to update any file under `src/client` and your browser should reload your code.

```
[WDS] App updated. Recompiling...
```


#### Test

Test, test and re-test …

Stop server, or use an other setup (//TODO)
```
$ npm run test
```
Tests are installed under `test` folder.
