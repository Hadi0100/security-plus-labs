# Lessons Learned

## Key Technical Insights
- Hashing protects stored credentials but does not eliminate cracking risk.
- Password entropy (length and unpredictability) has a much bigger impact than complexity alone.
- Salting effectively defeats rainbow table attacks.
- MFA significantly reduces the impact of credential theft.
- Weak or reused passwords remain one of the most common entry points in real breaches.

---

## Security Concepts Reinforced
- Hashing vs encryption
- Authentication factors (knowledge, possession, inherence)
- Password attack types
- Cryptographic best practices
- Access control defense strategies

---

## Personal Notes
- I underestimated how quickly weak passwords could realistically be cracked.
- Seeing the difference between short and long passwords made password policy design more intuitive.
- This lab encouraged me to audit and improve my own account security practices.

---

## Future Improvements
- Run live cracking tests using Hashcat on controlled samples.
- Compare bcrypt performance against SHA256.
- Explore MFA implementation options in lab environments.

