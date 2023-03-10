![line](https://github.com/fwd/n2/raw/master/.github/line.png)

<h1 align="center">Developer Nano Wallet</h1>

<h3 align="center">In Beta. Use with caution and report bugs.</h3>

![line](https://github.com/fwd/n2/raw/master/.github/line.png)

**Local:**
```html
<script src="/latest.js"></script>
```

**CDN:**
```html
<script src="https://offline.nano.to/latest.js"></script>
```

**NPM:**
```js
// npm install fwd/nano-offline
const nano = require('@fwd/nano-offline')
```

**USAGE:**
```js
;(async () => {
    
    await nano.import( await nano.generate() )

    console.log( await nano.accounts() )

    // console.log( "QR Code:", await wallet.qrcode() )
    // console.log( "Open Link:", wallet.nanolooker() )

    await nano.wait({ amount: '0.001' })

    await nano.receive()

    await nano.send({ 
        to: 'nano_1faucet7b6xjyha7m13objpn5ubkquzd6ska8kwopzf1ecbfmn35d1zey3ys', 
        amount: (await wallet.balance()).balance
    })

    // console.log(await wallet.accounts({ export: true }))

    // from RAM not Blockchain
    await nano.destroy()

})()
```

![line](https://github.com/fwd/n2/raw/master/.github/line.png)

### License

MIT (No Commercial Restrictions)

Contact [@nano2dev](mailto:support@nano.to) for licensing questions.

![line](https://github.com/fwd/n2/raw/master/.github/line.png)

### Stargazers

[![Stargazers over time](https://starchart.cc/fwd/nano-js.svg)](https://github.com/fwd/nano-js)
