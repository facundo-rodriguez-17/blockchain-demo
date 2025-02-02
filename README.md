# Blockchain Demo
A web-based demonstration of blockchain concepts.

This is a very basic visual introduction to the concepts behind a blockchain. We introduce
the idea of an immutable ledger using an interactive web demo.

## Setup
Get the code:

```
git clone https://github.com/facundo-rodriguez-17/blockchain-demo
```

Install dependencies:

```
cd blockchain-demo
npm install
```
Run the server:

```
npm start
```

Point a web browser at the demo:

```
http://localhost:3000
```

## Setup using Docker

Get the code:

```
git clone https://github.com/facundo-rodriguez-17/blockchain-demo
```

Run the Docker setup:

```
cd blockchain-demo
docker-compose up -d
```

Point a web browser at the demo:

```
http://localhost:3000
```

## Optional Configuration
You can adjust the "number of zeros" required by the demo by editing the first two lines of
`public/javascripts/blockchain.js`.

Because there are 16 possible characters in a hex value, each time you increment the difficulty
by one you make the puzzle 16 times harder. In my testing, a difficulty of 6 requires a
maximumNonce well over 500,000,000.

If you adjust the difficulty above 4, blocks will show up as not mined because the demo data
assumes 4 zeros for a signed block. For example, on the `http://localhost:3000/block` page
with a difficulty of 6, the first nonce that works is `8719932` yielding a hash of
`000000669445c22167511857d8f3b822b331c3342f25dfdcb326e35c1a7aa267`.

In the production bitcoin blockchain, block `458091` has the hash digest
`00000000000000000000011246f099d94f91628d71c9d75ad2f9a06e2beb7e92`. That's 21 zeros in a row!

### Public Private Key Demo

The 2nd part of the 101 session:
* https://github.com/facundo-rodriguez-17/public-private-key-demo

## Send Thanks

Bitcoin gratefully accepted: `1CxjiLtSBPAYt3vgFmoXrVTegkPTh2D2Rs`
