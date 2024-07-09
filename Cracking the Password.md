# Cracking the Password

Once you have the hash, you can use John the Ripper to crack the password.

```bash
john hash.txt
```


> By default, John the Ripper will first try with a single-core attack, checking file name combinations, then the default dictionary, and finally performing a brute force attack.
The cracked password will be shown.
To check the cracked password:

```
john --show hash.txt
