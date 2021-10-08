# Encryption [1,3]
## Basics [1]
## Ciphers [1,3]
    * Classical
        - Caesar Cipher
        - Vigenere Cipher
        - Shift Ciphers (Caesar)
    * How they work
        - The Permutation
        - The mode of operation
        - Why are classical ciphers not secure?
    * Ciphers vs Encryption
    * When do Ciphers Do more than encryption?
        - Authenticated Encryption
        - Format-Preserving Encryption
        - Fully Homomorphic Encryption
        - Searchable Encryption
        - Tweakable Encryption
## Perfect Encryption [1]
    * The One Time Pad (OTP)
        - Using OTP
        - Why is OTP secure?
## Encryption Security [1]
    * Attack Models
    * Security Goals
    * Security Notions
## Symmetric [1,3]
    * Basics
    * Simple Symmetric Encryption: The Substitution Cipher
## Asymmetric [1]
## Authenticated Encryption [1]
    * Using MACs
        - Encrypt & MAC
        - MAC then Encrypt
        - Encrypt then MAC
    * Authenticated Ciphers
        - Authenticated Encryption w/ associated Data
        - Avoiding Predictability w/ Nonces
        - What makes a good cipher?
        - AES-GCM: The Authenticated Cipher Standard
            * GCM Internals: CTF & GHASH
            * GCM Security
            * GCM Efficiency
        - OCB: An authenticated Cipher Faster than GCM
            * OCB Internals
            * OCB Security
            * OCB Efficiency
        - SIV: The Safest Authenticated Cipher
        - Permutation-Based AEAD
        - What can go wrong
            * AES-GCM & Weak Hash Keys
            * AES-GCM & Small Tags
## Strong Encryption [7]
    * AES
    * ECB & CBC modes
    * Padding Oracle Attack
    * RSA
        - Public-Key Encryption
        - Algorithm
        - Python Implementation
        - Cracking RSA w/ Similar Factors
    * Cryptography w/i IoT
    * ZigBee 
        - Cryptographic Keys
        - Complexity of ZigBee Key Management
    * BlueTooth LE
## What can go wrong [1]
    * Weak Cipher
    * Wrong Model

# Obfuscation [7]
    * Caesar Cipher / ROT13
    * Base64
        - Binary Data
        - ASCII Data
    * XOR

# Randomness [1,2]
## Random vs Non-Random [1]
## Randomness as Probability Distribution [1]
## Generating Randomness [2]
    * Real Random
    * Attack Models for a PRNG
    * Fortuna
    * The Generator
    * Accumulator
    * Seed File Management
    * Choosing Random Elements
## Entropy: A Measure of Uncertainty [1]
## Random Number Generators (RNG) & Psuedorandom Number Generator (PRNG) [1]
    * How PRNGs work
    * Security Concerns
    * The PRNG Fortuna
    * Cryptographic vs Non-Cryptographic PRNGs
    * The Uselessness of Statistical Tests
## Real World PRNGs [1]
    * Generating Random Bits in Unix-Based Systems
    * The CryptGenRandom() Function in Windows
    * A Hardware-Based PRNG: RDRAND in Intel Microprocessors
## What can go wrong [1]
    * Poor Entroy Sources
    * Insufficient Entropy @ boot time
    * Non-Cryptographic PRNG
    * Sampling Bug w/ Strong Randomness

# Primes [2]
    * Divisibility and Primes
    * Generating Small Primes
    * Computations Modulo a Prime
    * Large Primes

# Cryptographic Security [1,2,3,4]
## Define it [1]
    * Theoretical Security: Informational Security
    * Practical Security: Computational Security
## Quantifying Security [1]
    * Measure Security in Bits
    * Full Attack Cost
    * Choosing and Evaluating Security Levels
## Achieving Security [1]
    * Provable Security
    * Heuristic Security
## Generating keys [1]
    * Symmetric Keys
    * Asymmetric Keys
    * Protecting Keys
## Key Establishment [3]
    * Introduction
        - Terminology
        - Key Freshness & Key Distribution
        - The n2 Key Distribution Problem
    * Key Establishment using Symmetric-Key Techniques
        - Key Establishment with a Key Distribution Center
        - Kerberos
        - Remaining Problems w/ Symmetric-Key Distribution
    * Key Establishment using Asymmetric Techniques
        - Man-in-the-middle attack
        - Certificates
        - Public-Key Infrastructure (PKI) & CAs
