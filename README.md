# TNLS
This repository is a beta implementation of the Secretpath (formerly Snakepath) Network and its underlying TNLS protocol, currently connecting the Eth  testnet to the Secret Network pulsar-3 testnet.

This project was started by Leor Fishman, Benjamin Simon, Kent Worchester. Continued by Alex | Secret Saturn.

Docs (which are relatively barebones atm but will be being improved over time) can be found at [the docs](https://fortress-labs.gitbook.io/snakepath/) and [the docs] (https://docs.scrt.network/secret-network-documentation/development/ethereum-evm-developer-toolkit/basics/cross-chain-messaging/snakepath)

# Usage (for Nunya)

## Custom Relayer

This branch "nunya" in this fork of https://github.com/SecretSaturn/SecretPath is used to run a custom Relayer for https://github.com/svub/nunya.

### Configuration

It is necessary to generate the .env file, as shown below, and then add an Ethereum and Secret Network private keys in the .env file, excluding their '0x' prefix, as specified in the https://github.com/svub/nunya setup instructions.
```
cp ./TNLS-Relayers/.env.example ./TNLS-Relayers/.env
```

Note: ./TNLS-Relayers/config.yml should be automatically updated via scripts by https://github.com/svub/nunya that uses it as a Git Submodule.

## Custom Gateway

The directory ./SecretPath/TNLS-Gateways/public-gateway has been cloned and used in ./packages/secret-contracts/secret-gateway of this repo https://github.com/svub/nunya/pull/33

# License

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
