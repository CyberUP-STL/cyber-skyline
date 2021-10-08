## Overview
XOR undoes itself, so decryption is the same operation as encryption. You can use single bytes or multiple byte keys for XOR. If you feed in two bits and they are the same, then the output is `0`. If the bits are different, the output is `1`. XOR operates on one bit at a time. Python indicates XOR with the `^` operator.
> `0 ^ 0 = 0`  
> `0 ^ 1 = 1`  
> `1 ^ 0 = 1`  
> `1 ^ 1 = 0`  

## Implement in Python

```python
text = raw_input("Enter text: ")
key = raw_input("Enter key: ")
n = len(text)

cipher = ""
for i in range(n):
  t = text[i]
  k = key[i%len(key)]
  x = ord(k) ^ ord(t)
  cipher += chr(x)
print text, key, cipher.encode("hex")
```

---


Source: Hands-On Cryptography with Python, Samuel Bowne, ISBN 978-1-78953-444-3