# Digital Envelope & Hybrid Encryption Implementation

Duration: October 2025  
Status: Completed  
Grade: 100/100

---

## Overview

Designed and implemented a complete hybrid encryption scheme combining symmetric and asymmetric cryptography for secure file protection, including digital signatures for authentication and integrity verification.

---

## Core Skills Developed

### Hybrid Encryption (Digital Envelope)
- Combined symmetric and asymmetric encryption advantages
- Generated random session keys for each encryption
- Encrypted data with symmetric key (fast)
- Encrypted session key with public key (secure distribution)
- Implemented efficient encryption for large files

### Bash Scripting for Cryptography
- Created automated encryption/decryption scripts
- Implemented command-line argument parsing
- Handled multiple operation modes (encrypt/decrypt, sign/verify)
- Managed temporary file cleanup
- Used exit codes for status reporting

### Session Key Management
- Generated cryptographically secure random keys
- Used session keys for one-time encryption
- Securely deleted keys after use
- Prevented key reuse across sessions

### AES-192-CTR Implementation
- Applied AES in Counter (CTR) mode
- Used 1 million iterations for key derivation
- Understood stream cipher properties
- Implemented without salt as specified

### RSA Key Operations
- Generated 2048-bit RSA key pairs
- Used public keys for session key encryption
- Used private keys for session key decryption
- Applied RSA with pkeyutl mode

### Digital Signatures
- Signed files using SHA-256 with RSA private keys
- Verified signatures using public keys
- Implemented detached signature files
- Validated file authenticity and integrity

### File Operations & Security
- Handled dynamic file paths and names
- Avoided hardcoded filenames and extensions
- Managed multiple output files (.enc, .key, .sig)
- Cleaned up sensitive temporary files

---

## Cryptographic Scheme Design

### Encryption Process
1. Generate random session key
2. Encrypt file with AES-192-CTR using session key
3. Encrypt session key with recipient's RSA public key
4. Output encrypted file and encrypted key envelope
5. Delete session key from memory

### Decryption Process
1. Decrypt session key using RSA private key
2. Decrypt file using recovered session key
3. Output plaintext file

### Signature Process
1. Hash file with SHA-256
2. Sign hash with RSA private key
3. Output detached signature file

### Verification Process
1. Hash original file
2. Decrypt signature with public key
3. Compare hashes to verify integrity

---

## Key Concepts

### Why Hybrid Encryption
- Symmetric encryption: Fast for large files but key distribution problem
- Asymmetric encryption: Solves key distribution but slow for large data
- Hybrid: Combines both advantages efficiently

### Session Keys
- Unique key per encryption session
- Prevents pattern analysis across multiple files
- Reduces risk if one key is compromised

### Digital Envelope
- Session key encrypted with public key forms the "envelope"
- Only holder of private key can open envelope
- Enables secure key distribution

---

## Tools & Commands

- OpenSSL for all cryptographic operations
- Bash scripting for automation
- AES-192-CTR for symmetric encryption
- RSA-2048 for asymmetric operations
- SHA-256 for hashing
- pkeyutl for key encryption

---

## Key Lessons

- Hybrid encryption is the practical solution for real-world applications
- Session keys provide forward secrecy
- Digital signatures ensure authenticity without encryption
- Proper file cleanup prevents key leakage
- Flexible scripts require dynamic parameter handling
- Exit codes enable programmatic verification

---

## Applications to Career Goals

- Secure Communications: Email encryption systems (like PGP)
- File Protection: Enterprise document encryption
- Security Engineering: Building secure file transfer systems
- PKI Implementation: Real-world public key infrastructure
- DevSecOps: Automated encryption in pipelines

---

*Completed: October 2025*