## Key Negotiation [2]
    * The setting
    * A first try
    * Protocols Live forever
    * An authentication convention
    * A Second Attempt
    * A Third Attempt
    * The Final Protocol
    * Different views of the protocol
    * Computational complexity of the protocol
    * Protocol complexity
    * A gentle warning
    * Key negotiation from a password
## Key Management [2,4]
    * The Clock 
        - Uses for a clock
        - Using the real-time clock chip
        - Security dangers
        - Creating a reliable clock
        - The same-state problem
        - Time
        - Closing Recommendations
    * Key Servers
        - Basics
        - Kerberos
        - Simpler Solutions
        - What to Choose
    * The Dream of PKI
        - A very short PKI Overview
        - PKI Examples
        - Additional Details
        - Summary
    * PKI Reality
        - Names
        - Authority
        - Trust
        - Indirect Authorization
        - Direct Authorization
        - Credential Systems
        - The Modified Dream
        - Revocation
        - So what is a PKI Good for?
        - What to choose
    * PKI Practicalities
        - Certificate Format
        - The Life of a key
        - Why keys wear out
        - Going further
    * Storing Secrets
        - Disk
        - Human Memory
        - Portable Storage
        - Secure Token
        - Secure UI
        - Biometrics
        - Single Sign-On (SSO)
        - Risk of Loss
        - Secret Sharing [2,4]
        - Wiping Secrets
## Standards & Patents
    * Standards
    * Patents
## Implementation Issues [2]
    * Creating Correct Programs
    * Creating Secure Software
    * Keeping Secrets
    * Quality of Code
    * Side-Channel Attacks
    * Large integer arithmetic
    * Faster Multiplication 
    * Side-channel attacks
    * Protocols
## What can go wrong [1]
    * Incorrect Security Proof
    * Short Keys for Legacy Support

# Cryptographic Techniques [4]
## Key Length [4]
    * Symmetric Key Length
    * Asymmetric Key Length
    * Comparing Symmetric & Public-Key Key Length
    * Birthday Attacks Against One-Way Hash Functions
    * How Long should the Key Be?
    * Caveat Emptor
## Key Management [4]
    * Generating Keys
    * Nonlinear Keyspaces
    * Transferring Keys
    * Verifying Keys
    * Using Keys
    * Updating Keys
    * Storing Keys
    * Backup Keys
    * Compromised Keys
    * Lifetime of Keys
    * Destroying Keys
    * Public-Key Key Management
## Algorithm Types & Modes [4]
    * Electronic Codebook Mode
    * Block Replay
    * Cipher Block Chaining Mode
    * Stream Ciphers
    * Self-Synchronizing Stream Ciphers
    * Cipher Feedback Mode
    * Sychronous Stream Ciphers
    * Output-Feedback Mode
    * Counter Mode
    * Other Block-Cipher Modes
    * Choosing a cipher mode
    * Interleaving
    * Block Ciphers versus stream ciphers
## Using Algorithms [4]
    * Choosing an Algorithm
    * Public-Key Cryptography versus Symmetric Cryptography
    * Encrypting Communications
    * Encrypting Data For Storage
    * Hardware Encryption Versus Software Encryption
    * Compression, Encoding, & Encryption
    * Detecting Encryption
    * Hiding Ciphertext in Ciphertext
    * Destroying Information

# Mathematical Background [4]
    * Information Theory
    * Complexity Theory
    * Number Theory
    * Factoring
    * Prime Number Generation
    * Discrete Logarithms in a Finite Field

# Ciphers [1,2,3,4,5]
## Miscellaneous [5]
    * Highlights of Fractional Substitution
    * Investigating the Unknown Cipher
    * Geometrical Types
        - The Nihilist Transportation
        - The Turning Grille
    * Transportation Types
    * Concealment Types
    * Irregular Types
        - Columnar Transposition
    * General Methods
        - Multiple Anagramming
    * Substitution Types
    * The Consonant-Line Short Cut
## Historical Ciphers [3,5]
    * Shift Ciphers (Caesar)
    * Affine Cipher
    * Vigenere Cipher
        - Key Progression
        - Miscellaneous Phases of Vigenere Decryptment
        - Multiple Alphabet Ciphers
    * Playfair Cipher
        - Polygram Substitution
