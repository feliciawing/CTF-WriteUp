# MetaCTF 2021

## Unbreakable Encryption

>There is a form of truly unbreakable encryption: the one time pad. Nobody, not Russia, not China, and not even Steve, who lives in his mom's basement and hacks governments for fun, can decrypt anything using this cipher... as long as it's used correctly. In this scheme, a truly random string as long as the plaintext is chosen, and the ciphertext is computed as the bitwise XOR of the plaintext and the key. However, if the key is reused even once, it can be cracked. We've intercepted some messages between some criminals, and we're hoping you could crack the one time pad they used. We're pretty sure they reused it, so you should be able to crack it...
>
>Ciphertext 1: 4fd098298db95b7f1bc205b0a6d8ac15f1f821d72fbfa979d1c2148a24feaafdee8d3108e8ce29c3ce1291
>
>Plaintext 1: hey let's rob the bank at midnight tonight!
>
>Ciphertext 2: 41d9806ec1b55c78258703be87ac9e06edb7369133b1d67ac0960d8632cfb7f2e7974e0ff3c536c1871b

### Steps

So we know that one time pad used twice becomes decryptable. So here we used [two-time pad cracker](https://www.tausquared.net/pages/ctf/twotimepad.html).

Here we put the ciphertext 1 and 2

![](img/hex.png)

Then because we already know the plaintext 1 we could insert it there and there we go, we found the plaintext 2 which is the flag

![](img/flag.png)

Flag : `MetaCTF{you're_better_than_steve!}`