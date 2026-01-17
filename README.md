# CLASSICAL CYPHERS

## ENCRYPTION AND DECRYPTION OF SOME COMMON CLASSICAL CYPHERS.
Encryption is done using a specified key, decryption is done using the same key, while breaking a cypher means decrypting the cypher without knowing the key used during encryption.

Typical methods used for breaking a classical cypher are frequency analysis and pattern recognition.

The English alphabets A - Z would be used for the illustrations.

The cyphers that would be examined includes:
[Atbash Cypher](#atbash-cypher)   
[Ceaser Cypher](#ceaser-cypher)
[Playfair Cypher](#playfair-cypher)
[Vigenere Cypher](#vigenere-cypher)
[Hill Cypher](#hill-cypher)

Atbash and ceaser cyphers are mono alphabetic cyphers. That is, one-to-one alphabet substitution cyphers.

Playfair cypher is the best known two - letter multi alphabetic cypher (Diagram). That is, two-to-two alphabets substitution cypher.

Vigenere cypher is a poly alphabetic substitution cypher.

## Atbash cypher
This is the simplest type of cypher which uses a one-to-one direct substitution. Encryption is achieved by reversing the alphabets of the plaintext, decryption is achieved by reversing the alphabets of the cyphertext, and breaking of the cypher is achieved by using pattern recognition.
Illustration is shown.

## Ceaser cypher
This is a direct one-to-one substitution of the alphabets using a specified step or count. It can also be achieved using mathematical notation given by:

Encryption: c = E(k, p)
c is the cypher text,
E is the encryption function, (p + K) mod 26
K is the key (specified count)
p is the plain text
26 is the number of alphabets

Decryption: p = D(k, c)
D is the decryption function, (c - k) mod 26

An example of the ceaser cypher is ROT13, which uses a step or count of 13 alphabets as the key. The counting wraps around after the last alphabet.
Illustration is shown.

A variation of the ceaser cypher, in which it is more difficult to guess the key is known as the Multiplicative Cypher. In this instance, it is important that the Greatest Common Divisor (gcd) of the key value and 26 is 1. This will be relevant during decryption.

Encryption: c = (p * k) mod 26
Decryption: p = (c * k-¹) mod 26
k-¹ is the multiplicative inverse of k (key)
Recall gcd(k, 26) = 1. It is only when this is true that k would have a multiplicative inverse.
Illustration is shown.

## Playfair cypher
This is the best known example of a multi alphabetic substitution cypher. A multi alphabetic substitution cypher is not a one-to-one substitution cypher, but rather, a many-to-many substitution cypher. Playfair uses a two-to-two substitution, which are called diagrams.
It’s algorithm is based on the use of a 5 * 5 matrix of letters constructed using a keyword. Illustration is shown.

## Vigenere cypher
This is a one-to-one poly alphabetic substitution cypher. This means that the same plaintext letter is not always encrypted to the same cyphertext letter. Illustration is shown.

## Hill cypher
This is a many-to-many substitution cypher, where the number of alphabets to be substituted can be any value greater than one. Illustration is shown.
