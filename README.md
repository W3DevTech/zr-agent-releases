# zr-agent releases

Release assets for **zr-agent**, the node agent of the zyber runner fleet. This repository holds no source code: each
release (`vX.Y.Z`) carries the agent binaries, `SHA256SUMS`, its minisign signature and `install.sh`.

## Install

```sh
npx @w3devx/zr-agent@<version> install --join <join token from the dashboard>
```

## Verify a release by hand

```sh
minisign -Vm SHA256SUMS -P RWRi1XVbz09Qp5TTZ0iefap1wtuBahGfzIp5j4z5KDXfM0bn05ImR3zc
sha256sum -c SHA256SUMS --ignore-missing
```

Release signing public key (minisign):

```
RWRi1XVbz09Qp5TTZ0iefap1wtuBahGfzIp5j4z5KDXfM0bn05ImR3zc
```
