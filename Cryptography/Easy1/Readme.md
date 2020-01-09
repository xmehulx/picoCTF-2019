# Easy1
**Points:** 100

## Category
General Skills

## Task
The one time pad can be cryptographically secure, but not when you know the key. Can you solve this? We've given you the encrypted flag, key, and a table to help ```UFJKXQZQUNB``` with the key of ```SOLVECRYPTO```. Can you use this [table](https://2019shell1.picoctf.com/static/30d4405c34cf6490b082e6cf8f56ac56/table.txt) to solve it?

# Solution
We are given a ciphertext and a key used to encrypt the original text. So, basically we have to backtrace our step and find original letters when crossed with the key give the encrypted letters.

| Original | Key | Cipher |
|:--------:|:---:|:------:|
|  **C**   |  S  |   U   |
|  **R**   |  O  |   F   |
|  **Y**   |  L  |   J   |
|  **P**   |  V  |   K   |
|  **T**   |  E  |   X   |
|  **O**   |  C  |   Q   |
|  **I**   |  R  |   Z   |
|  **S**   |  Y  |   Q   |
|  **F**   |  P  |   U   |
|  **U**   |  T  |   N   |
|  **N**   |  O  |   B   |

# Flag
> picoCTF{CRYPTOISFUN}
