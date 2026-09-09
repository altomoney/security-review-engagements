# Alto Security Review Engagements

This repository contains all available security audit reports for Alto protocol smart contracts and infrastructure.

## About Alto's Security Program

Security is a top priority at Alto. We engage with leading security firms to conduct thorough audits of our codebase. All findings are addressed before deployment, and completed reports are published here for transparency.

## Completed Audits

| Date | Provider | Scope | Technical Scope | Report |
|:-----|:---------|:------|:----------------|:-------|
| June 2026 | Cantina | Lending, liquidations & Peg Stability Module | Changes to `AltoBaseMarket` from [PR #518](https://github.com/altomoney/v1/pull/518); `LiquidationPeriphery`; the `AdvancedPermissionsUsm` and `AdvancedPermissionsFeeStrategy` extensions from [PR #512](https://github.com/altomoney/v1/pull/512) and [PR #513](https://github.com/altomoney/v1/pull/513)<br>Reviewed version: [`da40ba42`](https://github.com/altomoney/v1/tree/da40ba42) | [📄 View Report](./reports/cantina_alto_money_jun2026.pdf) |
| April 2026 | Cantina | Lending vault | `AltoVault`; `AltoBalancesLib`; `MarketLib`; `PendingLib`; `AltoAdapter`<br>Reviewed version: [`b1d504fc`](https://github.com/altomoney/v1/tree/b1d504fc) | [📄 View Report](./reports/report-cli-cantina-2032a5c5-8cb7-433b-bdfe-64b0cde36cac-alto-phaze-solo.pdf) |
| February 2026 | Cantina | Lending | `AltoBaseMarket`; `AltoBorrowMarket`; `AltoMintMarket`; `AdaptiveCurveIrm`; `FixedRateIrm`; `AltoLeverage`; `AltoLeverageSwapper`; `AssetShareConversionMath`; `ExpLib`; `Uint128Converter`; `DlbDcfPriorityLiquidationEngine`; `AdapterContractApproval`; `FixedPointMath`; `AltoTimelockController`; `market*` functions in `AltoAdapter`<br>Reviewed version: [`75f40717`](https://github.com/altomoney/v1/tree/75f40717) | [📄 View Report](./reports/report-cli-cantina-altomoney-0114.pdf) |
| December 2025 | Cantina | Oracles, DUSD, vesting & leverage | ERC-4626 ratio, Chainlink, Curve, Uniswap, multi-Chainlink, and rewards oracles; `DUSD`; `AltoVesting`; `AltoLeverageSwapper`<br>Reviewed version: [`2cae67d9`](https://github.com/altomoney/v1/tree/2cae67d9) | [📄 View Report](./reports/report-cantinacode-alto-money-solo-1204.pdf) |
| November 2025 | Cantina | Peg Stability Module | `DUSDUsm`; `FixedFeeStrategy`; `FixedPriceStrategy`; `Usm`<br>Reviewed version: [`75fd6ea2`](https://github.com/altomoney/v1/tree/75fd6ea2) | [📄 View Report](./reports/report-cantinacode-alto-money-1124.pdf) |
| November 2025 | Bailsec | Staking & rewards | `IAltoStaking`; `ITVLWeightedContainers`; `AltoStaking`; `TVLWeightedContainers`; `AltoRewardsDistributor`; `AltoReferralWhitelistAdapter`; `MerkleRootManager`; `stakingLock`, `stakingUnlock`, and `rewardsDistributorClaimRewardTokens` in `AltoAdapter`<br>Reviewed version: [`282aee08`](https://github.com/altomoney/v1/tree/282aee08b4a53f753fa11e05e5139b27dcefe272) | [📄 View Report](./reports/Bailsec%20-%20ALTO%20-%20Staking%20Rewards%20-%20Final%20Report.pdf) |
| November 2025 | Enigma Dark | Oracles, DUSD, vesting, leverage & staking | ERC-4626 ratio, Chainlink, Curve, Uniswap, multi-Chainlink, and rewards oracles; `DUSD`; `AltoVesting`; `AltoLeverageSwapper`; `IAltoStaking`; `ITVLWeightedContainers`; `AltoStaking`; `TVLWeightedContainers`; `stakingLock` and `stakingUnlock` in `AltoAdapter`<br>Reviewed version: [`4bff7afb`](https://github.com/altomoney/v1/tree/4bff7afb040ee83dce14016b2c206009ce91a759) | [📄 View Report](./reports/2025-11_Managed_Security_Review_Alto_foundation.pdf) |
| November 2025 | Bailsec | Lending & leverage | `AltoBaseMarket`; `AltoBorrowMarket`; `AltoLeverage`; `AdaptiveCurveIRM`; `FixedRateIRM`; `AssetShareConversionMath`. Oracle, router/`AuthUpgradeable`, and swap control flow are excluded.<br>Reviewed version: [`c965a0a4`](https://github.com/altomoney/v1/tree/c965a0a49000824f1fa93e5007c06e25a826bdfa) | [📄 View Report](./reports/Bailsec%20-%20ALTO%20-%20Lending%20Market%20-%20Final%20Report.pdf) |
| September 2025 | Enigma Dark | Rewards | `AltoReferralWhitelistAdapter`; `AltoRewardsDistributor`; `MerkleRootManager`; `rewardsDistributorClaimRewardTokens` in `AltoAdapter`<br>Reviewed version: [`9184b9df`](https://github.com/altomoney/v1/tree/9184b9df000e231b606161cf16be2cd08a723ccb) | [📄 View Report](./reports/2025-09_Managed_Security_Review_Alto_foundation.pdf) |
| July 2025 | Enigma Dark | Lending | Lending markets and related IRM, liquidation, math, authorization, adapter, and contract-upgradeability code<br>Reviewed version: [`cd400bfc`](https://github.com/altomoney/v1/tree/cd400bfc868a5880a0c0336086e13288f5e61083) | [📄 View Report](./reports/2025-07_Managed_Security_Review_Alto_foundation.pdf) |

## Security Providers

- **[Enigma Dark](https://www.enigmadark.com/)** — Managed security review program with continuous coverage
- **[Bailsec](https://bailsec.io/)** — Smart contract security audits
- **[Cantina](https://cantina.xyz/)** — Web3 security reviews


## Alto Bug Bounty Program

Starting on December 11th, 2025, the deployed contracts referencing the following Alto [smart-contract repository](https://github.com/altomoney/v1) are subject to the Alto Bug Bounty Program to incentivize responsible vulnerability disclosure.

### Scope

The scope of the Program is strictly limited to the following deployed [contracts](./deployments/mainnet.md).

The following are not within the scope of the Program:

- Bugs in any third-party contract or platform that merely integrates with Alto.
- Vulnerabilities already reported and/or discovered in contracts built by third parties on top of Alto.
- Any previously reported vulnerabilities.

### Public Disclosure of Known Issues

Bug reports covering previously-discovered bugs (listed below) are not eligible for a reward within this program. This includes known issues that the project is aware of but has consciously decided not to “fix”, necessary code changes, or any implemented operational mitigating procedures that can lessen potential risk.

### Vulnerability description

| **Severity**           | **Impact: High** | **Impact: Medium** | **Impact: Low** |
|------------------------|------------------|---------------------|------------------|
| **Likelihood: High**   | Critical         | High                | Medium           |
| **Likelihood: Medium** | High             | Medium              | Low              |
| **Likelihood: Low**    | Medium           | Low                 | Low              |


### Smart Contract Severity Rewards

| **Critical** | **High** | **Medium** | 
|--------------|----------|------------|
| **Max:** \$100,000  | **Max:** \$20,000  | **Flat:** \$3,000 | 
| **Min:** \$20,000    | **Min:** \$5,000  | —                  | 


### Reward Calculation for Critical Level Reports

For critical smart contract bugs, the reward amount is 10% of the funds directly affected up to a maximum of USD $100,000. The calculation of the amount of funds at risk is based on the time and date the bug report is submitted. However, a minimum reward of USD $20,000 is to be rewarded in order to incentivize security researchers against withholding a critical bug report.

### Reward Payment Terms

Payouts are handled by the Alto team directly and are denominated in USD. However, payments are done in USDC on Mainnet.

The calculation of the net amount rewarded is based on the average price of USDC between CoinMarketCap.com and CoinGecko.com at the time the bug report was submitted. No adjustments are made based on liquidity availability.


### Disclosure

**!!! DO NOT OPEN A PUBLIC GITHUB ISSUE !!!**

Any vulnerability or bug discovered must be reported to the following email: security@altofoundation.org

The vulnerability must not be disclosed publicly or to any other person, entity, or email address before the Alto team has been notified, has fixed the issue, and has granted permission for public disclosure.

A detailed report of a vulnerability increases the likelihood of a reward and may increase the reward amount. Please provide as much information about the vulnerability as possible, including:

- The conditions on which reproducing the bug is contingent
- The steps needed to reproduce the bug or, preferably, a proof of concept
- The potential implications of the vulnerability being abused
- Anyone who reports a unique, previously-unreported vulnerability that results in a change to the code or a configuration change and who keeps such vulnerability confidential until it has been resolved by our engineers will be recognized publicly for their contribution if they so choose.




---

<p align="center">
  <a href="https://altofoundation.org">Website</a> •
  <a href="https://docs.alto.money">Documentation</a> •
  <a href="https://x.com/alto_money">X</a>
</p>
