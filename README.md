# Sample repository for git-crypt setup

## git-crypt installation

**Windows**: https://github.com/oholovko/git-crypt-windows#installation

**Mac**: `brew install git-crypt`

## Setup instructions

Run once per repository:
```
$ git-crypt init
$ git-crypt export-key ../git-crypt-key
```

## Usage instructions

Run once per user:
```
$ ./unlock.py "<base64-encoded-key>"
```

Anything inside of the `secrets/` directory will automatically be encrypted. Simply commit the secrets, and they will be encrypted.

To check whether your files will be encrypted, run `git-crypt status`.

Check [the docs](https://www.agwa.name/projects/git-crypt/) for information on how to edit `.gitattributes` and configure encrypted paths.