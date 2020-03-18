# Password-Manager2.0
Fully encrypted password manager. Good for ssh servers

## How to use it
First, copy  all of files. Edit 'master-password.txt' and write there SHA512 hash with your password, and save this file.
Now, your password manager is ready to use.

### What is key, and how to use it
Key is needed to encrypt your password using cesar algorithm. Type a number like 10 or 5. You have to remember it.

### How to make SHA512 hash?
Open your python console and type:

>>> import hashlib
>>> hash = hashlib.sha512()
>>> hash.update("--your password--".encode())
>>> hash = hash.hexdigest()
>>> hash

And copy output of 'hash' and paste it into 'master-password.txt' file. Save this file and that's it.

## Known bugs
I don't know any bug. If you found something, add it to issues.
