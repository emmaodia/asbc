1. What information is held for an Ethereum Account?

- Nonce
- Balance
- Storage Root
- Code hash

2. Where is the full Ethereum State held?

- The World State is a mapping between addressess and account states. It is not stored on the Blockchain. It is assummed that the implemetation will maintain this mapping in a modified Merkle Patricia Trie.

3. What is a replay attack? Which two pieces of information can prevent it?

- Replay Attack, or Replay Attack, happens when a malicious actor intercepts and then repeats a valid data transmission that goes through a network
- Start counting nonce from 1.
- Use Keccak hashing for `address(this)`

4. WHat checks are made on Transactions for `view` functions?

- View functions do not perform any state changes. Therefore they do not count for transactions.
