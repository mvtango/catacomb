# catacomb

Encrypts content using public keys from GitHub.
Encrypted files can then be decrypted using the matching `~/.ssh/id_rsa`.

## Installation

Using [fresh], run the following:

``` sh
fresh mvtango/catacomb bin/catacomb --bin
```

Manually:

``` sh
mkdir ~/bin/
wget https://raw.github.com/mvtango/catacomb/master/bin/catacomb ~/bin/catacomb
export PATH="$PATH:~/bin/"
# the PATH will need to be set in your shell config
```

## Usage


      cat plain.txt | catacomb [public_key_file|github handle] >cipher.txt

      or

      cat cipher.txt | catacomb [secret_key_file] >plain.txt


## Notes

* Encrypts using a key file or the first key retrieved from GitHub
* Decrypts using the key file provided on the command line.`

## Licence

MIT.

## Forked from 

<https://github.com/twe4ked/catacomb/blob/master/bin/catacomb>

[fresh]: https://github.com/freshshell/fresh
