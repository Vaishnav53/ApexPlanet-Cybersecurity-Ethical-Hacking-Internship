# Cryptography Basics

## Introduction

Cryptography is the science of protecting information by transforming it into a secure format. It ensures confidentiality, integrity, authentication, and non-repudiation of data.

---

# Objectives of Cryptography

## Confidentiality

Ensures that only authorized users can access information.

### Example

Encrypted messages.

---

## Integrity

Ensures that data is not modified during transmission.

### Example

Hashing algorithms.

---

## Authentication

Verifies the identity of users or systems.

### Example

Digital Certificates.

---

## Non-Repudiation

Prevents users from denying their actions.

### Example

Digital Signatures.

---

# 1. Symmetric Encryption

Symmetric encryption uses the same key for encryption and decryption.

```text
Plaintext
    ↓
Encryption Key
    ↓
Ciphertext
    ↓
Same Key
    ↓
Plaintext
```

### Advantages

* Fast
* Efficient
* Suitable for large data

### Disadvantages

* Key distribution problem

---

## Common Symmetric Algorithms

### AES

Advanced Encryption Standard.

* Most widely used
* Supports 128, 192, 256-bit keys

### DES

Data Encryption Standard.

* Older algorithm
* Considered insecure today

### 3DES

Triple DES.

* Improved version of DES
* Slower than AES

---

# 2. Asymmetric Encryption

Uses two keys:

```text
Public Key
Private Key
```

### Process

```text
Public Key → Encrypt
Private Key → Decrypt
```

### Advantages

* Secure key exchange
* Digital signatures

### Disadvantages

* Slower than symmetric encryption

---

## Common Asymmetric Algorithms

### RSA

Most widely used public-key algorithm.

### ECC

Elliptic Curve Cryptography.

Provides strong security using smaller keys.

---

# 3. Hashing

Hashing converts data into a fixed-length value.

### Properties

* One-way function
* Fixed output length
* Cannot be reversed

---

## MD5

Output:

```text
128-bit
```

Weak and vulnerable to collisions.

---

## SHA-1

Output:

```text
160-bit
```

Deprecated due to vulnerabilities.

---

## SHA-256

Output:

```text
256-bit
```

Widely used and secure.

---

# 4. Public Key Infrastructure (PKI)

PKI is a framework that manages digital certificates and encryption keys.

### Components

* Certificate Authority (CA)
* Registration Authority (RA)
* Digital Certificates
* Public Keys
* Private Keys

---

# 5. Digital Certificates

Digital certificates verify the identity of systems and websites.

### Information Contained

* Subject Name
* Public Key
* Issuer
* Expiration Date
* Digital Signature

---

# 6. SSL/TLS

SSL/TLS secures communication between clients and servers.

### Example

```text
https://example.com
```

---

## TLS Handshake Process

### Step 1

Client connects to server.

### Step 2

Server sends certificate.

### Step 3

Certificate validation.

### Step 4

Session key generation.

### Step 5

Secure encrypted communication begins.

---

# OpenSSL

OpenSSL is a command-line tool used to implement cryptographic functions.

### Generate SHA256 Hash

```bash
sha256sum file.txt
```

### Encrypt File

```bash
openssl enc -aes-256-cbc -in secret.txt -out encrypted.enc
```

### Decrypt File

```bash
openssl enc -aes-256-cbc -d -in encrypted.enc -out decrypted.txt
```

---

# Real-World Applications

* HTTPS Websites
* VPN Connections
* Secure Email
* Digital Signatures
* Blockchain Technologies
* Password Storage

---

# Cybersecurity Relevance

Cryptography protects sensitive information, secures communication channels, validates identities, and ensures trust in digital systems.

---

# Conclusion

Cryptography is a core pillar of cybersecurity. Understanding encryption, hashing, certificates, PKI, and TLS is essential for protecting modern information systems.
