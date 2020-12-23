# org.groestlcoin.electrum-grs

Flatpak build of [electrum-grs](https://www.groestlcoin.org/groestlcoin-electrum-wallet/).

## Building

The `python3-requirements*` files are built
using
[these](https://github.com/Groestlcoin/electrum-grs/tree/master/contrib/deterministic-build)
deterministic requirements files,
and `flatpak-pip-generator` from
[flatpak-builder-tools](https://github.com/flatpak/flatpak-builder-tools/), with
a few modifications.


## User data

Wallets are located at `~/.var/app/org.groestlcoin.electrum-grs/.electrum-grs`, to use
`~/.electrum-grs` instead, give the app filesystem permissions

``` sh
flatpak override --filesystem=home org.groestlcoin.electrum-grs
```
