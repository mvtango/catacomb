# catacomb


**forked from <https://github.com/twe4ked/catacomb> - great stuff, 
I just wanted flexibility with decrypthion!**


Encrypts STDIN to STDOUT using public ssh key files or public 
ssh keys from GitHub.

Decrypts STDIN to STDOUT using secret ssh key files.

## Installation

Using [fresh], run the following:

``` sh
fresh twe4ked/catacomb bin/catacomb --bin
```

Manually:

``` sh
mkdir ~/bin/
wget https://raw.github.com/twe4ked/catacomb/master/bin/catacomb ~/bin/catacomb
export PATH="$PATH:~/bin/"
# the PATH will need to be set in your shell config
```

## Usage

### Encrypting

``` sh
catacomb $recipients_github_username|public key filename  < file.txt > encrypted.txt
```

### Decrypting

``` sh
catacomb $secret_key_filename < encrypted.txt
```

## Licence

MIT.

[fresh]: https://github.com/freshshell/fresh
