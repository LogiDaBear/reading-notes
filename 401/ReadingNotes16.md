# Cryptography
- [caesar salad](https://en.wikipedia.org/wiki/Caesar_cipher)
- [encryption, decryption y hacking](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)

- [video Cryptography crash course](https://www.youtube.com/watch?v=jhXCTbFnK8o)

## What is the basic principle behind the Caesar Cipher, and how was it used historically?

Historically, the Caesar Cipher was used by Julius Caesar himself during the Roman Empire to communicate securely with his generals. The shift value was known to both the sender and the receiver, allowing them to encrypt and decrypt messages. However, as the cipher is relatively simple, it is vulnerable to brute-force attacks. With only 25 possible shift values, it can be easily broken by trying all possible keys.
- shift
- encryption
- decryption

Despite its vulnerability, the Caesar Cipher still serves as an introductory example in cryptography and provides a foundation for more advanced encryption techniques. It demonstrates the concept of substitution ciphers and the importance of key management in encryption systems.

## What are the key differences between symmetric and asymmetric encryption? How is asymmetric used in secure communication today?
The key difference is in their operation and usage- symmetric encryption is generally faster than asymmetric encryption but also is less secure

Asymmetric encryption is widely used in secure communication today for various purposes:

Confidentiality: Asymmetric encryption is used to establish a secure channel for exchanging symmetric keys in symmetric encryption schemes. For example, in the widely used Transport Layer Security (TLS) protocol, asymmetric encryption is used during the initial handshake phase to negotiate a shared symmetric key, which is then used for faster symmetric encryption.

Digital Signatures: Asymmetric encryption is used to create digital signatures, which provide integrity and authentication. The private key is used to sign the data, and the corresponding public key is used to verify the signature. This ensures that the data has not been tampered with and that it originated from the expected sender.

Key Exchange: Asymmetric encryption is used for secure key exchange in protocols like Diffie-Hellman key exchange. It allows two parties to establish a shared secret key over an insecure channel without explicitly transmitting the key.

## How do computers generate random numbers, and what are the differences between true random number generation (TRNG) and pseudo-random number generation (PRNG)? Discuss their use cases in cryptography.

Computers generate random numbers using different methods, and there are two primary types of random number generation: true random number generation (TRNG) and pseudo-random number generation (PRNG)
### key differences
- Randomness: TRNGs produce genuinely random numbers based on unpredictable physical processes, while PRNGs generate numbers that are statistically random but ultimately deterministic.
- Seed Dependency: PRNGs require an initial seed value, and if the seed is known or predictable, the entire sequence of numbers can be reproduced. TRNGs are not dependent on seed values.
- Speed and Efficiency: PRNGs are computationally efficient and can generate a large number of pseudo-random numbers quickly. TRNGs, on the other hand, may be slower as they rely on physical processes.
- Entropy Source: TRNGs require a reliable and unpredictable entropy source, which can be challenging to maintain. PRNGs do not have this strict requirement.

## What’s the difference between encryption and decryption? Explain with an analogy.

Encryption is like putting the secret message inside a locked box. You have a special key that only you and your friend know. You use this key to lock the box and make sure nobody else can read the message inside. It's like hiding the message in a secret code that only you and your friend understand. Once the message is encrypted, it becomes difficult for anyone else to understand what it says.

Decryption, on the other hand, is like opening the locked box with the special key. When your friend receives the locked box, they use the key that matches the lock to unlock it. Now they can read the message inside, as it's no longer in the secret code. Decryption is the process of converting the encrypted message back to its original form, making it understandable again.

So, encryption is like locking the message inside a box, and decryption is like opening the box with the right key to read the message. By using encryption and decryption, you can keep your secret message safe from others who may try to read it. 

## Things I wanna kno understand gooder
How to snek wif compiter