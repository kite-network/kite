# Kite Protocol

```
1. noun, slang: A message, note, or letter passed secretly or illegally to, from, or between prisoners.
```

Kite is a community currency for enthusiasts of privacy preserving technologies. 

The Kite community uses a purpose-built ledger for such coins, based on the CosmosSDK.

Freely mine some coins by operating blockchain nodes. There's no premine, or permission needed to join.

## Testnet
Testnets are created in a decentralized manner requiring no permission: just submit a proof of work (more below) when registration opens.

Testnets preserve state: Coins created in each testnet iteration, e.g chain ids: alpha, bravo, charlie,  are rolled over into the next test net.

Participants in each network have an opportunity to recreate data and coins from from a previous test-net account to a new one. Unclaimed Kite coins in testnets are sent to a BURN account, in a new genesis.

## Genesis
Users must submit a proof of work together with a genesis registration. The proof of work artifact is a json file with two fields: preimage, and sha2 hash.

To create such a file a participant must run a miner producing a proof that achieve the following:

- Inputs (preimage), concatenated:
  - public key,
  - hex-encoded chain-id,
  - nonce

- Outputs (hash): A hash with 5 leading zeros.

The miner may increment the nonce in multiple attempts to yield a result.

## Rules for the ledger
A validator operates computer hardware which engages in consensus, a group of these is a validator set.
Epochs, or consensus intervals, last 24 hours, at which time a new validator set is chosen.

Active validators have voting power proportionate to the value of assets in account (i.e. no bonding is necessary).

New coins are created by the ledger only when rewards are granted by the system for database consensus work performed.  The base of coins inflates, they are minted to validators based on a fixed 10% per year inflation schedule, divided equally among participating validators of a given epoch..

No payment is necessary to join the network. Coins can be mined by submitting proofs at genesis, or when joining the network.

The native Kite coin is transferable up to a certain safety limit per epoch. This safety limit increases progressively according to a predefined schedule.

## Governance
There is no governance. This is for everyone's safety.  Make your voice known in this github. Conduct polls if you want your idea incorporated.

## DAO
There is no Dao. This is for everyone's safety.

## Permission
There is no permission.

## Privacy
Do not link your previous identity, and reputation to this project. This is for everyone's safety.

Contributions are accepted from anonymous accounts only. Perhaps use https://www.gitmask.com/

Otherwise use a single-use github account, with single-use email accounts, like the account that created this, and the admins here.
