# caesar
**Points:** 100

## Category
Cryptography

## Task
Decrypt this [message](https://2019shell1.picoctf.com/static/1f33970830e651254c964ee5d04f0e85/ciphertext). You can find the ciphertext in /problems/caesar_6_238b8f4604d91ecb59cda5b4f0e66fc8 on the shell server.

# Solution
As the name of the challenge suggests, we have to decrypt the caesar cipher. And for that we'll use [this](https://cryptii.com/pipes/caesar-cipher) online website.

The letters were rotated 15 times (a>p, b>q, etc). Hence the plaintext is ```crossingtherubiconojovpqjs```

# Flag
> picoCTF{crossingtherubiconojovpqjs}
