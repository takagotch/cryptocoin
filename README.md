### cryptocoin
---
https://github.com/cryptocoinjs/cryptocoin

http://cryptocoinjs.com/

```sh
npm install --save cryptocoin
component install cryptocoinjs/cryptocoin
bower install cryptocoin

npm init
npm install --save coinkey
npm install --save coinkey@1.0.0
npm install --save coinkey@latest
npm install --save-dev mocha
npm init 
touch app.js
npm install --save coinkey@1.0.0
node app.js
```

```
<script src="/path/to/cryptocoin.min.js"></script>
```

```js
var CoinKey = require('coinkey')
var ck = new CoinKey.createRandom()
console.log("Private Key (Wallet Import Format): " + ck.privateWif)
console.log("Private Key (Hex): " + ck.privateKey.toString('hex'))
console.log("Address: " + ck.publicAddress)

var CoinKey = require('coinkey')
var ck = CoinKey.fromWif('xxxx')
console.log("Address: " + ck.publicAddress)

var CoinKey = require('coinkey')

var buffer = new Buffer('xxx', 'hex')
var ck = new CoinKey(buffer)
console.log("Private Key (Wallet Import Format): " + ck.privateWif)
console.log("Private Key (Hex): " + ck.privateKey.toString('hex'))
console.log("Address: " + ck.publicAddress)

var CoinKey = require('coinkey')
var coinInfo = require('coininfo')
var dogeInfo = coinInfo('DOGE').versins
var ck = new CoinKey.createRandom(dogeinfo)
console.log("Private Key (Wallet Import Format)" + ck.privateWif)
console.log("Private Key (Hex):" + ck.privateKey.toString('hex'))
console.log("Address: " + ck.publicAddress)

var p = new Peer('example.com');
var btc = new BTCNetwork();

p.on('versionMessage', function(d) {
  var parsed = btc.parseVersionMessage(d.data);
});
```


