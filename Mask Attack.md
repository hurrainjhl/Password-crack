# Mask Attack and Clearing Cached Passwords

## Mask Attack

If you know the structure or type of password, you can use a mask attack with John the Ripper. Here's how:

- `?d` indicates a digit.
- `?d?d?d` will check all combinations of 3 digits.
- You can specify `?l` for lowercase letters or `?u` for uppercase letters.

```bash
john --mask='?d?d?d' hash.txt
```

#### Clearing Cached Passwords

To clear cached passwords and remove the `john.pot` file:

##### Using `sudo find` and `rm` (Recommended)

This command searches the entire filesystem for a file named `john.pot`, suppresses permission error messages, and removes the file using `sudo`.

```bash
sudo find / -name "john.pot" -exec rm {} \; 2>/dev/null
```

#### Checking for `john.pot`

To check the location of `john.pot` without removing it:

```bash
find / -name "john.pot" 2>/dev/null
```
#### Removing `john.pot`

The `john.pot` file is used by John the Ripper to store cracked passwords.

##### Manually Removing `john.pot`

To manually remove `john.pot`, use the following commands:

```bash
find -name "john.pot"
```

```bash
sudo rm ./.john/john.pot
```


This Markdown section provides clear instructions on manually removing the `john.pot` file, which is used by John the Ripper for storing cracked passwords.

