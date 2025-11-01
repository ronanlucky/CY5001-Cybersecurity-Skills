# OpenSSL Cryptographic Operations & Digital Signatures

Duration: October 2025  
Status: Completed  
Grade: 100/100

---

## Overview

Implemented comprehensive cryptographic operations using OpenSSL toolkit, including symmetric and asymmetric encryption, digital signatures, hash functions, and cryptographic attack techniques.

---

## Core Skills Developed

### Symmetric Cryptography
- Generated random initialization vectors (IV) and keys
- Implemented AES-128-CBC encryption and decryption
- Used AES-192-CTR with salt for secure encryption
- Understood the role of IV in block cipher modes
- Performed symmetric encryption with passwords

### Asymmetric Cryptography (RSA)
- Generated 2048-bit RSA key pairs
- Extracted public keys from private keys
- Encrypted data with public keys
- Decrypted data with private keys
- Understood RSA key pair relationships

### Hash Functions
- Generated MD5 hashes (deprecated, for educational purposes)
- Created SHA-256 and SHA-512 hashes
- Understood hash function properties
- Used hashing for data integrity verification

### Digital Signatures
- Created digital signatures using RSA private keys
- Combined SHA-256/SHA-512 with RSA for signatures
- Verified signatures using public keys
- Understood non-repudiation through signatures
- Applied signatures to binary files (asciinema recordings)

### Cryptographic Attack Techniques
- Implemented MD5 hash cracking through brute force
- Used Python for automated cryptographic attacks
- Applied itertools for exhaustive search
- Understood computational complexity of attacks
- Recognized weaknesses in MD5 algorithm

### File Operations & Encoding
- Used xxd for hexadecimal file viewing
- Compared files using SHA-1 checksums
- Worked with binary and text file formats
- Transferred encrypted files securely with SCP

---

## Key OpenSSL Commands

- Random Generation: openssl rand
- RSA Keys: openssl genrsa, openssl rsa
- Symmetric Encryption: openssl aes-128-cbc, openssl enc
- Asymmetric Encryption: openssl pkeyutl
- Hashing: openssl dgst -md5/-sha256/-sha512
- Digital Signatures: openssl dgst -sign, openssl dgst -verify

---

## Cryptographic Concepts

### Symmetric vs Asymmetric
- Symmetric: Same key for encryption and decryption (faster)
- Asymmetric: Key pairs with different purposes (more secure for key exchange)
- Use cases for each approach

### Digital Signature Process
- Hash the message
- Encrypt hash with private key (signature)
- Recipient decrypts signature with public key
- Compare decrypted hash with message hash

### Initialization Vectors (IV)
- Randomness in block cipher modes
- Prevents pattern detection
- Must be unique per encryption

### Salt in Encryption
- Adds randomness to password-based encryption
- Prevents rainbow table attacks
- Makes brute force more difficult

---

## Python Scripting for Cryptography

- Automated brute-force attacks with itertools
- Efficient hash comparison loops
- Command-line integration with subprocess
- Performance optimization for cryptographic operations

---

## Key Lessons

- MD5 is cryptographically broken and should not be used for security
- Digital signatures provide authentication and non-repudiation
- Symmetric encryption is faster but requires secure key exchange
- Asymmetric encryption solves key distribution problem
- IVs and salts add essential randomness to encryption
- Brute force attacks demonstrate importance of key strength

---

## Applications to Career Goals

- Security Engineering: Implementing encryption in applications
- Cryptographic Protocol Analysis: Understanding TLS/SSL
- Penetration Testing: Identifying weak cryptographic implementations
- Secure Communications: Building encrypted channels
- Code Signing: Ensuring software authenticity

---

*Completed: October 2025*
