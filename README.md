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