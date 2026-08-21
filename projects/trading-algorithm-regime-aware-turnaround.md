# Rebuilding confidence in an emerging-markets trading strategy

The $5 billion mandate lost $150 million in three months. The immediate responsibility was not to defend the model; it was to stop uncontrolled exposure, locate the loss, and define what evidence could earn capital back.

At D. E. Shaw, I designed and governed the recovery architecture across Quant Research, Trading, Risk, Compliance, Data Science, Engineering, Investor Relations, and the investment committee.

## Loss attribution came before model redesign

The original strategy had learned mainly from a decade in which mean reversion worked, then met persistent volatility, sanctions, elections, geopolitical shock, and thinner liquidity. Monthly review compressed everything into P&L.

I rebuilt the operating evidence from model decisions, market data, FIX fills, slippage, exposures, limit events, and dated macro events:

**investment loss = signal-selection error + sizing error + execution shortfall**

That decomposition assigned the correct owner. A sound signal executed badly needed a trading fix. A wrong-regime signal needed research. An acceptable idea with too much capital needed risk action.

## The adaptive layer could interpret; it could not authorize itself

The redesign classified regime, weighted mean-reversion/trend/capital-preservation specialists, and reduced exposure when confidence or liquidity deteriorated.

Capital, concentration, and drawdown limits stayed deterministic and outside the model. I required currency-crisis, sanctions, election, flash-crash, and liquidity-withdrawal stress plus rolling unseen windows.

The Basel Committee’s [2016 market-risk framework](https://www.bis.org/bcbs/publ/d352.pdf) was a relevant reference for expected shortfall, stressed behavior, and liquidity horizons; it did not define the investment mandate.

## Capital returned in tranches

I began with $500 million in Brazil and India rather than restoring the full mandate.

Weekly reviews joined return, Sharpe, drawdown, slippage, regime classification, concentration, liquidity, limits, and unexplained variance. A tranche advanced only if:

- signal behavior held in unseen data and live trading;
- execution stayed inside cost bounds;
- stressed loss and drawdown stayed within budget;
- every limit/override remained observable; and
- Investment, Risk, Compliance, Trading, and the portfolio owner accepted one record.

This reconciled competing needs: enough exposure for Investment to demonstrate recovery, a bounded failure for Risk/Compliance, stable requirements for Engineering, and accurate explanations for Investor Relations.

## Recovery record

| Capital decision | Failure baseline → release objective → result | Measurement |
|---|---|---|
| Stop/recover loss | -$150M over 3 months → recover under gated risk → recovered in 9 months | Official strategy P&L/capital ledger |
| Bound initial live authority | full mandate under pressure → limited proof → $500M Brazil/India pilot | Allocation ledger |
| Prove live economics | new design no live result → positive → 12% in 3 months | Pilot P&L / deployed capital |
| Improve risk-adjusted return | Sharpe 0.6 → improve → 1.2 | Team convention for return / volatility |
| Reduce implementation loss | slippage index 100 → reduce → 60 | FIX fills vs approved benchmark; -40% |
| Establish run-rate | none accepted → sustainable economics → estimated $40M annualized | Live result under approved annualization assumptions |
| Rebuild external confidence | no recovery-linked inflow → positive → $200M new AUM | Subscription records; communication contributed but was not sole cause |

The $40 million is explicitly an estimate, not booked annual profit. The $200 million inflow cannot be causally assigned to one intervention.

## The operating model outlasted the turnaround

Monthly retrospective review became continuous monitoring plus weekly cross-functional capital decisions. Investor Relations used the same regime/risk/recovery record translated for clients, so allocator questions exposed missing evidence rather than spawning a separate marketing narrative.

Loss decomposition, staged authority, shared telemetry, capital gates, committee decisions, and the interface to investor evidence were the responsibilities I carried. Quant teams controlled models; Trading execution; Risk/Compliance limits; Engineering systems; Investor Relations client dialogue.

The rule I retained: an adaptive model may interpret the regime, but it cannot decide how much institutional capital it is permitted to risk. Authority returns only when signal, execution, liquidity, and controls agree in unseen data and live trading.
