# Hello DApp Example

This is a simple example showing how to connect to the **Base Testnet** using `ethers.js`.

```js
import { ethers } from "ethers";

const provider = new ethers.JsonRpcProvider("https://sepolia.base.org");

async function main() {
  const blockNumber = await provider.getBlockNumber();
  console.log("Current block number on Base Testnet:", blockNumber);
}

main();
