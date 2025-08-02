# Hashing and Digital Signatures

## Hash Functions
- Converts data into a fixed-size hash.
- One-way, deterministic, and collision-resistant.

### Popular Hash Functions
- **SHA-256**, **SHA-3**, **BLAKE2**.
- **MD5** and **SHA-1** are broken (collision attacks).

## Applications
- Data integrity verification.
- Password storage (with salt).
- Blockchain transactions.

## Digital Signatures
- Combines **hashing** and **asymmetric crypto**.
- Proves **message authenticity** and **non-repudiation**.

### Process
1. Hash the message.
2. Sign the hash using the sender’s private key.
3. Receiver verifies using sender’s public key.

### Standards
- **RSA**, **DSA**, **ECDSA**.

## Takeaways
- Hash functions ensure data integrity.
- Digital signatures authenticate messages.
