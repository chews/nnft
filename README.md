# nnft
The Not Flame Thrower Token - Burning things rare or not. The NNFT challenges you to think about impermanance, value, and what does art really mean?
The Not Fame Thrower from the Boring Company was a drop of a rare item, we've taken that item and made it a digital maker of rare items.

This forge is really just a smart contract paried with IPFS pinning, but it is a fun way to look at the creation of burnable NFTS.

To get around the gas problem (hahahaha see what I did there) I'm leveraging the Matic chain, google cloud functions handle the IOT and pinning cause the arduino is too underpowered. The smartphone coordinates contract spends.

### Prizes
Use of Matic for NFT  - https://explorer-mumbai.maticvigil.com/address/0x679803912F0c4d7665df3c9346C4Ae64A65b7bC0
Pinata for IPFS pinning
IPFS for hosting burned artifacts
```
{
  IpfsHash: 'QmPCFTr3iw3n2DHkBLJsH8DK7gXjdnXKC1k3Kn7LG8zHGg',
  PinSize: 3202304,
  Timestamp: '2021-03-21T16:04:47.924Z'
}
(base) ➜  NFTminter git:(main) ✗ node test.js
{
  IpfsHash: 'QmPCFTr3iw3n2DHkBLJsH8DK7gXjdnXKC1k3Kn7LG8zHGg',
  PinSize: 3202304,
  Timestamp: '2021-03-21T16:04:47.924Z'
}
```
## Starting with the Boring Company Flamethrower

![not a flamethrower](https://images.squarespace-cdn.com/content/v1/5915617137c58104451ac5fb/1547102278389-T1626TUAKA8ENDM7YXHI/ke17ZwdGBToddI8pDm48kBbdSUIHrnfszC0Uv-s6NXNZw-zPPgdn4jUwVcJE1ZvWEtT5uBSRWt4vQZAgTJucoTqqXjS3CfNDSuuf31e0tVHVFCHbO600DSvoILJ4oa2QnThAdi_sonYsmMjm7Z6bbO87Nsj43NRAr6WuWZv5DKs/giphy.gif?format=500w)

## first we make it less boring by giving it an electronically controlled valve and add on an Arduino.
![not a flamethrower](https://pbs.twimg.com/media/Ew8qgQCU8AE9pql?format=jpg&name=medium)

## The Flamethrower is paired with a smartphone, that has a burner wallet.
This wallet also sends the request to the arduino for verification, it checks to see the presence of the NFT and if there allows the valve to open.

## Now we can quickly issue burnable tokens to folks to be used with the art piece.
https://explorer-mumbai.maticvigil.com/address/0x679803912F0c4d7665df3c9346C4Ae64A65b7bC0/transactions
```
curl -X POST -H 'Content-Type: application/json' https://us-central1-libertasswap.cloudfunctions.net/mint-nft-matic -d '{"address": "0x744D8d9d64E19669E1Cb21EB5e872e8F1BCA6646", "gas_price":"1.4"}'
```

## with token stored in the flamethrower they are held there till they are used (spent or sent to 0x0).
[![](http://img.youtube.com/vi/xESYIHffsc0/0.jpg)](http://www.youtube.com/watch?v=xESYIHffsc0 "")


