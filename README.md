# Alto Security Review Engagements

This repository contains all available security audit reports for Alto protocol smart contracts and infrastructure.

## About Alto's Security Program

Security is a top priority at Alto. We engage with leading security firms to conduct thorough audits of our codebase. All findings are addressed before deployment, and completed reports are published here for transparency.

## Completed Audits

| Date | Provider | Scope | Report |
|:-----|:---------|:------|:-------|
| April 2026 | Cantina | Vault code upgrade | [PENDING]() |
| February 2026 | Cantina | Liquidation Mechanism | [📄 View Report](./reports/report-cli-cantina-altomoney-0114.pdf) |
| December 2025 | Cantina | Oracles & Miscellaneous | [📄 View Report](./reports/report-cantinacode-alto-money-solo-1204.pdf) |
| November 2025 | Cantina | PSM | [📄 View Report](./reports/report-cantinacode-alto-money-1124.pdf) |
| November 2025 | Bailsec | Staking & Rewards | [📄 View Report](./reports/Bailsec%20-%20ALTO%20-%20Staking%20Rewards%20-%20Final%20Report.pdf) |
| November 2025 | Enigma Dark | Oracles & Miscellaneous, Staking | [📄 View Report](./reports/2025-11_Managed_Security_Review_Alto_foundation.pdf) |
| November 2025 | Bailsec | Lending Market | [📄 View Report](./reports/Bailsec%20-%20ALTO%20-%20Lending%20Market%20-%20Final%20Report.pdf) |
| September 2025 | Enigma Dark | Rewards | [📄 View Report](./reports/2025-09_Managed_Security_Review_Alto_foundation.pdf) |
| July 2025 | Enigma Dark | Lending | [📄 View Report](./reports/2025-07_Managed_Security_Review_Alto_foundation.pdf) |

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