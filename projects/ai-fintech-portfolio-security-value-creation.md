# Turning Shared AI FinTech Security Risk into Portfolio Value

I led this portfolio value-creation work during my [AWS experience beginning in July 2024](https://github.com/beastofbayarea/shivam-singh-investments/blob/main/shivam-singh-investments.pdf).

Across several AI FinTech companies, different incidents pointed to one investment constraint: enterprise adoption was moving faster than the companies' security and compliance systems. The risks included public-model data leakage, biased credit behavior, deepfake onboarding, and unprotected data in use.

I translated those recurring risks into a shared operating thesis. Security work would be prioritized not only by technical severity, but by its effect on bank-buyer confidence, compliance readiness, insurance cost, retention, and valuation risk.

## I created a common control plane with company-level gates

NIST's Cybersecurity Framework 2.0 supplied the primary portfolio structure. I used its govern, identify, protect, detect, respond, and recover functions to define outcomes while allowing each company to implement controls appropriate to its architecture.

The shared pattern combined identity and access management, verified access, fairness tests, model guardrails, deepfake detection, key management, protected execution, code scanning, Security Hub, and automated audit evidence. NIST's Generative AI Profile added the model-specific frame around confabulation, privacy, information integrity, cybersecurity, bias, and human oversight.

Each remediation had an investment gate, accountable operator, production proof, and a business measure. A slide showing a planned control did not reduce portfolio risk.

## A failed privacy path sharpened the decision model

One company initially chose fully homomorphic encryption. The protection was strong in theory, but the implementation produced 14-second latency against a sub-300-millisecond adoption requirement.

I ran two technical paths in parallel and used the predefined performance threshold to stop the losing option. The replacement used Nitro Enclaves and delivered approximately 200–220 milliseconds. The decision did not abandon privacy; it chose a control that protected data in use while allowing the customer workflow to function.

That episode became a portfolio rule: the strongest isolated control is not automatically the lowest-risk product choice. If it makes the service unusable, customers will avoid the product or teams will route around the control.

## Proof and ownership made the standard durable

I introduced a 72-hour production-proof rule for material remediations. Evidence had to show that the control was deployed, observable, and behaving as intended. Automated evidence reduced recurring manual preparation, while an internal security champion at each company owned the operating standard after the central program moved on.

I reported progress in two connected views:

- technical and governance evidence, such as control coverage, findings, response ownership, and audited Security Hub scores; and
- portfolio value, such as enterprise readiness, sales friction, insurance premium, retention, and adoption economics.

## What changed across the portfolio

- No breaches were recorded during the program period.
- Compliance readiness fell from nine months to three.
- Cyber-insurance premiums declined 40%.
- Audited companies maintained Security Hub scores above 95.
- Reported AI return on investment increased from 4%–5% to 10%–12%.
- Customer retention improved 18%.

## The investment lesson

Cybersecurity becomes a value-creation program when technical evidence is connected to the buyer's decision and a long-term operator owns the control. I use common standards to accelerate the repeatable work, but I retain explicit product and architecture gates so a portfolio company does not implement security theater—or a technically pure system nobody can adopt.

## External foundations

These sources supplied the primary cybersecurity and generative-AI risk methodology. My resume is linked only to establish employment chronology.

| Source | How I applied it |
|---|---|
| [NIST — Cybersecurity Framework 2.0 (2024)](https://doi.org/10.6028/NIST.CSWP.29) | I used its outcome-based functions to create a common portfolio control and ownership structure. |
| [NIST — Generative AI Profile (2024)](https://doi.org/10.6028/NIST.AI.600-1) | I used its model-specific risks and measurement guidance for leakage, bias, integrity, oversight, and production proof. |
