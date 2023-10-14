# Airdrop-Smart-Contract

The `whitelist` mapping keeps track of whitelisted addresses. 
The `merkleRoot` variable stores the root hash of the Merkle tree. 
The `addToWhitelist` and `removeFromWhitelist` functions allow the contract owner to add or remove addresses from the whitelist. 
The `claimTokens` function is used by whitelisted addresses to claim their tokens. It requires the address to be whitelisted and verifies the Merkle proof provided by the user against the Merkle root hash. If the proof is valid, the desired token transfer or action can be performed. 
The `verifyProof` function checks the validity of the Merkle proof by hashing the leaf node (address) along with the proof elements and comparing it to the Merkle root. 
The `getNodeHash` function calculates the hash of an address node in the Merkle tree.
