# ECC Chat Demonstration

An educational web application demonstrating Elliptic Curve Cryptography (ECC) for secure chat communication.

## Features

### 1. Curve Selection
- Choose from three standard elliptic curves:
  - **P-256** (secp256r1) - 256-bit security
  - **P-384** (secp384r1) - 384-bit security
  - **P-521** (secp521r1) - 521-bit security

### 2. Curve Parameters Display
Shows the mathematical foundation of ECC:
- **Curve Equation**: y² = x³ + ax + b (mod p)
- **Prime Field (p)**: The finite field over which the curve is defined
- **Generator Point (G)**: The primitive element (base point) used for key generation
- **Order of the Group (n)**: The number of points on the curve
- **Cofactor (h)**: Ratio of total points to the order

### 3. Key Generation Process
For each user (Alice and Bob):
1. Select a random private key: d ∈ [1, n-1]
2. Calculate public key: Q = d × G (scalar multiplication)
3. Display both keys with clear visual distinction

### 4. Public Key Exchange
- Users share their public keys with each other
- Visual confirmation when keys are sent
- Visual confirmation when keys are received
- Private keys remain secret throughout

## How to Run

Simply open `index.html` in a modern web browser (Chrome, Firefox, Edge, Safari).

No server or installation required!

## Presentation Flow

1. **Start**: Explain what ECC is and why it's used
2. **Curve Selection**: Show different curve options and their security levels
3. **Show Curve Details**: Display the mathematical parameters
4. **Generate Keys**: Click both "Generate Keys" buttons
5. **Explain Keys**: Show the difference between private (secret) and public (shareable) keys
6. **Exchange Keys**: Click both "Send Public Key" buttons
7. **Confirm Receipt**: Show that both users now have each other's public keys

## Educational Points to Highlight

- **Private Key**: Random number that must be kept secret
- **Public Key**: Derived from private key using elliptic curve point multiplication
- **Generator Point (G)**: The starting point for all key generation
- **Order (n)**: Defines the size of the key space
- **Security**: Larger curves (P-521) provide more security but require more computation

## Next Steps (Future Enhancements)

- Message encryption using received public keys
- Message decryption using private keys
- Shared secret generation (ECDH)
- Digital signatures (ECDSA)

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6+)
- Web Crypto API (native browser cryptography)
