# Base64 Encoding
## Overview
First lets cover encoding ASCII data as bytes and base64 encoding those bytes. 

In ASCII, each character equates to one byte:
> `A` is `65` in `Base 10`, and in binary, it is `0b01000001`.  
> `B` is `66` in `Base 10`, and in binary, it is `0b01000010`.  
> `C` is `67` in `Base 10`, and in binary, it is `0b01000011`.  

So the string `ABC` can be interpreted as a 24-bit string that looks like  
> `0b01000011|01000010|01000001`

To interpret this bit string as Base64, we need to break it into groups of 6 bits.  
6 bits have a total of 64 combinations, so you need 64 characters to encode it.  

We use the capital letters for the first 26, lowercase letters for another 26, the digits for another 10, which gets you up to 62 characters. In the most common form of base64, you use `+` and `/` for the last two characters.  
The `=` is used to indicate padding if the input string length is not a multiple of 3 bytes:  
> `'ABC'` is `0b01000011|01000010|01000001`  
> 6-bit groups `0b010000|110100|001001|000001`  
> Decimal `16` `20` `9` `3`  
> Base64 `Q` `U` `J` `D`  

## Implement in Python
Base64 Input: `U2FtcGxlIHRleHQ=`
```python
a = raw_input("Enter encoded text:")

for i in range(6):
  a = a.decode("base64")
  print i, a
```

---


Source: Hands-On Cryptography with Python, Samuel Bowne, ISBN 978-1-78953-444-3