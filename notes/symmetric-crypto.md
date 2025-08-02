# Symmetric Cryptography

Symmetric cryptography uses the same secret key for both encryption and decryption.

## Key Concepts
- **Same key**: Shared between sender and receiver.
- **Fast and efficient** for large data.

## Block Ciphers
- **AES (Advanced Encryption Standard)** is the most widely used.
- Encrypts data in fixed-size blocks (e.g., 128 bits).

## Modes of Operation
- **ECB (Electronic Codebook)**: Encrypts blocks independently (not secure).
- **CBC (Cipher Block Chaining)**: Uses IV and chaining to improve security.
- **CTR (Counter)**: Converts block cipher to stream cipher.
- **GCM (Galois/Counter Mode)**: Adds integrity checking.

## Stream Ciphers
- Encrypt data bit-by-bit.
- Example: RC4 (now considered insecure).

## Key Management
- Key must be securely distributed and stored.

## Takeaways
- Symmetric crypto is fast but relies on secure key exchange.
