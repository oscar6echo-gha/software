# Software

Ref <https://github.com/mamba-org/micromamba-releases/releases>

```sh
VERSION=1.4.5-0
NAME=micromamba-linux-64
URL=https://github.com/mamba-org/micromamba-releases/releases/download/$VERSION/$NAME
URL_SHA=$URL.sha256

wget $URL -O $NAME
wget $URL_SHA -O $NAME.sha256

echo "$(cat $NAME.sha256)  $NAME" | sha256sum --check
# micromamba-linux-64: OK
```
