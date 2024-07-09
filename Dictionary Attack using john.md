# Dictionary Attack Using John

You can use a dictionary attack with John the Ripper by specifying a wordlist. This example uses the inbuilt dictionary file.

```bash
john --w hash.txt
```

```--w``` refers to --wordlist or --wordlist=FILE, 

which specifies a wordlist to use for cracking passwords.
