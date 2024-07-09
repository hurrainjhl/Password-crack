# Multi-Attack

To run John the Ripper faster and use it with multiple processes, 

you can use the `fork` option. This is useful for multicore processors.

```bash
john hash.txt --fork=3
```

```fork=3 ```tells John to create three processes for cracking the password, utilizing multiple cores for faster processing.
