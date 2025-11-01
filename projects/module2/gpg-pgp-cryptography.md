# GPG/PGP Cryptography & Secure Communications

Duration: October 2025  
Status: Completed  
Grade: 100/100

---

## Overview

Implemented Pretty Good Privacy (PGP) using GnuPG for secure communications, digital signatures, and public key infrastructure management.

---

## Core Skills Developed

### RSA Key Pair Generation
- Generated 4096-bit RSA key pairs
- Created keys with proper identity information
- Configured key expiration policies
- Understood asymmetric cryptography fundamentals
- Backed up private keys securely

### Public Key Distribution
- Exported public keys in ASCII armor format
- Shared public keys with peers
- Imported public keys from various sources
- Managed local keyring

### Web of Trust & Key Signing
- Verified key fingerprints before signing
- Signed classmates' public keys
- Imported signatures from others
- Built trust relationships through key certification
- Understood decentralized trust model

### Message Encryption
- Encrypted messages using public keys
- Created confidential communications
- Encrypted files for specific recipients
- Verified encryption with correct keys
- Understood that only private key holders can decrypt

### Digital Signatures
- Created detached signatures for files
- Verified digital signatures
- Understood signature authenticity
- Used private keys for signing
- Verified signatures with public keys

### Combined Signing & Encryption
- Created messages that are both signed and encrypted
- Implemented confidential and authenticated communications
- Understood order of cryptographic operations
- Verified sender identity while maintaining confidentiality

### Keyserver Operations
- Uploaded public keys to Ubuntu keyserver
- Downloaded keys from keyservers
- Verified key fingerprints from public databases
- Published key signatures to keyservers
- Used keyserver infrastructure for key distribution

### File Decryption with Third-Party Keys
- Imported temporary key pairs
- Used password-protected private keys
- Decrypted messages intended for specific recipients
- Verified signatures from external parties
- Managed multiple key pairs

---

## Key Concepts Mastered

### Asymmetric Cryptography
- Public key for encryption, private key for decryption
- Private key for signing, public key for verification
- Key pair relationship and mathematical foundations
- RSA algorithm at 4096-bit strength

### Digital Signatures
- Non-repudiation through signature verification
- Signature creation with private keys
- Detached vs. embedded signatures
- Signature authenticity validation

### Web of Trust
- Decentralized trust model
- Key certification through signatures
- Fingerprint verification importance
- Trust propagation through network

### Confidentiality vs. Authentication
- Encryption provides confidentiality
- Signatures provide authentication
- Combined operations provide both
- Use cases for each mechanism

---

## Tools & Commands

- Key Generation: gpg --gen-key, gpg --full-generate-key
- Key Export: gpg --export, gpg --armor --export
- Key Import: gpg --import, gpg --recv-key
- Encryption: gpg --encrypt, gpg -e
- Decryption: gpg --decrypt, gpg -d
- Signing: gpg --sign, gpg --detach-sign
- Verification: gpg --verify
- Keyserver: gpg --keyserver, gpg --send-keys
- Key Management: gpg --list-keys, gpg --fingerprint

---

## Security Best Practices

- Always verify key fingerprints before signing
- Back up private keys in secure locations
- Use strong passphrases for private key protection
- Verify signatures before trusting encrypted content
- Keep private keys secure and never share them
- Use appropriate key sizes (4096-bit RSA minimum)
- Regularly update keys and manage expiration
- Upload signed keys to keyservers for distribution

---

## Applications to Career Goals

- Secure Communications: Encrypted email and file transfer
- Identity Verification: Digital signature validation
- PKI Management: Enterprise key infrastructure
- Security Engineering: Implementing cryptographic solutions
- Code Signing: Software authenticity verification

---

*Completed: October 2025*
