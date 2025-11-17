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
* @aws-sdk/crc64-nvme-crt: RVFaKT3n9gw=
* Crc64Nvme: RVFaKT3n9gw=

Benchmark:
CrtCrc64Nvme x 977,782 ops/sec ±18.56% (66 runs sampled)
Crc64Nvme x 29,763 ops/sec ±0.79% (90 runs sampled)
Fastest is CrtCrc64Nvme
```
