# Attacks in Cryptography

## Types of Attacks

### Brute-force Attack
- Tries every possible key combination.
- Mitigated by long key lengths.

---

### Ciphertext-only Attack
- Attacker only has access to ciphertexts.

---

### Known-plaintext Attack
- Attacker has some pairs of plaintext and ciphertext.

---

### Chosen-plaintext & Chosen-ciphertext Attacks
- Attacker can encrypt/decrypt arbitrary inputs to gather information.

---

### Side-channel Attacks
- Exploits implementation leaks (timing, power consumption, etc.)

---

### Cryptanalysis Examples
- **Frequency Analysis**: For classical ciphers.
- **Padding Oracle Attack**
- **Birthday Attack**: Targets hash collisions.

---

## Preventive Strategies
- Use strong, tested algorithms.
- Employ secure protocols.
- Keep cryptographic libraries up to date.