## Block Ciphers [1,2,3,4]
    * Introduction
        - What is it?
        - Security Goals
        - Block Size
        - The Codebook Attack
        - Types of Attack [2]
        - The Ideal Block Cipher [2]
        - Real Block Ciphers [2]
        - Definition of Block Cipher Security [2]
    * How to Construct a Block Cipher
        - A Block Ciphers Rounds
        - The Slide Attack and Round Keys
        - Substitution-Permutation Networks
        - Feistel Schemes
    * The Advanced Encryption Standard (AES) [3]
        - AES Internals
        - AES in Action
        - AES History
        - Implementing AES
            * Table Based Implementations
            * Native Instructions
        - Is AES Secure?
    * Modes of Operation [1,2,3]
        - The Electronic Codebook (ECB) Mode
        - The Cipher Block Chaining (CBC) Mode
        - How to Encrypt any message in CBC Mode
        - The Counter (CTR) Mode
        - Output Feedback (OFB) Mode [2]
        - Combined Encryption & Authentication [2]
        - Padding [2]
        - Which should I use? [2]
        - Info Leakage [2]
        - Galois Counter Mode (GCM) [3]
        - Cipher Feedback (CFB) Mode [3]
    * Exhaustive Key Search Revisted [3]
    * Increasing the Security of Block Ciphers [3]
        - Double Encryption and Meet in the middle Attacks
        - Triple Encryption
        - Key Whitening
    * Different Block Ciphers [4]
        - Lucifer
        - Madryga
        - NewDES
        - FEAL
        - REDOC
        - LOKI
        - Khufu & Khafre
        - RC2
        - IDEA
        - MMB
        - CA-1.1
        - Skipjack
        - GOST
        - CAST
        - Blowfish
        - SAFER
        - 3-Way
        - Crab
        - SXAL8/MBAL
        - RC5
        - Other Block Algorithms
        - Theory of Block Cipher Design
        - Choosing a Block Algorithm
    * Combining Block Ciphers
        - Double Encryption
        - Triple Encryption
        - Doubling the Block Length
        - Other Multiple Encryption Schemes
        - CMDF Key Shortening
        - Whitening
        - Cascading Multiple Block Algorithms
        - Combining Multiple Block Algorithms
    * What Can go Wrong? [1]
        - Meeting in the Middle Attacks
        - Padding Oracle Attacks
## Stream Ciphers [1,3,4]
    * Introduction
        - Stream Ciphers vs Block Ciphers [3]
        - Encryptions & Decryption [3]
        - How stream ciphers work
            * Stateful and counter-based stream ciphers
        - Choosing a Stream Cipher
    * Hardware-oriented stream ciphers
        - Feedback shift registers
        - Grain-128a
        - A5/1
    * Software-oriented stream ciphers
        - RC4
        - Salsa20
    * Random Numbers & an Unbreakable Stream Cipher
        - RNGs (see ____)
        - The One Time Pad (see ____)
        - Towards Practical Stream Ciphers
    * Shift Register-Based Stream Cipher
        - Linear Feedback Shift Registers (LFSR)
        - Known-Plaintext Attack Against Single LFSRs
        - Trivium
    * Stream Cipher Design
        - Design & Analysis of Stream Ciphers
        - System-Theoretic Approach to Stream Cipher Design
        - Complexity-Thematic Approach to Stream Cipher Design
        - Other Approaches to Stream-Cipher Design
        - Cascading Multiple Stream Ciphers
        - Generating Multiple Streams from a single Psuedo-Random-Sequence Generator
        - Real Random-Sequence Generator
    * Other Ciphers
        - Linear Congruential Generators
        - A5
        - Hughes XPD/KPD
        - Nanoteq
        - Rambutan
        - Gifford
        - Algorithm M
        - PKZIP
        - RC4
        - SEAL
        - WAKE
        - Feedback w/ Carry Shift Registers
        - Stream Ciphers using FCSRs
        - Nonlinear-Feedback Shift Registers
    * What can go wrong?
        - Nonce Reuse
        - Broken RC4 Implementation
        - Weak Ciphers baked into hardware
## Authenticated Ciphers [1]
    * Authenticated Encryption w/ associated Data
    * Avoiding Predictability w/ Nonces
    * What makes a good cipher?
    * AES-GCM: The Authenticated Cipher Standard
        - GCM Internals: CTF & GHASH
        - GCM Security
        - GCM Efficiency
        - What can go wrong
            * AES-GCM & Weak Hash Keys
            * AES-GCM & Small Tags
    * OCB: An authenticated Cipher Faster than GCM
        - OCB Internals
        - OCB Security
        - OCB Efficiency
    * SIV: The Safest Authenticated Cipher
    * Permutation-Based AEAD
