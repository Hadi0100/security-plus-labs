# Password Cracking Analysis

## Simulated Password Dataset

| Account | Hash Type | Password Strength |
|------------|------------|------------------|
| User-A | SHA256 | Weak |
| User-B | SHA256 | Weak |
| User-C | SHA256 | Moderate |
| User-D | SHA256 | Strong |

---

## Attack Methods Reviewed

### Dictionary Attack
Uses large lists of known passwords and variations. Highly effective against common patterns and reused credentials.

### Brute Force Attack
Attempts every possible combination. The time required grows exponentially as length and character variety increase.

### Credential Stuffing
Reuses leaked username/password combinations across multiple services. Very effective when users recycle passwords.

---

## Estimated Crack Time (Rough)

| Password Example | Length | Complexity | Approximate Time |
|------------------|-----------|---------------|------------------|
| password123 | 11 | Low | Almost instant |
| Password123 | 11 | Low | Seconds |
| L3tM3In2024 | 10 | Medium | A few minutes on consumer hardware (rough estimate) |
| F7$kL9@Q!2xZ | 12 | High | Likely many years using consumer-grade hardware |

---

## Rainbow Table Considerations
- Without salting, identical hashes can be precomputed and cracked quickly using lookup tables.
- Salting forces attackers to recompute hashes individually, significantly increasing effort and cost.

---

## Defensive Controls
- Enforce long passphrases instead of short complex passwords.
- Use modern salted hashing algorithms (bcrypt, scrypt, Argon2).
- Enable multi-factor authentication wherever possible.
- Apply account lockout and monitoring policies.
- Educate users on phishing and credential reuse risks.

---

## Practical Reflection
This lab highlighted how much password length matters compared to just adding symbols. It also reinforced how dangerous reused credentials can be when large breach datasets are available to attackers.
