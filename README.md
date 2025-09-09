# Assignment 1 - Extend the Mini Blockchain

## How to Run 
1. Make sure Node.js is installed.
   - Confirm by running:
```
node -v
npm -v
```
3. Clone this repository or download the file.
4. Open a terminal within a project folder.
5. Run:
```
node blockchain.js
```

## Screenshots of Terminal:
### Mined Blocks
![Image](https://github.com/user-attachments/assets/b39646b0-e419-468d-b08c-41d8ff6c1e75)

## Full Chain
![Image](https://github.com/user-attachments/assets/716fdc37-80b9-4f5d-b983-1b50d020647e)
![Image](https://github.com/user-attachments/assets/e303d5c3-57be-48d3-a560-00a05db7ebc3)

## Valid Chain = true & Tampered Chain = false
![Image](https://github.com/user-attachments/assets/7565da1c-b4e2-4216-baef-d7eb2d78f0f9)

## Reflection

While doing this assignment, I learned quite a bit about hashing and immutability. I learned that hashing is similar to a digital fingerprint, where even small, slight changes in a block's transaction produce an entirely different hash. Because of this, blockchains are immutable because once that block is mined, its data cannot be changed without breaking the chain. Altering a block without breaking the chain is impossible unless the block is remade and remined. 

Proof-of-Work makes blockchains secure because it makes the mining process computationally expensive. This process is intentionally difficult so that creating a new block takes time and effort. If someone changes a block, they can't just fix that one block on its own since every block after is linked to it through its has, so all the other blocks would have to be recalculated and re-mined to keep the chain valid. For example, an attacker would have to re-mine that block and all the blocks that come after it. That would take a huge amount of time and computer power, which makes it impossible to tamper with. In real-world networks with many blocks and high mining difficulty, this becomes especially true. 

Something that surprised me while coding this assignment was how straightforward basic blockchain logic is, and how a small amount of code can show the power of blockchains. At first, when looking at the code, it looked rather simple and not as complex as I thought it would be. But, once you take into consideration the proof-of-work and transactions, I could see how quickly a single change to even one block affects the entire chain, displaying a blockchain's immutability. Additionally, seeing how each block depends on the previous one made me realize why blockchains are so secure and why they are difficult to tamper with. 
