# api documentation for  [bitcoin (v3.0.1)](https://github.com/freewil/node-bitcoin#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-bitcoin.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-bitcoin) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bitcoin.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bitcoin)
#### Communicate with bitcoind via JSON-RPC

[![NPM](https://nodei.co/npm/bitcoin.png?downloads=true)](https://www.npmjs.com/package/bitcoin)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bitcoin/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-bitcoin%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bitcoin/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-bitcoin/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-bitcoin/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Bill Casarin",
        "email": "bill@casarin.ca",
        "url": "jb55.com"
    },
    "bugs": {
        "url": "https://github.com/freewil/node-bitcoin/issues"
    },
    "contributors": [
        {
            "name": "Sean Lavine",
            "email": "sean@eternalrise.com"
        }
    ],
    "dependencies": {},
    "description": "Communicate with bitcoind via JSON-RPC",
    "devDependencies": {
        "clone": "^1.0.2",
        "mocha": "^2.3.3",
        "standard": "^5.3.1"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "ff9e0b62a71bbb8adddb34ee2e427dac21c1096f",
        "tarball": "https://registry.npmjs.org/bitcoin/-/bitcoin-3.0.1.tgz"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "e956310d4379b85ef76d4c79d0b9bb97fa856d25",
    "homepage": "https://github.com/freewil/node-bitcoin#readme",
    "keywords": [
        "bitcoin",
        "rpc"
    ],
    "license": "Unlicense",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "freewil",
            "email": "sean@eternalrise.com"
        }
    ],
    "name": "bitcoin",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/freewil/node-bitcoin.git"
    },
    "scripts": {
        "pretest": "standard --verbose",
        "test": "make test"
    },
    "version": "3.0.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module bitcoin](#apidoc.module.bitcoin)