## Other Ciphers [5]
    * Polyalphabetical Encipherment Applied by Groups
    * Periodic Ciphers w/ Mixed Alphabets
    * Some Periodic Number-Ciphers
    * Auto-Encipherment
    * The Kasiski Method for Periodic Ciphers
    * The Gronsfeld, Porta, & Beaufort Ciphers
    * Simple Substitution with Complexities

# Hash Functions [1,2,3,4]
## Introduction [2,3]
    * Security of Hash Functions
        - Requirements [3]
            * Preimage Resistance or One-Wayness
            * Second Preimage Resistance or Weak Collision Resistance
            * Collision Resistance and the Birthday Attack
    * Real Hash Functions
    * Overview of Hash Algorithms
        - Dedicated Hash Functions: MD4 Family
        - Hash Functions from Block Ciphers
    * Weaknesses of Hash Functions
    * Fixing the Weaknesses
    * Which should I choose?
    * Motivation: Signing Long Messages [3]
## One-Way Hash Functions [4]
    * Background
    * Snefru
    * N-Hash
    * MD4
    * MD5
    * MD2
    * Secure Hashing Algorithm (SHA)
    * RIPE-MD
    * HAVAL
    * One-Way Hash Functions Using Symmetric Block Algorithms
    * Using Public-Key Algorithms
    * Choosing a One-Way Hash Function
    * Message Authentication Codes (MAC)
## Secure Hash Functions [1]
    * Unpredictability Again
    * Preimage Resistance
    * Collision Resistance
    * Finding Collisions
## Building Hash Functions [1]
    * Compression-Based Hash Functions: The Merkle-Damgard Construction
    * Permutation-Based Hash Functions: Sponge Functions
## Comparing Hash Functions [1]
## Hash Families [1,3]
    * SHA
        - SHA1 [1,3]
            * Preprocessing
            * Hash Computation
            * Implementation
        - SHA2
        - SHA3
            * The competetion
            * Keccak
        - SHA128
        - SHA256
        - SHA512
    * MD5
    * MD4 [3]
    * Blake2
## Keyed Hashing [1,2,3]
    * Message Authentication Codes (MACs)
        - MACs in Secure Communication
        - Forgery and Chosen-Message Attacks
        - Replay Attacks
        - What does a MAC do? [2]
        - The Ideal MAC & MAC Security [2]
        - CBC-MAC & CMAC [2,3]
        - HMAC [2,3]
        - GMAC [2,3]
        - Which MAC to Choose [2]
        - Using a MAC
        - Principles [3]
    * Psuedorandom Functions (PRFs)
        - PRF Security
        - Why PRFs are stronger than MACs
    * Creating Keyed Hashes from Unkeyed Hashes
        - The Secret-Prefix Construction
        - The Secret-Suffix Construction
        - The HMAC Construction
        - A Generic Attack Against Hash-Based MACs
    * Creating Keyed Hashes from Block Ciphers: CMAC
        - Breaking CBC-MAC
        - Fixing CBC-MAC
    * Dedicated MAC Designs
        - Poly1305
        - SIPHash
## What can go wrong? [1]
        * The Length-Extension Attack
        * Fooling Proof-of-Storage Protocols
        * Timing Attacks on MAC verification
        * When Sponges Leak

# Digital Signatures [3,4]
## Introduction [3]
## The RSA Signature Scheme [3]
    * Schoolbook RSA Digital Signature
    * Computational Aspects
    * Security
## The Elgamal Signature Scheme [3]
    * Schoolbook Elgamal Digital Signature
    * Computational Aspects
    * Security
## The Digital Signature Algorithm (DSA) [3]
    * The DSA Algorithm
    * Computational Aspects
    * Security
## The EC Signature Scheme (ECDSA) [3]
    * The ECDSA Algorithm
    * Computational Aspects
    * Security
## Public Key Digital Signature Algorithms[4]
    * DSA
    * DSA variants
    * GOST DSA
    * Discrete Logarithm Signature Schemes
    * Ong-Schnorr-Shamir
    * ESIGN
    * Cellular Automata
    * Other Public-Key Algorithms

# Secure Channels [2]
## Introduction
    * Properties of a Secure Channel
    * Order of Authentication and Encryption
