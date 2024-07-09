## Getting the Hash

To begin, you need to extract the hash from the password-protected file.

In this example, we use `office2john` to get the hash from a `.docx` file.

```bash
office2john crackme.docx > hash.txt
```
1: ```office2john``` is part of the John the Ripper suite, used to extract password hashes from Microsoft Office files.

2:```crackme.docx``` is the password-protected file.

3:```hash.txt``` is the file where the extracted hash will be saved.
