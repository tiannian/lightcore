# Lightcore

> An experimental absolute distributed UTXO system with unlimited TPS and Offline transaction.

## Inspired

- China CBDC origin design (DC/EP).
- Bitcoin
- MimbleWimble
- Bulletproof
- MicroService

## Core Design

- Offline UTXO
- Aggregated Pedersen Commitment
- Aggregated Range Proof
- MicroService
- Distributed timestamp by BFT

## Architecture

## Design

### Coin

Coin is a data with special construction, each Coin has it owned value.

Origin coin is a data without cryptographic info.

``` rust
struct OriginCoin {
  pub value: u64,
  pub owner: Point,
  pub id: Hash,
  pub issuer: Sign,
}

struct VerifiableCoin {
  pub 
}
```

### Original Transfer
> Sender and Receiver must be online.



#### Delay Transfer
> When transfer happend, Sender and Receiver can offline, when
#### Receiver Proxy
> Use Proxy make Receiver offline to receive token.