## Designing a Secure Channel
    * Overview
    * Details
## Alternatives

# Public Key Cryptography [3,4]
## Introduction [3]
    * Symmetric vs Asymmetric
## Public Key Algorithms[4]
    * Background
    * Knapsack Algorithms
    * RSA
    * Pohlig-Hellman
    * Rabin
    * ElGamal
    * McEliece
    * Elliptic Curve Cryptosystems
    * LUC
    * Finite Automation Public-Key Cryptosystems
## Public Key Digital Signature Algorithms[4]
    * DSA
    * DSA variants
    * GOST DSA
    * Discrete Logarithm Signature Schemes
    * Ong-Schnorr-Shamir
    * ESIGN
    * Cellular Automata
    * Other Public-Key Algorithms
## Practical Aspects [3]
    * Security Mechanisms
    * The Remaining Problem: Authenticity of Public Keys
    * Important Public-Key Algorithms
    * Key Lengths and Security Levels
## Essential Number Theory & Public-Key Algorithms [3]
    * Euclidean Algorthim
    * Extended Euclidean Algorthim
    * Euler's Phi Function
    * Fermat's Little Theorem and Euler's Theorem
## Diffie Helman Key Exchange [3]
    * Overview
    * Security of DH KE
## Some Math [3]
    * Groups
    * Cyclic Groups
    * Subgroups
## Discrete Logarithm Problem [3]
    * The Discrete Logarithm Problem in Prime Fields
    * The Generalized Discrete Logarithm Problem
    * Attacks Against the Discrete Logarithm Problem
## The Elgamal Encryption Scheme [3]
    * From Diffie-Hellman Key Exchange to Elgamal Encryption
    * The Elgamal Protocol
    * Computational Aspects
    * Security

# RSA [1,2]
## The Math [1,2]
    * Multiplication modulo n [2]
## Theory [2,3]
    * Introduction
    * RSA Defined
    * Pitfalls using RSA
## Trapdoor Permutation [1]
## Key Generation & Security [1,3]
    * Proof of Correctness [3]
## Encrypting w/ RSA [1,2,3]
    * Breaking RSA Encryption Malleability
    * Strong RSA Encryption: OAEP
## Signing w/ RSA [1,2]
    * Breaking RSA Signatures
    * The PSS Signature Standard
    * Full Domain Hash Signatures
## Implementations [1,2,3]
    * Fast Exponentiation Algorithm: Square & Multiply
    * Small Exponents for Faster Public-Key Ops
    * The Chinese Remainder Theorem [1,2]
    * RSA In practice : Padding [3]
    * Software
    * Hardware
## Speed-Up Techniques [3]
    * Fast Encryption with Short Public Exponents
    * Fast Decryption with Chinese Remainder Theorem
## Finding Large Primes [3]
    * How Common are Primes
    * Primality Tests
## What can go wrong? [1,3]
    * Bellcore Attack on RSA-CRT
    * Side Channel Attacks
    * Sharing Private Exponents or Moduli
    * Attacks [3]

# DES [3,4]
## Introduction [3,4]
    * Confusion & Diffusion
    * Overview of the DES Algorithm
    * Background
    * Variants
    * How secure is DES today?
## Differential & Linear Cryptanalysis [4]
## Internal Structure of DES [3]
    * Initial & Final Permutation
    * The f-Function
    * Key Schedule
## Decryption [3]
## Security of DES [3,4]
    * Exhaustive Key Search
    * Analytical Attacks
## Implementation of DES [3,4]
    * Design
        - Criteria [4]
    * Software
    * Hardware
## Alternatives to DES [3]
    * AES
    * Triple DES (3DES)
    * DESX
    * Lightweight Cipher PRESENT

# AES [3]
## Introduction [3]
    * Overview of AES Algorithm
    * Brief history of AES
## Some Math [3]
    * Existence of Finite Fields
    * Prime Fields
    * Extension Fields GF(2m)
    * Addition and subtraction in GF(2m)
    * Multiplication in GF(2m)
    * Inversion in GF(2m)
## Internal Structure [3]
    * Byte Substitution Layer
    * Diffusion Layer
    * Key Addition Layer
    * Key Schedule
## Decryption [3]
## Implementation [3]
    * Software
    * Hardware

