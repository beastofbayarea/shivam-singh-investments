# Trading Algorithm Recovery - Regime-Aware Turnaround

> **Document type:** Externally grounded interview case reconstruction, not a claim of an independently verified completed engagement.
>
> **Timeline alignment:** The [public Investment and Portfolio Strategy resume](https://github.com/beastofbayarea/shivam-singh-investments/blob/main/shivam-singh-investments.pdf) is used only to place this case within the D. E. Shaw role dated July 2016-December 2019.

## Evidence-grounded premise

Tashman's research warns that model utility should be evaluated out of sample across rolling origins and multiple periods. The Basel Committee's 2016 market-risk framework emphasizes expected shortfall under stress and liquidity horizons. Together they support diagnosing algorithm performance by regime, cost, liquidity, and tail risk rather than aggregate backtest return.

## Case approach

- Rebuild data lineage and evaluate signals over rolling periods that include distinct market regimes.
- Include transaction cost, liquidity, capacity, delay, and model-change assumptions.
- Compare expected and realized behavior under stress and define conditions for de-risking or shutdown.
- Reintroduce exposure through controlled capital gates with independent risk review.

## Evidence-based success measures

Use out-of-sample stability, stress loss, turnover cost, liquidity consumption, forecast degradation, limit breaches, and rollback effectiveness. These are proposed measures, not historical results.

## External source map

| Source | Contribution |
|---|---|
| [Tashman - Out-of-sample tests of forecasting accuracy (2000)](https://www.sciencedirect.com/science/article/pii/S0169207000000650) | Primary rolling out-of-sample validation methodology. |
| [Basel Committee - Revised market-risk framework (2016)](https://www.bis.org/press/p160114.htm) | Primary stress, expected-shortfall, and liquidity-horizon context. |
| [Public resume](https://github.com/beastofbayarea/shivam-singh-investments/blob/main/shivam-singh-investments.pdf) | Work dates only. |
