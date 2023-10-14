# Cryptography

* Types of Attacks
  * Cryptoanalysis
  * Brute Force Attack
* Types of Cryptography
  * Symmetric
  * Asymmetric
* Block vs Stream Cipher
* DES
  * Symmetric
  * Block Cipher (64 bits each)
  * Insecure due to the relatively short 56-bit key size
  * Triple DES
* AES
  * Symmetric
  * Also known as Rijndael
  * Block Cipher (128 bits each)
* RSA
  * Asymmetric
  * Rivest–Shamir–Adleman
  * Encryption key is public and distinct from the decryption key, which is kept secret (private)
* Diffie-Hellman key exchange
* Digital signature
* Digital certificate
* SSL and SSL certificate
* SSL/TLS handshake protocol



# Questions

Certainly! Here are some interview questions based on those bullet points:

### Cryptography

1. Can you explain what cryptography is and why it is important in modern computing?

### Types of Attacks

1. What are the common types of attacks that cryptography aims to prevent?
2. How does a Man-in-the-Middle attack work?

### Cryptoanalysis

1. What is cryptoanalysis and how is it different from cryptography?

### Brute Force Attack

1. Explain what a Brute Force Attack is and how you can defend against it.

### Types of Cryptography

1. What are the main types of cryptography? Can you explain the difference between symmetric and asymmetric cryptography?

### Symmetric

1. What are the advantages and disadvantages of symmetric cryptography?

### Asymmetric

1. How does asymmetric cryptography work? What are its pros and cons?

### Block vs Stream Cipher

1. Can you explain the difference between a block cipher and a stream cipher?

### DES (Data Encryption Standard)

1. What is DES and why is it considered insecure today?

### Symmetric

1. Is DES a symmetric or asymmetric algorithm?

### Block Cipher

1. What is the block size used in DES?

### Triple DES

1. How does Triple DES improve upon DES?

### AES (Advanced Encryption Standard)

1. What is AES and how does it differ from DES?

### Symmetric

1. Confirm if AES is a symmetric or asymmetric algorithm?

### Block Cipher

1. What is the block size used in AES?

### RSA

1. What is RSA and how is it used in secure communications?

### Asymmetric

1. Is RSA a symmetric or asymmetric algorithm?

### Encryption Key

1. In RSA, is the encryption key public or private?

### Diffie-Hellman Key Exchange

1. Can you explain how the Diffie-Hellman key exchange works?

### Digital Signature

1. What is a digital signature and how is it used for authentication?

### Digital Certificate

1. What is a digital certificate and how is it different from a digital signature?

### SSL and SSL Certificate

1. What is SSL and how do SSL certificates contribute to web security?

### SSL/TLS Handshake Protocol

1. Can you explain the steps involved in an SSL/TLS handshake?

Feel free to use these questions to prepare for your interview or adapt them as needed. Good luck!


# Answer

Of course! Here are the answers to the interview questions:

### Cryptography

1. **Cryptography** is the practice of securing communication and data against unauthorized access. It's crucial in modern computing for protecting information in various applications including online banking, e-commerce, and secure communications.

### Types of Attacks

1. Cryptography aims to prevent a variety of attacks, including Man-in-the-Middle attacks, Replay attacks, and Brute Force attacks.
2. A **Man-in-the-Middle attack** occurs when an unauthorized party intercepts and possibly alters the communication between two parties.

### Cryptoanalysis

1. **Cryptoanalysis** is the study of analyzing cryptographic systems to find vulnerabilities. It is different from cryptography, which is the creation of cryptographic algorithms.

### Brute Force Attack

1. A **Brute Force Attack** involves trying every possible key until the correct one is found. Defenses include using longer keys, rate limiting, and lockout policies.

### Types of Cryptography

1. The main types of cryptography are **Symmetric** and **Asymmetric**. Symmetric uses the same key for encryption and decryption, while asymmetric uses different keys.

### Symmetric

1. **Symmetric cryptography** is faster but less secure if the key is compromised.

### Asymmetric

1. **Asymmetric cryptography** uses a pair of keys: a public key for encryption and a private key for decryption. It's more secure but slower.

### Block vs Stream Cipher

1. **Block Ciphers** encrypt data in fixed-size blocks, while **Stream Ciphers** encrypt data bit-by-bit or byte-by-byte.

### DES (Data Encryption Standard)

1. **DES** is an older symmetric key algorithm. It's considered insecure due to its short key length of 56 bits.

### Symmetric

1. DES is a **symmetric algorithm**.

### Block Cipher

1. DES uses a **block size of 64 bits**.

### Triple DES

1. **Triple DES** applies the DES algorithm three times to each data block, which makes it more secure than DES but slower.

### AES (Advanced Encryption Standard)

1. **AES**, also known as Rijndael, is a symmetric algorithm that's considered secure and is widely used. It's different from DES in terms of key length, block size, and security.

### Symmetric

1. AES is a **symmetric algorithm**.

### Block Cipher

1. AES has a **block size of 128 bits**.

### RSA

1. **RSA** is an asymmetric algorithm used for encryption and digital signatures. It's named after its inventors: Rivest, Shamir, and Adleman.

### Asymmetric

1. RSA is an **asymmetric algorithm**.

### Encryption Key

1. In RSA, the **encryption key is public**, and distinct from the decryption key, which is private.

### Diffie-Hellman Key Exchange

1. The **Diffie-Hellman key exchange** is a method for securely exchanging cryptographic keys over a public channel.

### Digital Signature

1. A **digital signature** is a cryptographic technique to authenticate the sender of a message or the signer of a document.

### Digital Certificate

1. A **digital certificate** is an electronic document that binds a public key to an entity and verifies that the public key actually belongs to them.

### SSL and SSL Certificate

1. **SSL (Secure Sockets Layer)** is a protocol for web security. An **SSL Certificate** is a digital certificate that provides authentication for a website and enables SSL/TLS encryption.

### SSL/TLS Handshake Protocol

1. The **SSL/TLS handshake protocol** is a series of steps to initiate an SSL or TLS session. It involves certificate exchange, selection of encryption algorithms, and creation of a shared secret for session encryption.

I hope these answers provide a comprehensive understanding of each topic. If you have further questions or need more details, feel free to ask!