# Diffie-Hellman [1,2]
## The Function [1]
## The Problems [1]
    * The Computational Diffie-Hellman Problem
    * The Decisional Diffie-Hellman Problem
    * More Diffie-Hellman Problem
## Protocols [1]
    * Key-Agreement
        - Example of Non-DH Key Agreement
        - Attack Models for Key Agreement Protocols
        - Performance
    * Diffie-Hellman
        - Anonymous Diffie-Hellman
        - Authenticated Diffie-Hellman
        - Menezes-Qu-Vanstone (MQV)
## Theory [2]
    * Groups
    * Basic DH
    * Man in the Middle
    * Pitfalls
    * Safe Primes
    * Using a Smaller Subgroup
    * The Size of P
    * Practical Rules
## What can go wrong? [1]
    * Not hashing the shared secret
    * Legacy Diffie-Hellman in TLS
    * Unsafe Group Parameters

# Elliptic Curves [1,3]
## Introduction [1]
    * What are they?
    * Elliptic Curves over integers
    * Adding & Multiplying Points
    * Elliptic Curve Groups
## How to compute w/ Elliptic Curves [3]
    * Definition of Elliptic Curves
    * Group Operations on Elliptic Curves
## The Elliptic Curve Discrete Logarithm (ECDLP) Problem [1,3]
## Diffie-Hellman Key Agreement over Elliptic Curves [1,3]
    * Signing with Elliptic Curves
    * Encrypting with Elliptic Curves
    * DHKE w/ Elliptic Curves
## Security [3]
## Implementation [3]
    * Software
    * Hardware
## Choosing a Curve [1]
    * NIST Curves
    * Curve25519
    * Other Curves
## What can go wrong? [1]

# TLS [1]
## Target Applications & Requirements [1]
## The TLS Protocol Suite [1]
    * The TLS & SSL protocol Family: a brief history
    * TLS in a nutshell
    * Certificates & certificate authorities
    * The record protocol
    * The TLS handshake protocol
    * TLS 1.3 cryptographic algorithms
## TLS 1.3 vs 1.2 [1]
    * Downgrade protection
    * Single Round-trip handshake
    * Session resumption
## Strengths of TLS [1]
    * authentication
    * forward secrecy
## What can go wrong? [1]
    * compromised certificate authority
    * compromised server
    * compromised client
    * Bugs in implementation

# Quantum & Post Quantum [1]
## How Quantum Computers work [1]
    * Quantum Bits
    * Quantum Gates
## Quantum Speed-up [1]
    * Exponential Speed-Up and Simon's Problem
    * The Threat of Shor's Algorithm
    * Shor's Algorithm solves the factoring problem
    * Shor's Algorithm and the discrete logarithm problem
    * Grover Algorithm
## Why are Quantum Computers so hard to build? [1]
## Post-Quantum Cryptographic Algorithms [1]
    * Code-Based Cryptography
    * Lattice-Based Cryptography
    * Multivariate Cryptography
    * Hash-Based Cryptography
## What can go wrong? [1]
    * Unclear security level
    * Fast Forward: What happens if its Too late?
    * Implementation Issues

# Hard Problems [1]
## Computational Hardness [1]
    * Measuring Running Time
    * Polynomial vs Superpolynomial Time
## Complexity Classes [1]
    * Nondeterministic Polynomial Time
    * NP-Complete Problems
    * The P vs NP Problems
## The Factoring Problem [1]
    * Factoring Large Numbers in Practice
    * Is factoring NP-Complete
## The Discrete Logarithm Problem [1]
    * What is a Group?
    * The Hard Thing
## What can go wrong? [1]
    * When Factoring is Easy
    * Small Hard Problems aren't Hard

# Cryptography [2,3,4]
## The Context of Crypto [2]
    * The Role of Crypto
    * The weakest link property
    * The adversarial setting
    * Professional paranoia
    * Threat Model
    * Cryptography is not the solution
    * Cryptography is very difficult
    * Cryptography is the easy part
    * Generic Attacks
    * Security & other design criteria
## Intro to Crypto [2,3]
    * Encryption
    * Authentication
    * Public-Key Encryption
    * Digital Signatures
    * PKI
    * Attacks
    * Under the Hood
    * Security Level
    * Performance
    * Complexity
    * Overview of Cryptology [3]
    * Cryptanalysis [3]
        - General Thoughts on Cryptosystems
        - How many key bits are enough?
    * Modular Arithmetic [3]
        - Modular Arithmetic
        - Integer Rings
