# Rotation Cipher Encoding
## Overview
A Caesar cipher (Also known as ROT13) is an ancient trick where you just move every letter forward three characters in the alphabet.  
Here is an Example: 
>  PlainText `ABCDEFGHIJKLMNOPQRSTUVWXYZ`  
> CipherText `DEFGHIJKLMNOPQRSTUVWXYZABC`

So if you were to put `hello` through a Caesar cipher with shift 3, it would become `khoor`

## Implement in Python
### PlainText -> CipherText
```python
alpha =  "ABCDEFGHIJKLMNOPQRSTUVWXYZ"

str_in = raw_input("Enter message, like HELLO: ")
shift = int(raw_input("Shift value, like 3: "))

n = len(str_in)
str_out = ""

for i in range(n):
   c = str_in[i]
   loc = alpha.find(c)
   newloc = (loc + shift)%26
   str_out += alpha[newloc]

print "Obfuscated version:", str_out
```

In case you haven't noticed, this code will work for converting both to and from CipherText.  
That is because all that a ROT13/Caesar Cipher does is rotate the characters $X characters

---


Source: Hands-On Cryptography with Python, Samuel Bowne, ISBN 978-1-78953-444-3