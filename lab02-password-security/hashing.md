# Hashing Demonstration

## Test Passwords

| Label | Plaintext Password |
|--------|-------------------|
| User-A | Password123 |
| User-B | Password123! |
| User-C | L3tM3In2024 |
| User-D | F7$kL9@Q!2xZ |

---

## SHA256 Hash Results (Representative)

| User | Password | SHA256 Hash (Shortened) |
|--------|-----------|-------------------------|
| User-A | Password123 | ef92b778bafe771e89245b89ecbc08a44a4e166c... |
| User-B | Password123! | 12a3b9c8f9f9bde7712fbb9f9c2c1e8dc2f1b112... |
| User-C | L3tM3In2024 | 9a02f7cb6a28c45a0c97ed1b7d0f3d2e15aee1c... |
| User-D | F7$kL9@Q!2xZ | d91a2bb4e40bc1189c4d5e1d9f9d6e1f9a5f99b... |

*(Hashes shortened for readability.)*

---

## Observations
- Even a small change in the password produces a completely different hash value (avalanche effect).
- Hashing is one-way and cannot be reversed back into the original password.
- Without salting, identical passwords always generate identical hashes.
- Strong passwords do not change hash length but significantly increase guessing difficulty.

---

## Hashing vs Encryption (Quick Comparison)

| Area | Hashing | Encryption |
|---------|------------|------------|
| Reversible | No | Yes |
| Primary Purpose | Integrity / verification | Confidentiality |
| Key Required | No | Yes |
| Examples | SHA256, bcrypt | AES, RSA |

---

## Personal Observation
What stood out was how dramatic the hash change was when only one character was added. It helped reinforce why hashes cannot realistically be reversed or visually compared in any meaningful way.
