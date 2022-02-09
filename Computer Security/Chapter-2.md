## Symmetric Encryption

Data Encryption Standard - DES
Advanced Encryption Standard - AES

Both are block encryption algorithms

Symmetric encryption - aka conventional encryption or single-key encryption

A single-key encryptions has 5 parts:
1. Plaintext
2. Encryption algorithm - performs various substitutions and transformations on plaintext
3. Secret key - is also input to the encryption algorithm. The exact substitution and transformations peformed by the algorithm depend on the key.
4. Ciphertext - the scrambled message produces as the output
5. Decryption algorithm - the encryption algorithm run in reverse. It takes the ciphertext and the secret key and produces the original plaintext.

### Symmetric Block Encryption Algorithms

Data Encryptions Standards - DES
Advanced Encryption Standards - AES

**Block ciphers** - algorithms that encode data one block at a time (a block can be 64, 128 etc) bits

**Stream cipher** - encrypts one byte at a time (it can be configured for each bit or chunks greater than 1 byte)


### Message Authentication and Hash Functions (MAC)

![Message Authentication Code diagram](Message-Authentication-Code.png)

Protection against **active attacks**

The MAC takes in the message, key and runs it through the MAC algorithm. Then when it sends the message it will attach this enciphered block to the actual message.

The receiver will then be able to decrypt (using the key) and verify the authenticity of the message.

### One-Way Hash Function

Hash function - takes input and maps to some output according to an algorithm

Properties of hash functions:

1. **one way (preimage) resistant**
E.g  For any h - code you can't find x such as H(x) = h
$$ H(x) = h $$

2. **second preimage resistant(weak collision resistant)**

$$ y \ne x; \space H(y) = H(x) $$

3. **collision resistant (strong collision resistant)**
Infeasible to find a pair
$$ (x, y) \space such \space as \space H(x) = H(y) $$

### Applications of Hash Functions

1. Passwords
2. Intrusion Detection

### Public key Encryption

**assymetric** - uses 2 separate keys

A public-key encryption has 6 components:
1. Plaintext
2. Encryption algorithm
3. Public key
4. Private key
5. Ciphertext
6. Decryption algorithm


## Glossary and acronyms

1. ECB - Electronic block encryption
2. DES - Data Encryptions Standards
3. AES - Advanced Encryption Standards
4. SHA - Secure Hash Algorithm