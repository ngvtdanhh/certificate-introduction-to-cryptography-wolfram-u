# ✍️ Digital Signature Explained

A **digital signature** is the cryptographic equivalent of a handwritten signature or a stamped seal. It provides proof that a digital message or document was created and sent by a known sender (authentication), and that it was not altered in transit (integrity).

---

## 🧩 How It Works

Digital signatures are built using **asymmetric cryptography** and **hashing**.

### Step-by-step Process:

1. **Message Hashing**  
   The sender hashes the original message using a cryptographic hash function (e.g., SHA-256).  
   → This produces a fixed-size **digest**.

2. **Signature Creation**  
   The sender encrypts the hash using their **private key**.  
   → This encrypted digest is the **digital signature**.

3. **Message Transmission**  
   The sender sends the **original message + signature** to the receiver.

4. **Signature Verification**  
   - Receiver hashes the received message again.
   - Decrypts the signature using the sender's **public key**.
   - Compares the result with their own hash.

> ✅ If the hashes match → Signature is valid  
> ❌ If they don't → Message was altered or not from the claimed sender

---

## 🔐 Why Use Hashing?

- Ensures consistent input size for encryption
- Increases performance
- Detects even small changes in the message

---

## ✅ What It Provides

| Property         | Explanation                                                   |
|------------------|---------------------------------------------------------------|
| **Authentication** | Verifies the identity of the sender                        |
| **Integrity**       | Detects any tampering with the message                     |
| **Non-repudiation**| Sender cannot deny sending the message                      |

---

## 📦 Real-World Use Cases

- **Software distribution**: Verifying integrity of packages (e.g., `.deb`, `.msi`)
- **Email signing (PGP, S/MIME)**: Prove authenticity of sender
- **Blockchain & smart contracts**: Confirm ownership and actions
- **Electronic contracts**: Legally binding signatures

---

## ⚠️ Limitations

- **Signature reuse**: Never reuse digital signatures.
- **Private key safety**: Compromised private key breaks the whole scheme.
- **Certificate trust**: Must trust the sender's public key (e.g., via PKI or manual verification).

---

## 📚 Summary

Digital signatures are fundamental to **secure digital communication**. They rely on solid cryptographic foundations to verify authenticity, prevent tampering, and ensure accountability in an increasingly digital world.

> “Trust, but verify – with math.” 🔐
