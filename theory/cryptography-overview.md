# 🔐 Introduction to Cryptography – Theoretical Overview

This document summarizes the foundational concepts introduced in the **"Introduction to Cryptography"** course by Wolfram U.

---

## 📘 1. What is Cryptography?

Cryptography is the science of securing communication and data through mathematical techniques. It ensures:

- **Confidentiality** – Only intended recipients can read the message.
- **Integrity** – The message is not altered during transit.
- **Authentication** – Verifying the identity of parties.
- **Non-repudiation** – Preventing denial of message origin or delivery.

---

## 🏛️ 2. Historical Ciphers

| Cipher            | Description                              | Vulnerabilities                 |
|------------------|------------------------------------------|----------------------------------|
| Caesar Cipher     | Shifts letters by a fixed number         | Easy to brute-force (26 keys)   |
| Monoalphabetic    | Substitution using a fixed mapping       | Frequency analysis               |
| Vigenère Cipher   | Uses keyword-based shifting              | Kasiski/Babbage attack          |

These classical ciphers laid the groundwork for modern cryptography.

---

## 🔑 3. Symmetric Encryption

- **Same key** is used for both encryption and decryption.
- Very fast and suitable for bulk data encryption.

**Example algorithms:**
- AES (Advanced Encryption Standard)
- DES, 3DES

> 🧠 Key management is a major challenge in symmetric cryptography.

---

## 🧾 4. Asymmetric Encryption (Public-Key Cryptography)

- Uses a **pair of keys**: public key (encrypt), private key (decrypt).
- Introduced by Diffie and Hellman in 1976.

**Example:**
- RSA – Based on the difficulty of factoring large primes.

> ✅ Solves the key distribution problem but is computationally slower.

---

## 🧮 5. Hash Functions

- One-way functions that convert data into fixed-size output.
- Commonly used for **integrity checks**, **password storage**, and **digital signatures**.

**Properties:**
- Deterministic
- Irreversible
- Collision-resistant

**Examples:**
- SHA-256
- MD5 (insecure due to collisions)

---

## ✍️ 6. Digital Signatures

- Combines **hashing** and **asymmetric cryptography**.
- Provides:
  - Authentication
  - Integrity
  - Non-repudiation

Process:
1. Sender hashes the message.
2. Signs the hash with private key.
3. Receiver verifies with sender's public key.

---

## 🤝 7. Key Exchange – Diffie–Hellman

- Enables two parties to securely agree on a shared secret over an insecure channel.
- Relies on modular exponentiation and discrete logarithms.

**Vulnerability:** Susceptible to **Man-in-the-Middle** if not authenticated.

---

## 📌 Final Notes

Cryptography is a critical part of modern digital infrastructure – securing everything from messaging apps to online banking. A good cryptographic system depends not only on the algorithm but also on proper implementation, key management, and understanding threat models.

> “Don't roll your own crypto.” – Every security expert, ever.

---

📚 *Source: Wolfram U – Introduction to Cryptography*
