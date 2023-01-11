## Cryptography

### Encryption, Decryption & Hacking

- Encryption: scrambling the data according to a secret key (in this case, the alphabet shift).
- Decryption: recovering the original data from scrambled data by using the secret key.
- Code cracking: uncovering the original data without knowing the secret, by using a variety of clever techniques.

- There are three main techniques to decrypt ciphers:
  - Frequency Analysis
    - human languages use some letters more than others. we can analyze the frequency of the characters in the message and identify the most likely 'E' (the most common letter in English) and narrow down the possible shift amounts based on that.
  - Known Plaintext
    - The original unencrypted message is called plaintext. We may be able to crack the code if you know some part of the original message.
  - Brute Force
    - You could just test each possible shift of the alphabet and see if any make sense with the first couple words.

### Ceasar Cipher

- One of the earliest encryption techniques is the Caesar Cipher, invented by Julius Caesar more than two thousand years ago to communicate messages to his allies. The Caesar Cipher is a great introduction to encryption, decryption, and code cracking, thanks to its simplicity.

### Cryptography Crash Course

- Crypto(secret) + graphy(writing)
- Substitution Ciphers
  - replace every letter in a message with something else, according to a translation
- Permutation Ciphers
  - put a message into a grid, and then encode them into a different order
- Enigma
  - enigma rotor typewriter. it used substitution ciphers, but there were three rotors, so it wasn't just E = L, E might be a different letter every time it shows up
- AES
  - In the 1970s, encryption moved from hardware to software. many many more possible combinations, so brute force decrypting is basically impossible
- One Way Functions
  - 
- 

### Sources

[Encryption, Decryption & Hacking](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)<br>
[Ceasar Cipher](https://en.wikipedia.org/wiki/Caesar_cipher)<br>
[Cryptography Crash Course](https://www.youtube.com/watch?v=jhXCTbFnK8o)<br>
[Introduction to Cryptography](https://thebestvpn.com/cryptography/)<br>
[How Computers Generate Random Numbers](https://www.howtogeek.com/183051/htg-explains-how-computers-generate-random-numbers/)<br>