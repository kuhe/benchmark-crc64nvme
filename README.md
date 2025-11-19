# benchmark-crc64nvme

Benchmark various CRC64NVME implementations on Node.js

## Pre-requisites

- Install **Node.js** by following these steps:
  1. Install [nvm](https://github.com/nvm-sh/nvm#installation-and-update).
  1. Use node v24.x.x by running `nvm use` or `nvm use 24` in a terminal window.
  1. Verify that node is installed by running `node -v` in a terminal window and confirm that it shows Node.js >=24, such as `v24.11.0`).
  1. Enable corepack by running `corepack enable` in a terminal window.
- Install dependencies by running `pnpm i`.
- Run benchmark with `pnpm benchmark:crc64nvme`.

## Setup

```console
$ node -v
v24.11.1

$ pnpm benchmark:crc64nvme

...

CRC32NVME values returned for random buffer:
* @aws-sdk/crc64-nvme-crt: URp3/lNbSBU=
* Crc64Nvme              : URp3/lNbSBU=
* Crc64Nvme2             : URp3/lNbSBU=

Benchmark:
CrtCrc64Nvme x 942,009 ops/sec ±17.90% (67 runs sampled)
Crc64Nvme x 29,465 ops/sec ±2.48% (90 runs sampled)
Crc64Nvme2 x 92,237 ops/sec ±2.44% (96 runs sampled)
Fastest is CrtCrc64Nvme
```
