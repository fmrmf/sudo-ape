# sudo-ape

Charts for sudooooo swap using ApeWorX


## Setup

Most of the [sudoswap](https://github.com/sudoswap/lssvm) pair contracts `LSSVMPair.sol` are **not** verified on Etherscan, so I went for a manual workaround by compiling locally in this project. This allows using ApeWorX's out-of-the-box `Contract` functionality to query for the events we care about.

Relevant needed contracts are in the `contracts/` folder. Simply

```
ape compile
```

and the notebook should run fine. Then,

```
ape notebook
```


## TODOs

For a given collection address, plot over all existing pools:

- [ ] prices and volume
- [ ] liquidity
- [ ] % slippage (curve) and fee metrics (or normalize by these)
- [ ] arbitrage opportunities (price differences between pools)