## Protocols [2,4]
    * Roles
    * Trust
    * Incentive
    * Trust in Cryptographic Protocols
    * Messages & Steps
    * Protocol Building Blocks [4]
        - Intro to Protocols
        - Communications using symmetric cryptography
        - one-way functions
        - one-way hash functions
        - Communications using public-key cryptography
        - digital signatures
        - digital signatures with encryption
        - random & pseudo-random sequence generation
    * Basic Protocols [4]
        - key exchange
        - authentication
        - authentication & key exchange
        - formal analysis of authentication & key exchange protocols
        - multiple-key public-key cryptography
        - secret splitting
        - secret sharing
        - cryptographic protection of databases
    * Intermediate Protocols [4]
        - timestamping services
        - subliminal channel
        - undeniable digital signatures
        - designated confirmer signatures
        - proxy signatures
        - group signatures
        - fail-stop digital signatures
        - computing w/ encrypted data
        - bit commitment
        - fair coin flips
        - mental poker
        - one-way accumulators
        - all-or-nothing disclosure of secrets
        - key escrow
    * Advanced Protocols [4]
        - zero-knowledge proofs
        - zero-knowledge proofs of identity
        - blind signatures
        - identity-based public-key cryptography
        - oblivious transfer
        - oblivious signatures
        - simultaneous contract signing
        - digital certified mail
        - simultaneous exchange of secrets
    * Esoteric Protocols [4]
        - secure elections
        - secure mulitparty computation
        - anonymous message broadcast
        - digital cash

# Identification Schemes [4]
    * Feige-Fiat-Shamir
    * Guillou-Quisquater
    * Schnorr
    * Converting Identification Schemes to signature schemes

# Key Exchange Algorithms [4]
    * Diffie-hellman
    * Station-to-station protocol
    * Shamirs three-pass protocol
    * COMSET
    * Encrypted Key Exchange
    * Fortified Key Negotiation
    * Conference Key Distrobution and Secret Broadcasting

# Special Algorithms for Protocols [4]
    * Multiple-key Public-Key Cryptography
    * Secret-Sharing Algorithms
    * Subliminal Channel
    * Undeniable Digital Signatures
    * Designated Confirmer Signatures
    * Computing with Encrypted Data
    * Fair Coin Flips
    * One-Way Accumulators
    * All-or-nothing Disclosure of secrets
    * Fair and failsafe cryptosystems
    * Zero-Knowledge Proofs of knowledge
    * Blind Signatures
    * Oblivious Transfer
    * Secure Multiparty computation
    * Probabilistic Encryption
    * Quantum Cryptography

# Example Implementations [4]
    * IBM Secret Key Management Protocol
    * MITRENET
    * ISDN
    * STU-III
    * Kerberos
    * KryptoKnight
    * SESAME
    * IBM Common Cryptographic Architecture
    * ISO Authentication Framework
    * Privacy-Enhanced Mail (PEM)
    * Message Security Protocol (MSP)
    * Pretty Good Privacy (PGP)
    * Smart Cards
    * Public-Key Cryptography Standards (PKCS)
    * Universal Electronic Payment System (UEPS)
    * Clipper
    * Capstone
    * AT&T Model 3600 Telephone Security Device (TSD)

# Politics [4]
    * National Security Agency (NSA)
    * National Computer Security Center (NCSC)
    * National Institute of Standards & Technology (NIST)
    * RSA Data Security, Inc 
    * Public Key Partners
    * International Association for Cryptographic Research (IACR)
    * RACE Integrity Primitives Evaluation (RIPE)
    * Conditional Access for Europe (CAFE)
    * ISO/IEC 9979
    * Professional, Civil Liberties, & Industry Groups
    * SCI.CRYPT
    * Cypherpunks
    * Patents
    * US Export Rules
    * Foreign Import & Export of Cryptography
    * Legal Issues

# Sources
## Books
### 1) Serious Cryptography: A Practical Introduction to Modern Encryption
### 2) Cryptography Engineering: Design Principles and Practical Applications
### 3) Understanding Cryptography: A Textbook for Students and Practitioners
### 4) Applied Cryptography: Protocols, Algorithms and Source Code in C
### 5) Cryptanalysis: A Study of Ciphers and Their Solution 
### 6) Codes, Ciphers, Steganography & Secret Messages
### 7) Hands-On Cryptography with Python
### 8) Practical Cryptography
