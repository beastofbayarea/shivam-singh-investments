# Earning Capital Back for a Regime-Aware Trading Strategy

I took ownership of this recovery during my [D. E. Shaw experience from July 2016 to December 2019](https://github.com/beastofbayarea/shivam-singh-investments/blob/main/shivam-singh-investments.pdf).

A $5 billion emerging-markets strategy lost $150 million over three months. The model had learned from a decade dominated by mean reversion, then encountered a persistent volatility and liquidity regime shaped by inflation, sanctions, elections, and geopolitical shocks. Monthly reviews and functional silos allowed the mismatch to compound.

I treated the decline as a system failure across signal, execution, risk, monitoring, and decision cadence—not as an unlucky quarter.

## I separated signal loss from execution loss

I formed one crisis team across Quant Research, Trading, Risk, Compliance, Data Science, Engineering, and Investor Relations. We rebuilt trade-level performance from FIX logs, market data, slippage, macro events, and model decisions.

The attribution separated two questions. Did the signal select the wrong exposure for the observed regime? Did execution lose value while implementing an otherwise valid position? Combining them in one P&L number would have hidden the remedy.

## The redesign recognized regime uncertainty

I replaced one static model choice with regime classification, ensemble selection, and adaptive exposure. The strategy could change how it interpreted conditions, but it remained inside deterministic capital, concentration, and drawdown limits.

The Basel Committee's 2016 market-risk framework provided contemporaneous context for expected shortfall, stress, and liquidity horizons. I used those concepts to make tail behavior and liquidity deterioration explicit in the release gates.

I stress-tested currency crises, flash crashes, sanctions, elections, and sudden liquidity withdrawal. Tashman's work on rolling out-of-sample evaluation influenced the validation design: performance had to hold across unseen windows rather than only fit the period that had already failed.

## Capital returned in tranches

The redesigned strategy did not regain authority through a presentation. I deployed it first to Brazil and India with a $500 million gated pilot. Weekly reviews covered return, Sharpe ratio, drawdown, slippage, regime classification, limit behavior, and unexplained variance.

Each capital tranche required evidence that both investment behavior and the operating controls remained inside the agreed boundary. If results diverged, the team could pause at a known exposure instead of discovering a problem after restoring the full fund.

## What the recovery produced

- Pilot return on investment improved 12% within three months.
- Execution slippage declined 40%.
- Sharpe ratio improved from 0.6 to 1.2.
- The $150 million loss was recovered within nine months.
- The strategy added an estimated $40 million in annualized profit.
- Transparent recovery evidence supported $200 million in new assets under management.

## The organizational change outlasted the model

I replaced monthly retrospective review with 24/7 monitoring, weekly cross-functional decisions during the pilot, and a reusable escalation playbook. Investor Relations received the same evidence model used by the technical and investment teams, translated for the client audience without exposing proprietary code.

## My investment rule after the turnaround

Adaptive models still need non-negotiable boundaries. I let the system learn how to respond to a changing regime, but I do not let it learn how much capital it may risk. Authority is earned through out-of-sample behavior, stressed execution, observable limits, and staged exposure.

## External foundations

These sources supplied the primary forecast-validation and market-risk methodology. My resume is linked only for employment chronology.

| Source | How I applied it |
|---|---|
| [Tashman — Out-of-sample tests of forecasting accuracy (2000)](https://www.sciencedirect.com/science/article/pii/S0169207000000650) | I used its rolling out-of-sample principles to avoid validating the redesign only on the known failure period. |
| [Basel Committee — Revised market-risk framework (2016)](https://www.bis.org/press/p160114.htm) | I used its expected-shortfall, stress, and liquidity-horizon context for risk gates and tranche decisions. |
