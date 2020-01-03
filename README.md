# This is my public drive thing

## What the f*** is this?
Github doesn't have any hard limits for repos (the max size is 100GB for a repo and 100MB per file). This means that if I divide my files enough I can encrypt them to prevent you guys from seeing them and have lots of storage that I don't have to keep on my own computer :)

## Can I see some of your files?
No, unless I share with you the aes passwords.

## What encryption do you use?
I'm using openssl to encrypt my stuff, because I'm too lazy to deal with rsa and pgp. I hope whoever forks this repo is ok with using AES or changing the scheme.

# How to use

## First...
None of the files that do not end in `.enc.backup` or `.enc` will be pushed, save for `README.md`, `.gitignore`, and the helper programs.
(Almost) All unencrypted files not be pushed to master.

### Setting up
run `git clone https://github.com/Lee-Garcon/public-drive.git`
run `cd public-drive`
run `chmod +x ./checkout ./decrypt ./encrypt`

### To encrypt a directory:
run `./encrypt [directory]`, where `[directory]` is the directory that you want to encrypt.
The program will prompt you with a password (and then ask you to confirm the password). Remember the password for decryption. The process will not overwrite anything that you have.
The program will push the current repo to the master branch.

### To decrypt a directory:
run `./decrypt [file]`, where `[file]` is the file that you want to decrypt. Make sure that the file ends with `.enc` or the script will break and cause the events of Terminator to happen.

# I do not have any weird files stored here.

## Nope, definitely not
