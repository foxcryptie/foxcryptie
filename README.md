# foxcryptie

Current focus: Solidity storage, payment accounting, and tests that show what a contract actually does. I also write small Python tools when they help with that work.

If you want to judge the code, these are good places to start:

- [Solidity Layout Diff](https://github.com/foxcryptie/solidity-layout-diff) reads `solc` storage-layout JSON and flags moved variables, type changes, and storage-gap cases. The examples are checked-in compiler output, so the tests can run without `solc`. A `PASS` covers storage layout only.
- [Stablecoin Payment Gateway](https://github.com/foxcryptie/stablecoin-payment-gateway) tracks pending invoice payments, merchant balances, and fees for one ERC-20 token. The tests follow those balances through payment, refund, settlement, and withdrawal. The merchant decides whether to settle or refund.
- [Smart Contract Security Lab](https://github.com/foxcryptie/smart-contract-security-lab) pairs three deliberately broken contracts with focused fixes. Start with the tests: they show the reentrant withdrawal, the `tx.origin` relay, and a reused signature before checking the corrected paths.
- [ERC-4626 Vault Lab](https://github.com/foxcryptie/erc4626-vault-lab) is an OpenZeppelin vault with a donation function. The tests are about share prices and rounding after assets arrive without new shares. It does not generate yield.

These are reference and learning projects. The contracts have not been audited or deployed as financial products. The security lab's vulnerable contracts are for local tests only.

For a scoped contract or tooling task, [open an issue here](https://github.com/foxcryptie/foxcryptie/issues/new) with the environment, expected behavior, and what would count as done.
