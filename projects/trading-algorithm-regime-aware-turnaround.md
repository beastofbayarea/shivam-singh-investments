# Rebuilding Confidence in an Emerging-Markets Trading Strategy

I led the recovery of an emerging-markets trading strategy. I had identified that the strategy was reacting badly to persistent changes in volatility, liquidity, and politics, while the team was reviewing the damage too slowly. I brought together Quant Research, Trading, Risk, Compliance, Data Science, Engineering, and Investor Relations.

The mandate managed $5 billion and had lost $150 million in three months. The immediate goal was not to defend the model. It was to find where value was being lost, stop uncontrolled exposure, and define what evidence the strategy would need to earn capital back.

## The first decision: treat the loss as more than a signal problem

The model had been trained largely on a decade in which mean reversion was a useful pattern. It then met a more persistent regime shaped by inflation, sanctions, elections, geopolitical shocks, and thinner liquidity. A monthly review combined every failure into one P&L number.

This was a capital-governance turnaround after a $150 million loss, not a model-tuning exercise. I owned the recovery architecture that determined when the strategy could trade, how much capital it could regain, which risks remained outside the model, and what evidence Risk, Trading, Compliance, investors, and the investment committee would all use to release the next tranche.

I replaced that view with trade-level attribution built from model decisions, market data, FIX execution logs, slippage, exposures, limit events, and a dated macro-event record. The analysis separated three possible losses:

`investment loss = signal selection error + position-sizing error + execution shortfall`

That separation mattered. A correct trade implemented badly needed an execution fix; a well-executed trade in the wrong regime needed a research fix; an acceptable signal with excessive capital needed a risk-control fix. One blended number could not assign the right owner.

## I changed the model, but kept authority outside it

The redesign combined regime classification, ensemble selection, and adaptive exposure. Instead of forcing one model to explain every market, the system identified the current conditions, weighted the models suited to them, and reduced exposure when classification confidence or liquidity deteriorated.

The model was not allowed to set its own capital, concentration, or drawdown limits. Those remained deterministic controls owned by the investment and risk process. I stress-tested currency crises, sanctions, elections, flash crashes, and sudden liquidity withdrawal, and I used rolling out-of-sample windows so the redesign could not pass by fitting only the failure period.

The Basel Committee's 2016 market-risk framework was a relevant contemporaneous reference for expected shortfall, stressed behavior, and risk-factor liquidity horizons. It did not define the investment mandate, but it reinforced the need to assess tail loss and the time required to exit risk—not only ordinary-period volatility.

## Capital came back through evidence, not argument

I started with a $500 million pilot in Brazil and India rather than restoring the full mandate. Every weekly decision reviewed return, Sharpe ratio, drawdown, execution shortfall, regime classification, concentration, liquidity, limit behavior, and unexplained variance.

A capital tranche could advance only if:

- the signal held in unseen data and the live pilot;
- realized execution remained inside the cost boundary;
- stressed loss and drawdown stayed within the agreed risk budget;
- every limit and override was observable; and
- Risk, Compliance, Trading, and the portfolio owner read the same evidence.

That structure resolved a central stakeholder conflict. The investment team wanted enough exposure to demonstrate recovery; Risk and Compliance needed a bounded failure; Engineering needed a stable specification; and Investor Relations needed an accurate explanation without proprietary code. A staged pilot served all four needs.

## Recovery ledger

| Measure | Failure baseline | Release objective | Result | Measurement |
|---|---:|---:|---:|---|
| Strategy loss | $150M over 3 months | Stop the drawdown and recover the loss under gated risk | Loss recovered within 9 months | Official strategy P&L and capital records |
| Pilot capital | Full mandate under pressure | Limit first live exposure | $500M in Brazil and India | Capital-allocation ledger |
| Pilot return | New design had no live result | Demonstrate positive live economics | 12% within 3 months | Pilot P&L divided by deployed capital |
| Sharpe ratio | 0.6 | Improve risk-adjusted return; no retained numeric target | 1.2 | Period return divided by return volatility using the team's reporting convention |
| Execution slippage | Pre-redesign level indexed to 100 | Reduce implementation loss | Index of 60, a 40% reduction | FIX fills compared with the team's execution benchmark |
| Annualized profit contribution | No accepted run-rate from the redesign | Establish sustainable economics | Estimated $40M | Live result annualized under the approved base assumptions |
| New assets under management | No recovery-linked inflow | Rebuild allocator confidence | $200M | Mandate subscription records; supported by, but not solely attributed to, recovery communication |

## The operating change was as important as the algorithm

I moved the team from monthly retrospective review to continuous monitoring and weekly cross-functional decisions during the pilot. Investor Relations used the same regime, risk, and recovery record as the technical teams, translated for clients. Questions from allocators therefore exposed missing evidence instead of being answered with a separate marketing story.

I can defend the measured P&L, slippage, Sharpe, and capital figures as program results. The $40 million figure is explicitly an annualized estimate, and the $200 million inflow cannot be assigned to one intervention alone. The stronger causal claim is operational: staged authority, shared telemetry, and explicit stop conditions shortened the distance between a market change and a capital decision.

## The rule I kept

An adaptive model may decide how to interpret a regime; it may not decide how much institutional capital it is allowed to risk. I return authority only after signal, execution, liquidity, and control behavior agree in unseen data and live trading.

### Technical references

1. [Basel Committee, Minimum capital requirements for market risk (2016)](https://www.bis.org/bcbs/publ/d352.pdf) — contemporaneous reference for expected shortfall, stress, and liquidity horizons.
2. [Basel Committee, consolidated market-risk standard (2019)](https://www.bis.org/bcbs/publ/d457.htm) — later revision used to confirm the continuing treatment of expected shortfall, modellability, and trading-desk evidence.
3. [Tashman, “Out-of-sample tests of forecasting accuracy” (2000)](https://doi.org/10.1016/S0169-2070(00)00065-0) — rolling-origin validation method.
4. [Kissell and Glantz, transaction-cost and best-execution framework (2003)](https://doi.org/10.1016/S1544-6123(03)01004-7) — separates ex-post slippage measurement from ex-ante transaction-cost estimation.
5. [Role chronology](https://github.com/beastofbayarea/shivam-singh-investments/blob/main/shivam-singh-investments.pdf) — establishes my D. E. Shaw work period from July 2016 to December 2019.
