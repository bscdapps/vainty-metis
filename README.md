# Vanity Metis



Browser-based Metis vanity address generator


[![Vanity-Metis](https://user-images.githubusercontent.com/75070913/169709660-e171ad7a-97f2-43e1-9e8f-aca4195d8d4d.png)

## What's a vanity address?

A vanity address is an address which part of it is chosen by yourself, making it look less random.

Examples: `0xc0ffee254729296a45a3885639AC7E10F9d54979`, or `0x999999cf1046e68e36E1aA2E0E07105eDDD1f08E`

## Usage


Enter as short prefix/suffix of your choice at the bottom of the page, and click ‘generate’ to start. Your browser will
generate lots of random addresses until one matches your input.

Once an address is found, you can reveal the private key, or click the 'save' button to download a password-encrypted keystore file.

You can increase the number of working threads to reach higher speeds, or decrease it if you computer struggles.


## Security

As explained above, everything is computed only in your browser. Nothing ever leaves your machine, or even your browser tab.
There is no database, no server-side code. Everything vanishes when you close your tab.

**Vanity-ETH cannot and will never store your private key**, and if you don't trust it, you have 3 ways to ensure your key remains private:

- Once the web page is loaded, you can turn off the internet and continue playing, it will work seamlessly)
and use it on a completely offline computer
- The code is 100% open source and available on Github. You can review it as much as you want before using it

Vanity-ETH uses a cryptographically secure pseudorandom number generator (CSPRNG) to generate Ethereum addresses.

The keystore file is encrypted with a AES-128-CTR cipher using the BKDF2-SHA256 derivation function with 65536 hashing rounds.


## Performance

For some reason, the performance of Vanity-Metis can vary a lot from a browser to another. 
Currently, Chrome provides the best results.

Using Vanity-Metis on your phone or tablet will work, but don't expect to reach the speed of a good old computer.


## Compatibility

Any address generated with Vanity-Metis is ERC-20 compatible, which means you can use it for an ICO, an airdrop, or just
to withdraw your funds from an exchange.

The keystore file is 100% compatible with , MetaMask, Mist, and geth.


## Build Vanity-ETH from source

The Travis CI bot 🤖 is in charge of building and deploying Vanity-ETH to Github pages, but you can make your own build
from source is you want

```sh
git clone 
cd vanity-metis
npm i
npm run serve
```

## Tips



