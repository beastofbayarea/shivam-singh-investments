# Finding investable pricing power inside a retail portfolio

## Underwriting conclusion

I identified a modeled $50 million revenue opportunity and reduced the decision cycle from six weeks to under one. The $50 million was neither booked revenue nor a company-wide pricing-power claim. It was the sum of segment-level opportunities whose customer behavior, competitive boundary, downside, owner, and rollout gate were explicit.

At McKinsey, I led this analysis across merchants, pricing/analytics, finance, client executives, and investment decision-makers. The task was to show where pricing power existed, where volume would migrate, and which value deserved no credit until a live test.

## Portfolio averages were economically useless

Customers encounter a product, channel, promotion, competitor, and alternative—not an average elasticity.

I segmented the portfolio by customer mission, product role, channel behavior, competitive visibility, and observed substitution:

- visible products that anchor price perception;
- differentiated products with defensible room;
- traffic/basket anchors whose direct increase could damage other sales;
- substitutable products where competitors set the ceiling.

Only segments with a reason to retain demand entered the value case. This converted “pricing sophistication” into a location-specific investment thesis.

Contemporaneous McKinsey work on [pricing fashion with science](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/pricing-fashion-with-science) and [the pricing renaissance](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights/the-pricing-renaissance-new-ways-to-reduce-risk-and-unlock-value) supplied market context around granular response, switching, transparency, and execution risk.

## Causal evidence remained a range

Historical price, promotion, seasonality, assortment, stock, and competitor action moved together. I used regression to estimate demand response and difference-in-differences to compare treated and comparison change.

Four safeguards mattered:

1. inspect pre-treatment paths for the parallel-trends requirement;
2. isolate stockouts, promotions, assortment changes, and shocks;
3. test alternative timing, segment, and competitor-response assumptions;
4. retain a downside range instead of a preferred point estimate.

The World Bank’s discussion of [difference-in-differences assumptions](https://blogs.worldbank.org/en/impactevaluations/often-unspoken-assumptions-behind-difference-difference-estimator-practice) informed the counterfactual discipline.

Later research found that observational scanner-price variation can fail to reproduce experimental elasticities even under DiD. That paper postdates the work and did not guide it, but it correctly limits the current claim: stronger observational identification is not the same as random assignment.

## Hindcasting was admission, not decoration

I ran the method across earlier decision windows, estimating on prior data and testing withheld outcomes. This rolling out-of-sample design checked temporal portability instead of in-sample explanation.

Key operating assumptions in the broader diligence reached roughly 95% hindcast accuracy. Forecast error remained in the downside. The [Tashman paper on out-of-sample testing](https://doi.org/10.1016/S0169-2070(00)00065-0) supports this rolling evaluation logic.

A model could pass hindcast and still fail under a competitor move, implementation error, or customer response outside historical range. The gate bounded uncertainty; it did not remove it.

## The investment memo linked evidence to capital

For each lever, the committee saw:

**segment → evidence → elasticity range → proposed move → volume downside → competitor/substitution sensitivity → owner → stop signal**

That artifact allowed merchants to challenge commercial logic, analysts to challenge identification, finance to reconcile the bridge, and executives to choose how much uncertainty to fund. Faster analysis did not mean weaker governance.

## Decision record

| Investment measure | Baseline → target → result | Method |
|---|---|---|
| Cycle time | 6 weeks → <1 week → <1 week | Scoped question to decision-ready memo; >83.3% lower |
| Modeled opportunity | no portfolio value → evidence-backed/downside-visible → $50M | Segment-level modeled revenue under base assumptions |
| Out-of-sample behavior | no common gate → decision-useful → ~95% on key broader-diligence assumptions | Forecast vs withheld historical outcomes |
| Realized revenue | absent → staged rollout measurement → not retained/not claimed | Transaction results with matched counterfactuals |

I owned segmentation, causal design, hindcast gate, downside model, value bridge, operating-owner map, and committee narrative. Merchants owned category decisions; analytics owned estimation; finance owned realization; executives owned capital.

The investment contribution was not a better dashboard. I made pricing power locatable, challengeable, and stoppable—strong enough to influence valuation without pretending a modeled opportunity had already been earned.
