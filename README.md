# JS Crypto Performance
[![DOI](https://zenodo.org/badge/73430536.svg)](https://zenodo.org/badge/latestdoi/73430536)

Performance measurement of three JavaScript public-key cryptography implementations: JSEncrypt, Forge and SubtleCrypto (native).

## Results
Run on Windows 10, Chrome 61.0.3163.100, Intel i7-4810MQ, with 16GB RAM.


|                               | JSEncrypt            | Forge                | SubtleCrypto          |
|-------------------------------|----------------------|----------------------|-----------------------|
| **Generate 2048-bit RSA key** | 0.11 ops/sec ±32.39% | 7.46 ops/sec ±16.80% | 7.71 ops/sec ±18.79%  |
| **Encrypt**                   | 1,132 ops/sec ±0.69% | 975 ops/sec ±0.63%   | 16,767 ops/sec ±1.72% |
| **Decrypt**                   | 32.59 ops/sec ±0.29% | 34.07 ops/sec ±0.44% | 1,618 ops/sec ±1.19%  |
