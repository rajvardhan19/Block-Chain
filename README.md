# Block Chain

<hr>
A blockchain is a distributed database secured by cryptography. It is the technology behind Bitcoin.

-> A blockchain has a list of blocks.
-> It starts with a single block, called the genesis block

```

const Block = require("./Block.js");

class Blockchain {
  constructor () {
    this.blockchain = [Block.genesis()];
  }

  get() {
    return this.blockchain;
  }

  get latestBlock() {
    return this.blockchain[this.blockchain.length - 1];
  }
};

module.exports = Blockchain;

```