1.  [function <span class="apidocSignatureSpan">bitcoin.</span>Client (opts)](#apidoc.element.bitcoin.Client)
1.  object <span class="apidocSignatureSpan">bitcoin.</span>Client.prototype
1.  object <span class="apidocSignatureSpan">bitcoin.</span>jsonrpc

#### [module bitcoin.Client](#apidoc.module.bitcoin.Client)
1.  [function <span class="apidocSignatureSpan">bitcoin.</span>Client (opts)](#apidoc.element.bitcoin.Client.Client)

#### [module bitcoin.Client.prototype](#apidoc.module.bitcoin.Client.prototype)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>addMultiSigAddress ()](#apidoc.element.bitcoin.Client.prototype.addMultiSigAddress)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>addNode ()](#apidoc.element.bitcoin.Client.prototype.addNode)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>backupWallet ()](#apidoc.element.bitcoin.Client.prototype.backupWallet)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>cmd ()](#apidoc.element.bitcoin.Client.prototype.cmd)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>createMultiSig ()](#apidoc.element.bitcoin.Client.prototype.createMultiSig)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>createRawTransaction ()](#apidoc.element.bitcoin.Client.prototype.createRawTransaction)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>decodeRawTransaction ()](#apidoc.element.bitcoin.Client.prototype.decodeRawTransaction)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>decodeScript ()](#apidoc.element.bitcoin.Client.prototype.decodeScript)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>dumpPrivKey ()](#apidoc.element.bitcoin.Client.prototype.dumpPrivKey)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>dumpWallet ()](#apidoc.element.bitcoin.Client.prototype.dumpWallet)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>encryptWallet ()](#apidoc.element.bitcoin.Client.prototype.encryptWallet)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>estimateFee ()](#apidoc.element.bitcoin.Client.prototype.estimateFee)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>estimatePriority ()](#apidoc.element.bitcoin.Client.prototype.estimatePriority)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>generate ()](#apidoc.element.bitcoin.Client.prototype.generate)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getAccount ()](#apidoc.element.bitcoin.Client.prototype.getAccount)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getAccountAddress ()](#apidoc.element.bitcoin.Client.prototype.getAccountAddress)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getAddedNodeInfo ()](#apidoc.element.bitcoin.Client.prototype.getAddedNodeInfo)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getAddressesByAccount ()](#apidoc.element.bitcoin.Client.prototype.getAddressesByAccount)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBalance ()](#apidoc.element.bitcoin.Client.prototype.getBalance)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBestBlockHash ()](#apidoc.element.bitcoin.Client.prototype.getBestBlockHash)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBlock ()](#apidoc.element.bitcoin.Client.prototype.getBlock)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBlockCount ()](#apidoc.element.bitcoin.Client.prototype.getBlockCount)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBlockHash ()](#apidoc.element.bitcoin.Client.prototype.getBlockHash)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBlockTemplate ()](#apidoc.element.bitcoin.Client.prototype.getBlockTemplate)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBlockchainInfo ()](#apidoc.element.bitcoin.Client.prototype.getBlockchainInfo)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getChainTips ()](#apidoc.element.bitcoin.Client.prototype.getChainTips)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getConnectionCount ()](#apidoc.element.bitcoin.Client.prototype.getConnectionCount)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getDifficulty ()](#apidoc.element.bitcoin.Client.prototype.getDifficulty)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getGenerate ()](#apidoc.element.bitcoin.Client.prototype.getGenerate)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getInfo ()](#apidoc.element.bitcoin.Client.prototype.getInfo)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getMempoolInfo ()](#apidoc.element.bitcoin.Client.prototype.getMempoolInfo)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getMiningInfo ()](#apidoc.element.bitcoin.Client.prototype.getMiningInfo)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getNetTotals ()](#apidoc.element.bitcoin.Client.prototype.getNetTotals)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getNetworkHashPs ()](#apidoc.element.bitcoin.Client.prototype.getNetworkHashPs)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getNetworkInfo ()](#apidoc.element.bitcoin.Client.prototype.getNetworkInfo)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getNewAddress ()](#apidoc.element.bitcoin.Client.prototype.getNewAddress)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getPeerInfo ()](#apidoc.element.bitcoin.Client.prototype.getPeerInfo)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getRawChangeAddress ()](#apidoc.element.bitcoin.Client.prototype.getRawChangeAddress)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getRawMemPool ()](#apidoc.element.bitcoin.Client.prototype.getRawMemPool)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getRawTransaction ()](#apidoc.element.bitcoin.Client.prototype.getRawTransaction)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getReceivedByAccount ()](#apidoc.element.bitcoin.Client.prototype.getReceivedByAccount)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getReceivedByAddress ()](#apidoc.element.bitcoin.Client.prototype.getReceivedByAddress)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getTransaction ()](#apidoc.element.bitcoin.Client.prototype.getTransaction)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getTxOut ()](#apidoc.element.bitcoin.Client.prototype.getTxOut)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getTxOutProof ()](#apidoc.element.bitcoin.Client.prototype.getTxOutProof)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getTxOutSetInfo ()](#apidoc.element.bitcoin.Client.prototype.getTxOutSetInfo)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getUnconfirmedBalance ()](#apidoc.element.bitcoin.Client.prototype.getUnconfirmedBalance)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getWalletInfo ()](#apidoc.element.bitcoin.Client.prototype.getWalletInfo)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>help ()](#apidoc.element.bitcoin.Client.prototype.help)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>importAddress ()](#apidoc.element.bitcoin.Client.prototype.importAddress)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>importPrivKey ()](#apidoc.element.bitcoin.Client.prototype.importPrivKey)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>importWallet ()](#apidoc.element.bitcoin.Client.prototype.importWallet)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>keyPoolRefill ()](#apidoc.element.bitcoin.Client.prototype.keyPoolRefill)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>keypoolRefill ()](#apidoc.element.bitcoin.Client.prototype.keypoolRefill)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listAccounts ()](#apidoc.element.bitcoin.Client.prototype.listAccounts)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listAddressGroupings ()](#apidoc.element.bitcoin.Client.prototype.listAddressGroupings)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listLockUnspent ()](#apidoc.element.bitcoin.Client.prototype.listLockUnspent)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listReceivedByAccount ()](#apidoc.element.bitcoin.Client.prototype.listReceivedByAccount)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listReceivedByAddress ()](#apidoc.element.bitcoin.Client.prototype.listReceivedByAddress)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listSinceBlock ()](#apidoc.element.bitcoin.Client.prototype.listSinceBlock)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listTransactions ()](#apidoc.element.bitcoin.Client.prototype.listTransactions)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listUnspent ()](#apidoc.element.bitcoin.Client.prototype.listUnspent)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>lockUnspent ()](#apidoc.element.bitcoin.Client.prototype.lockUnspent)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>move ()](#apidoc.element.bitcoin.Client.prototype.move)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>ping ()](#apidoc.element.bitcoin.Client.prototype.ping)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>prioritiseTransaction ()](#apidoc.element.bitcoin.Client.prototype.prioritiseTransaction)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>sendFrom ()](#apidoc.element.bitcoin.Client.prototype.sendFrom)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>sendMany ()](#apidoc.element.bitcoin.Client.prototype.sendMany)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>sendRawTransaction ()](#apidoc.element.bitcoin.Client.prototype.sendRawTransaction)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>sendToAddress ()](#apidoc.element.bitcoin.Client.prototype.sendToAddress)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>setAccount ()](#apidoc.element.bitcoin.Client.prototype.setAccount)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>setGenerate ()](#apidoc.element.bitcoin.Client.prototype.setGenerate)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>setTxFee ()](#apidoc.element.bitcoin.Client.prototype.setTxFee)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>signMessage ()](#apidoc.element.bitcoin.Client.prototype.signMessage)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>signRawTransaction ()](#apidoc.element.bitcoin.Client.prototype.signRawTransaction)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>stop ()](#apidoc.element.bitcoin.Client.prototype.stop)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>submitBlock ()](#apidoc.element.bitcoin.Client.prototype.submitBlock)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>validateAddress ()](#apidoc.element.bitcoin.Client.prototype.validateAddress)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>verifyChain ()](#apidoc.element.bitcoin.Client.prototype.verifyChain)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>verifyMessage ()](#apidoc.element.bitcoin.Client.prototype.verifyMessage)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>verifyTxOutProof ()](#apidoc.element.bitcoin.Client.prototype.verifyTxOutProof)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>walletLock ()](#apidoc.element.bitcoin.Client.prototype.walletLock)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>walletPassphrase ()](#apidoc.element.bitcoin.Client.prototype.walletPassphrase)
1.  [function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>walletPassphraseChange ()](#apidoc.element.bitcoin.Client.prototype.walletPassphraseChange)

#### [module bitcoin.jsonrpc](#apidoc.module.bitcoin.jsonrpc)
1.  [function <span class="apidocSignatureSpan">bitcoin.jsonrpc.</span>Client (opts)](#apidoc.element.bitcoin.jsonrpc.Client)



# <a name="apidoc.module.bitcoin"></a>[module bitcoin](#apidoc.module.bitcoin)

#### <a name="apidoc.element.bitcoin.Client"></a>[function <span class="apidocSignatureSpan">bitcoin.</span>Client (opts)](#apidoc.element.bitcoin.Client)
- description and source-code
```javascript
function Client(opts) {
  this.rpc = new rpc.Client(opts)
}
```
- example usage
```shell
...
'npm install bitcoin'

## Examples

### Create client
'''js
// all config options are optional
var client = new bitcoin.Client({
  host: 'localhost',
  port: 8332,
  user: 'username',
  pass: 'password',
  timeout: 30000
});
'''
...
```



# <a name="apidoc.module.bitcoin.Client"></a>[module bitcoin.Client](#apidoc.module.bitcoin.Client)

#### <a name="apidoc.element.bitcoin.Client.Client"></a>[function <span class="apidocSignatureSpan">bitcoin.</span>Client (opts)](#apidoc.element.bitcoin.Client.Client)
- description and source-code
```javascript
function Client(opts) {
  this.rpc = new rpc.Client(opts)
}
```
- example usage
```shell
...
'npm install bitcoin'

## Examples

### Create client
'''js
// all config options are optional
var client = new bitcoin.Client({
  host: 'localhost',
  port: 8332,
  user: 'username',
  pass: 'password',
  timeout: 30000
});
'''
...
```



# <a name="apidoc.module.bitcoin.Client.prototype"></a>[module bitcoin.Client.prototype](#apidoc.module.bitcoin.Client.prototype)

#### <a name="apidoc.element.bitcoin.Client.prototype.addMultiSigAddress"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>addMultiSigAddress ()](#apidoc.element.bitcoin.Client.prototype.addMultiSigAddress)
- description and source-code
```javascript
addMultiSigAddress = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.addNode"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>addNode ()](#apidoc.element.bitcoin.Client.prototype.addNode)
- description and source-code
```javascript
addNode = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.backupWallet"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>backupWallet ()](#apidoc.element.bitcoin.Client.prototype.backupWallet)
- description and source-code
```javascript
backupWallet = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.cmd"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>cmd ()](#apidoc.element.bitcoin.Client.prototype.cmd)
- description and source-code
```javascript
cmd = function () {
  var args = [].slice.call(arguments)
  var cmd = args.shift()

  callRpc(cmd, args, this.rpc)
}
```
- example usage
```shell
...
  if (err) return console.log(err);
  console.log('Balance:', balance);
});
'''
### Getting the balance directly using 'cmd'

'''js
client.cmd('getbalance', '*', 6, function(err, balance, resHeaders){
  if (err) return console.log(err);
  console.log('Balance:', balance);
});
'''

### Batch multiple RPC calls into single HTTP request
...
```

#### <a name="apidoc.element.bitcoin.Client.prototype.createMultiSig"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>createMultiSig ()](#apidoc.element.bitcoin.Client.prototype.createMultiSig)
- description and source-code
```javascript
createMultiSig = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.createRawTransaction"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>createRawTransaction ()](#apidoc.element.bitcoin.Client.prototype.createRawTransaction)
- description and source-code
```javascript
createRawTransaction = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.decodeRawTransaction"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>decodeRawTransaction ()](#apidoc.element.bitcoin.Client.prototype.decodeRawTransaction)
- description and source-code
```javascript
decodeRawTransaction = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.decodeScript"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>decodeScript ()](#apidoc.element.bitcoin.Client.prototype.decodeScript)
- description and source-code
```javascript
decodeScript = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.dumpPrivKey"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>dumpPrivKey ()](#apidoc.element.bitcoin.Client.prototype.dumpPrivKey)
- description and source-code
```javascript
dumpPrivKey = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.dumpWallet"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>dumpWallet ()](#apidoc.element.bitcoin.Client.prototype.dumpWallet)
- description and source-code
```javascript
dumpWallet = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.encryptWallet"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>encryptWallet ()](#apidoc.element.bitcoin.Client.prototype.encryptWallet)
- description and source-code
```javascript
encryptWallet = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.estimateFee"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>estimateFee ()](#apidoc.element.bitcoin.Client.prototype.estimateFee)
- description and source-code
```javascript
estimateFee = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.estimatePriority"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>estimatePriority ()](#apidoc.element.bitcoin.Client.prototype.estimatePriority)
- description and source-code
```javascript
estimatePriority = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.generate"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>generate ()](#apidoc.element.bitcoin.Client.prototype.generate)
- description and source-code
```javascript
generate = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getAccount"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getAccount ()](#apidoc.element.bitcoin.Client.prototype.getAccount)
- description and source-code
```javascript
getAccount = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getAccountAddress"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getAccountAddress ()](#apidoc.element.bitcoin.Client.prototype.getAccountAddress)
- description and source-code
```javascript
getAccountAddress = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getAddedNodeInfo"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getAddedNodeInfo ()](#apidoc.element.bitcoin.Client.prototype.getAddedNodeInfo)
- description and source-code
```javascript
getAddedNodeInfo = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getAddressesByAccount"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getAddressesByAccount ()](#apidoc.element.bitcoin.Client.prototype.getAddressesByAccount)
- description and source-code
```javascript
getAddressesByAccount = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getBalance"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBalance ()](#apidoc.element.bitcoin.Client.prototype.getBalance)
- description and source-code
```javascript
getBalance = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
...
  timeout: 30000
});
'''

### Get balance across all accounts with minimum confirmations of 6

'''js
client.getBalance('*', 6, function(err, balance, resHeaders) {
  if (err) return console.log(err);
  console.log('Balance:', balance);
});
'''
### Getting the balance directly using 'cmd'

'''js
...
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getBestBlockHash"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBestBlockHash ()](#apidoc.element.bitcoin.Client.prototype.getBestBlockHash)
- description and source-code
```javascript
getBestBlockHash = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getBlock"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBlock ()](#apidoc.element.bitcoin.Client.prototype.getBlock)
- description and source-code
```javascript
getBlock = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getBlockCount"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBlockCount ()](#apidoc.element.bitcoin.Client.prototype.getBlockCount)
- description and source-code
```javascript
getBlockCount = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getBlockHash"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBlockHash ()](#apidoc.element.bitcoin.Client.prototype.getBlockHash)
- description and source-code
```javascript
getBlockHash = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getBlockTemplate"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBlockTemplate ()](#apidoc.element.bitcoin.Client.prototype.getBlockTemplate)
- description and source-code
```javascript
getBlockTemplate = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getBlockchainInfo"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getBlockchainInfo ()](#apidoc.element.bitcoin.Client.prototype.getBlockchainInfo)
- description and source-code
```javascript
getBlockchainInfo = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getChainTips"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getChainTips ()](#apidoc.element.bitcoin.Client.prototype.getChainTips)
- description and source-code
```javascript
getChainTips = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getConnectionCount"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getConnectionCount ()](#apidoc.element.bitcoin.Client.prototype.getConnectionCount)
- description and source-code
```javascript
getConnectionCount = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getDifficulty"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getDifficulty ()](#apidoc.element.bitcoin.Client.prototype.getDifficulty)
- description and source-code
```javascript
getDifficulty = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getGenerate"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getGenerate ()](#apidoc.element.bitcoin.Client.prototype.getGenerate)
- description and source-code
```javascript
getGenerate = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getInfo"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getInfo ()](#apidoc.element.bitcoin.Client.prototype.getInfo)
- description and source-code
```javascript
getInfo = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getMempoolInfo"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getMempoolInfo ()](#apidoc.element.bitcoin.Client.prototype.getMempoolInfo)
- description and source-code
```javascript
getMempoolInfo = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getMiningInfo"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getMiningInfo ()](#apidoc.element.bitcoin.Client.prototype.getMiningInfo)
- description and source-code
```javascript
getMiningInfo = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getNetTotals"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getNetTotals ()](#apidoc.element.bitcoin.Client.prototype.getNetTotals)
- description and source-code
```javascript
getNetTotals = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getNetworkHashPs"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getNetworkHashPs ()](#apidoc.element.bitcoin.Client.prototype.getNetworkHashPs)
- description and source-code
```javascript
getNetworkHashPs = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getNetworkInfo"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getNetworkInfo ()](#apidoc.element.bitcoin.Client.prototype.getNetworkInfo)
- description and source-code
```javascript
getNetworkInfo = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getNewAddress"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getNewAddress ()](#apidoc.element.bitcoin.Client.prototype.getNewAddress)
- description and source-code
```javascript
getNewAddress = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getPeerInfo"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getPeerInfo ()](#apidoc.element.bitcoin.Client.prototype.getPeerInfo)
- description and source-code
```javascript
getPeerInfo = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getRawChangeAddress"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getRawChangeAddress ()](#apidoc.element.bitcoin.Client.prototype.getRawChangeAddress)
- description and source-code
```javascript
getRawChangeAddress = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getRawMemPool"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getRawMemPool ()](#apidoc.element.bitcoin.Client.prototype.getRawMemPool)
- description and source-code
```javascript
getRawMemPool = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getRawTransaction"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getRawTransaction ()](#apidoc.element.bitcoin.Client.prototype.getRawTransaction)
- description and source-code
```javascript
getRawTransaction = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getReceivedByAccount"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getReceivedByAccount ()](#apidoc.element.bitcoin.Client.prototype.getReceivedByAccount)
- description and source-code
```javascript
getReceivedByAccount = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getReceivedByAddress"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getReceivedByAddress ()](#apidoc.element.bitcoin.Client.prototype.getReceivedByAddress)
- description and source-code
```javascript
getReceivedByAddress = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getTransaction"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getTransaction ()](#apidoc.element.bitcoin.Client.prototype.getTransaction)
- description and source-code
```javascript
getTransaction = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getTxOut"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getTxOut ()](#apidoc.element.bitcoin.Client.prototype.getTxOut)
- description and source-code
```javascript
getTxOut = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getTxOutProof"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getTxOutProof ()](#apidoc.element.bitcoin.Client.prototype.getTxOutProof)
- description and source-code
```javascript
getTxOutProof = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getTxOutSetInfo"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getTxOutSetInfo ()](#apidoc.element.bitcoin.Client.prototype.getTxOutSetInfo)
- description and source-code
```javascript
getTxOutSetInfo = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getUnconfirmedBalance"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getUnconfirmedBalance ()](#apidoc.element.bitcoin.Client.prototype.getUnconfirmedBalance)
- description and source-code
```javascript
getUnconfirmedBalance = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.getWalletInfo"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>getWalletInfo ()](#apidoc.element.bitcoin.Client.prototype.getWalletInfo)
- description and source-code
```javascript
getWalletInfo = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.help"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>help ()](#apidoc.element.bitcoin.Client.prototype.help)
- description and source-code
```javascript
help = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.importAddress"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>importAddress ()](#apidoc.element.bitcoin.Client.prototype.importAddress)
- description and source-code
```javascript
importAddress = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.importPrivKey"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>importPrivKey ()](#apidoc.element.bitcoin.Client.prototype.importPrivKey)
- description and source-code
```javascript
importPrivKey = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.importWallet"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>importWallet ()](#apidoc.element.bitcoin.Client.prototype.importWallet)
- description and source-code
```javascript
importWallet = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.keyPoolRefill"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>keyPoolRefill ()](#apidoc.element.bitcoin.Client.prototype.keyPoolRefill)
- description and source-code
```javascript
keyPoolRefill = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.keypoolRefill"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>keypoolRefill ()](#apidoc.element.bitcoin.Client.prototype.keypoolRefill)
- description and source-code
```javascript
keypoolRefill = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.listAccounts"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listAccounts ()](#apidoc.element.bitcoin.Client.prototype.listAccounts)
- description and source-code
```javascript
listAccounts = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.listAddressGroupings"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listAddressGroupings ()](#apidoc.element.bitcoin.Client.prototype.listAddressGroupings)
- description and source-code
```javascript
listAddressGroupings = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.listLockUnspent"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listLockUnspent ()](#apidoc.element.bitcoin.Client.prototype.listLockUnspent)
- description and source-code
```javascript
listLockUnspent = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.listReceivedByAccount"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listReceivedByAccount ()](#apidoc.element.bitcoin.Client.prototype.listReceivedByAccount)
- description and source-code
```javascript
listReceivedByAccount = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.listReceivedByAddress"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listReceivedByAddress ()](#apidoc.element.bitcoin.Client.prototype.listReceivedByAddress)
- description and source-code
```javascript
listReceivedByAddress = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.listSinceBlock"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listSinceBlock ()](#apidoc.element.bitcoin.Client.prototype.listSinceBlock)
- description and source-code
```javascript
listSinceBlock = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.listTransactions"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listTransactions ()](#apidoc.element.bitcoin.Client.prototype.listTransactions)
- description and source-code
```javascript
listTransactions = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.listUnspent"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>listUnspent ()](#apidoc.element.bitcoin.Client.prototype.listUnspent)
- description and source-code
```javascript
listUnspent = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.lockUnspent"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>lockUnspent ()](#apidoc.element.bitcoin.Client.prototype.lockUnspent)
- description and source-code
```javascript
lockUnspent = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.move"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>move ()](#apidoc.element.bitcoin.Client.prototype.move)
- description and source-code
```javascript
move = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.ping"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>ping ()](#apidoc.element.bitcoin.Client.prototype.ping)
- description and source-code
```javascript
ping = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.prioritiseTransaction"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>prioritiseTransaction ()](#apidoc.element.bitcoin.Client.prototype.prioritiseTransaction)
- description and source-code
```javascript
prioritiseTransaction = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.sendFrom"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>sendFrom ()](#apidoc.element.bitcoin.Client.prototype.sendFrom)
- description and source-code
```javascript
sendFrom = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.sendMany"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>sendMany ()](#apidoc.element.bitcoin.Client.prototype.sendMany)
- description and source-code
```javascript
sendMany = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.sendRawTransaction"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>sendRawTransaction ()](#apidoc.element.bitcoin.Client.prototype.sendRawTransaction)
- description and source-code
```javascript
sendRawTransaction = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.sendToAddress"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>sendToAddress ()](#apidoc.element.bitcoin.Client.prototype.sendToAddress)
- description and source-code
```javascript
sendToAddress = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.setAccount"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>setAccount ()](#apidoc.element.bitcoin.Client.prototype.setAccount)
- description and source-code
```javascript
setAccount = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.setGenerate"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>setGenerate ()](#apidoc.element.bitcoin.Client.prototype.setGenerate)
- description and source-code
```javascript
setGenerate = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.setTxFee"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>setTxFee ()](#apidoc.element.bitcoin.Client.prototype.setTxFee)
- description and source-code
```javascript
setTxFee = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.signMessage"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>signMessage ()](#apidoc.element.bitcoin.Client.prototype.signMessage)
- description and source-code
```javascript
signMessage = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.signRawTransaction"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>signRawTransaction ()](#apidoc.element.bitcoin.Client.prototype.signRawTransaction)
- description and source-code
```javascript
signRawTransaction = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.stop"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>stop ()](#apidoc.element.bitcoin.Client.prototype.stop)
- description and source-code
```javascript
stop = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.submitBlock"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>submitBlock ()](#apidoc.element.bitcoin.Client.prototype.submitBlock)
- description and source-code
```javascript
submitBlock = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.validateAddress"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>validateAddress ()](#apidoc.element.bitcoin.Client.prototype.validateAddress)
- description and source-code
```javascript
validateAddress = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.verifyChain"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>verifyChain ()](#apidoc.element.bitcoin.Client.prototype.verifyChain)
- description and source-code
```javascript
verifyChain = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.verifyMessage"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>verifyMessage ()](#apidoc.element.bitcoin.Client.prototype.verifyMessage)
- description and source-code
```javascript
verifyMessage = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.verifyTxOutProof"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>verifyTxOutProof ()](#apidoc.element.bitcoin.Client.prototype.verifyTxOutProof)
- description and source-code
```javascript
verifyTxOutProof = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.walletLock"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>walletLock ()](#apidoc.element.bitcoin.Client.prototype.walletLock)
- description and source-code
```javascript
walletLock = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.walletPassphrase"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>walletPassphrase ()](#apidoc.element.bitcoin.Client.prototype.walletPassphrase)
- description and source-code
```javascript
walletPassphrase = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bitcoin.Client.prototype.walletPassphraseChange"></a>[function <span class="apidocSignatureSpan">bitcoin.Client.prototype.</span>walletPassphraseChange ()](#apidoc.element.bitcoin.Client.prototype.walletPassphraseChange)
- description and source-code
```javascript
walletPassphraseChange = function () {
  var args = [].slice.call(arguments)
  callRpc(commands[protoFn], args, this.rpc)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bitcoin.jsonrpc"></a>[module bitcoin.jsonrpc](#apidoc.module.bitcoin.jsonrpc)

#### <a name="apidoc.element.bitcoin.jsonrpc.Client"></a>[function <span class="apidocSignatureSpan">bitcoin.jsonrpc.</span>Client (opts)](#apidoc.element.bitcoin.jsonrpc.Client)
- description and source-code
```javascript
Client = function (opts) {
  this.opts = opts || {}
  this.http = this.opts.ssl ? https : http
}
```
- example usage
```shell
...
'npm install bitcoin'

## Examples

### Create client
'''js
// all config options are optional
var client = new bitcoin.Client({
  host: 'localhost',
  port: 8332,
  user: 'username',
  pass: 'password',
  timeout: 30000
});
'''
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
