# foxcryptie

Solidity and Python projects, with code, tests, and notes on what each project does and does not cover.

## Selected projects

- [Solidity Layout Diff](https://github.com/foxcryptie/solidity-layout-diff) — a Python CLI that compares Solidity compiler storage layouts. It reports `PASS`, `REVIEW`, `FAIL`, or `UNASSESSED` and includes regression cases built from checked-in compiler output. It is a first-pass check, not a full upgrade validator.
- [Stablecoin Payment Gateway](https://github.com/foxcryptie/stablecoin-payment-gateway) — a single-token invoice contract with separate pending funds, merchant credit, and protocol fees. Foundry tests cover settlement, refunds, fee-on-transfer rejection, and accounting. The merchant controls settlement and refunds; the payer has no forced refund path.
- [Smart Contract Security Lab](https://github.com/foxcryptie/smart-contract-security-lab) — local Foundry examples of reentrancy, `tx.origin` authorization, and signature replay. Each case has a vulnerable contract, a corrected example, and tests that show the difference.
- [ERC-4626 Vault Lab](https://github.com/foxcryptie/erc4626-vault-lab) — an OpenZeppelin-based vault used to test deposits, withdrawals, share rounding, and how asset donations change share value. It has no yield strategy.

These are learning and reference projects. The contracts have not been independently audited and should not be used with real funds. The security lab deliberately includes vulnerable contracts for local testing.

## Contact

For a scoped contract or Python tooling task, [open a project inquiry](https://github.com/foxcryptie/foxcryptie/issues/new) with the goal, environment, expected behavior, and timeline.
