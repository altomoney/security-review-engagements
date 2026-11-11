# Acknowledgements

Alto thanks the people below for responsibly disclosing issues through the [bug bounty program](./README.md#alto-bug-bounty-program). Each reporter chose to be credited.

| Reported | Reported by | Severity | Finding | Resolution |
|:---------|:------------|:---------|:--------|:-----------|
| September 2026 | Akira Nakao ([everforyou](https://github.com/everforyou)) | Low | `AltoVault.maxDeposit` could quote more than `deposit` accepts when a queued market has its own supply cap | Mitigated on mainnet by configuration. The source fix is [pending](https://github.com/altomoney/v1/blob/dev/PENDING.md#pending-fixes) and ships with the next vault deployment. |
