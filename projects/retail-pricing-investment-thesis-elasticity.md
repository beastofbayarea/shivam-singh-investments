# Finding Investable Pricing Power Inside a Retail Portfolio

I led the pricing analysis for a retail investment decision. I had identified that the retailer needed to know which customers would accept a price change, where they would switch, and whether the opportunity could survive real competition. I worked with merchants, pricing and analytics teams, finance leaders, client executives, and the investment decision makers.

## The conclusion, stated narrowly

I identified a modeled $50 million revenue opportunity and reduced the analytical cycle from six weeks to less than one. The $50 million was an evidence-weighted opportunity under stated assumptions—not booked revenue, profit, or a promise that every recommended change would be implemented.

The work was an investment-underwriting intervention, not a pricing dashboard. I translated millions of observed customer and competitor decisions into segment-level elasticity, downside cases, rollout gates, and a capital-allocation view that showed where pricing power was defensible, where volume would migrate, and where the committee should assign no value until a live test proved it.

That distinction shaped the work. The investment committee needed to know which value was observed, which was estimated, which depended on execution, and what result would invalidate the thesis.

## Why one elasticity number would have been wrong

Customers did not experience a portfolio average. They saw a product, a price, a channel, a promotion, and an alternative at a particular moment. Contemporaneous McKinsey research on retail pricing reinforced the need to account for price perception, segment, channel transparency, competitor response, and switching.

I divided the portfolio by customer mission, product role, channel behavior, competitive visibility, and observed substitution. That produced economically different groups:

- visible products that shaped the retailer's overall price image;
- differentiated products with room to move;
- traffic or basket anchors where a price increase could damage other sales; and
- highly substitutable products where the competitor, not the model, set the boundary.

The thesis valued pricing power only where the retailer had a defensible reason for it.

## How I tried to identify cause rather than coincidence

Historical sales alone could not tell me what a new price would do. Price, promotion, seasonality, assortment, stock availability, and competitor action moved together. I used regression to estimate demand response, then difference-in-differences to compare changes in treated and comparison groups.

The design had four safeguards:

1. I checked whether treatment and comparison groups followed similar paths before the change—the parallel-trends requirement.
2. I excluded or separately modeled periods distorted by stock-outs, major promotions, assortment changes, and unusual events.
3. I tested sensitivity to treatment timing, segment definition, and competitor response.
4. I retained a downside range instead of turning one preferred coefficient into a point forecast.

A later retail field study found that observational scanner-price variation did not reproduce experimental elasticities, including in a difference-in-differences design. That research post-dates this project, so it did not guide the original work. It does sharpen how I describe the result now: the design improved causal credibility, but it did not make non-randomized pricing evidence equivalent to a controlled experiment.

## Hindcasting was the model's admission test

I ran the model over earlier decision windows and compared its forecasts with outcomes that were already known but withheld from estimation. This rolling out-of-sample approach tested whether the method traveled across time rather than merely explaining the sample used to build it.

Across the broader diligence work, key operating assumptions reached approximately 95% hindcast accuracy. I kept forecast error in the downside case. A good historical fit increased confidence in the range; it did not remove implementation, competitive, or customer risk.

## The investment memo was built as a bridge from evidence to action

For each pricing lever, the committee saw:

- the customer and product segment;
- the observed evidence and estimated elasticity range;
- the proposed move and implementation sequence;
- expected revenue effect and volume downside;
- competitor and substitution sensitivity;
- operational owner; and
- a stop or rollback signal.

Merchants could challenge commercial assumptions, analytics could challenge identification, finance could reconcile the value bridge, and executives could choose how much uncertainty to fund. That shared artifact also prevented the faster analytical cycle from becoming a less governed cycle.

## Measurement record

| Decision measure | Baseline | Target | Result | How it was measured |
|---|---:|---:|---:|---|
| Analytical cycle time | 6 weeks | Under 1 week | Under 1 week | Calendar time from scoped question to decision-ready analysis |
| Modeled revenue opportunity | No quantified portfolio opportunity | Identify evidence-backed value with downside visible | $50 million | Sum of segment-level modeled revenue effects under the base assumptions |
| Out-of-sample performance | No common hindcast gate | Decision-useful historical performance; no numeric target retained | About 95% on key operating assumptions across the broader diligence | Forecast-to-actual comparison on withheld historical windows |
| Realized revenue | Not established in the retained record | Measure during staged rollout | Not claimed | Would require transaction-level rollout results and matched counterfactuals |

## What I would say if challenged

The strongest claim is that I made pricing power investable: granular enough to locate, tested enough to bound, fast enough to use, and explicit enough to stop. The work did not prove a company-wide trait and did not convert a modeled opportunity into realized revenue. Its value was a decision system that showed where evidence ended and execution began.

### Method and market sources

- [McKinsey, “Pricing fashion with science” (2014)](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/pricing-fashion-with-science) — contemporaneous link between granular elasticity and retail price decisions.
- [McKinsey, “The pricing renaissance” (2015)](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/the-pricing-renaissance-new-ways-to-reduce-risk-and-unlock-value) — contemporaneous treatment of switching, segment response, transparency, and risk.
- [World Bank, assumptions behind difference-in-differences (2013)](https://blogs.worldbank.org/en/impactevaluations/often-unspoken-assumptions-behind-difference-difference-estimator-practice) — parallel-trends and counterfactual discipline.
- [Tashman, “Out-of-sample tests of forecasting accuracy” (2000)](https://doi.org/10.1016/S0169-2070(00)00065-0) — rolling-origin and out-of-sample forecast evaluation.
- [Bray, Sanders, and Stamatopoulos, “Observational Price Variation in Scanner Data Does Not Reproduce Experimental Price Elasticities”](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4899765) — later evidence used only to qualify the causal limits of observational pricing work.
- [Role chronology](https://github.com/beastofbayarea/shivam-singh-investments/blob/main/shivam-singh-investments.pdf) — establishes my McKinsey work period from July 2014 to June 2016.
