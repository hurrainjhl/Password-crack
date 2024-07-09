# Dictionary Attack Using Rockyou

To use the Rockyou dictionary for a dictionary attack with John the Ripper, follow these steps:

1. Uncompress the Rockyou file if it is not already extracted:

```bash
gunzip /usr/share/wordlists/rockyou.txt.gz
```
2. Verify the extraction:
   
  ```bash
  ls /usr/share/wordlists/
```

3. Use the rockyou.txt wordlist:

   ```bash
   john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt 

or

```bash
john --w=/usr/share/wordlists/rockyou.txt hash.txt
```
