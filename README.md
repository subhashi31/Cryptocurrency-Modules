# Cryptocurrency-Modules

In this project, we have implemented four cryptocurrency modules: Elliptic curve cryptography, Transactions, Script, and Block.

Elliptic curve cryptography: We implemented signing and verification in this module, by using Finite fields and elliptic curves, classes implemented are FiniteFieldElement, Point (for point on elliptic curve), Signature class to store signature object, PrivateKey class to sore private key and also public key corresponding to it. Using FiniteFieldElement class, Point and S256Field class we created S256Point class that contains signature method for signing.

Transactions: We created a tx class, a tx_in class and tx_out class and implemented various functions like: id method, hash method, serialize method, is_coinbase method, verify method, sig_hash method, etc. A transaction has four components: Version, Inputs, Outputs, Locktime. The inputs refer to bitcoins that belong to you. Each input contains four fields: Previous transaction ID, Previous transaction index, ScriptSig, Sequence. Outputs define where the bitcoins are going. Each output has two fields: Amount, ScriptPubKey.

Script: Implemented Script class for scripts, it contains parse method to parse hexadecimal input to script object , serialise method to serialise script object to hexadecimal representation add method combines to scripts to create new script object and evaluate method to evaluate script object.

Block: We created a block class and implemented various functions like: check_pow method, hash method, serialize method, target method, difficulty method, etc. The block header is metadata about the transactions included in a block. The block header consists of: Version, Previous block, Merkle root, Timestamp, Bits, Nonce.

Reference Book: Programming Bitcoin - Jimmy Song
