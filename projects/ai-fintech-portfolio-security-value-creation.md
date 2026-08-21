# Making AI FinTech Safe Enough for Bank Adoption

I led a security value-creation project for a group of AI FinTech companies. I had identified that bank buyers were being asked to trust products that handled sensitive data and decisions before the companies could show consistent safeguards. I worked across founders, product and security leaders, compliance teams, bank customers, insurers, and the investment team.

The investment problem was larger than preventing an incident. Weak security evidence was slowing enterprise sales, extending compliance work, raising insurance cost, and leaving portfolio value exposed to a single avoidable failure. I therefore treated security as an operating and commercial system rather than a collection of technical fixes.

## The portfolio thesis I put into operation

I created a common risk language, then refused to force every company into the same architecture. NIST Cybersecurity Framework 2.0 gave the portfolio six outcome areas—govern, identify, protect, detect, respond, and recover. NIST's Generative AI Profile added the risks that ordinary cloud controls did not cover well: sensitive-data disclosure, fabricated output, harmful bias, information integrity, model misuse, and unclear human responsibility.

For each company, I connected four questions:

| Investment question | Product question | Proof required | Business decision affected |
|---|---|---|---|
| What loss could change the value of the company? | Where could data, identity, a model, or an operator fail? | Deployed control, live telemetry, named owner, and recovery evidence | Invest, remediate, insure, sell, or stop |
| What would a regulated buyer challenge? | Can the team explain access, data use, model behavior, and escalation? | Buyer-ready control record and test result | Enterprise launch readiness |
| Which control could damage the product? | Does privacy or review make the service too slow or unusable? | Security and customer-performance test on the same path | Architecture choice |
| What must remain after the central project ends? | Who owns alerts, exceptions, evidence, and retesting? | Company-level operator and recurring review | Durability of the value plan |

This turned a broad security agenda into company-specific gates. Identity and access management, model guardrails, fairness tests, deepfake detection, key management, protected execution, code scanning, Security Hub, and automated audit evidence were used only where they addressed an explicit failure path.

## The privacy design that failed—and the decision it improved

At one company, fully homomorphic encryption offered strong protection for data in use but produced a 14-second response. The customer experience needed to remain below 300 milliseconds. I kept two technical paths alive until comparable timing evidence made the choice clear, then stopped the slower path.

The selected design used AWS Nitro Enclaves and delivered approximately 200–220 milliseconds. Nitro Enclaves isolate memory and processing from the parent instance, remove ordinary interactive access and external networking, and use signed attestation measurements to let AWS KMS release keys only to approved code. That made the decision technically stronger than simply saying “confidential computing”: the access policy could be tied to measured enclave code.

The lesson was not that one privacy technology is universally better. It was that the lowest-risk product is the one that satisfies the threat model and the customer task together. A theoretically stronger safeguard that users route around is not an effective control.

## I made remediation observable and transferable

Every material fix received an accountable operator, a release gate, a commercial measure, and a 72-hour production-proof requirement. A completed ticket or presentation was not evidence. The company had to show that the control was deployed, visible in monitoring, and behaving as intended in the live environment.

I paired the shared portfolio standard with a security champion inside each company. The central team could supply patterns and escalation, but the company operator owned exceptions, evidence refresh, incident response, and the next audit. This resolved the competing priorities between shipping, buyer diligence, and remediation: the same proof served engineering, compliance, insurance, and sales instead of creating four reporting systems.

## Results, thresholds, and how I read them

| Measure | Baseline | Target or decision rule | Observed result | Measurement method |
|---|---:|---:|---:|---|
| Protected-compute response | 14 seconds | Below 300 ms | About 200–220 ms | Like-for-like application timing on the two privacy paths |
| Compliance readiness cycle | 9 months | Shorten materially; no separate numeric target was retained | 3 months | Elapsed time from gap assessment to audit-ready control evidence |
| Audited Security Hub posture | Not retained | Above 95 | Above 95 | Audited Security Hub score for participating companies |
| Cyber-insurance premium | Pre-program premium indexed to 100 | Reduce without weakening coverage | Index of 60, a 40% decline | Renewal premium comparison |
| Reported AI return on investment | 4%–5% | Improve after adoption blockers were removed | 10%–12% | Portfolio-company reporting before and after the program |
| Customer retention | Pre-program cohort indexed to 100 | Improve | Index of 118 | Company retention reporting over the program period |

No breaches were recorded during the program period. I do not treat that as proof that the program “prevented” a breach, and I do not claim security alone caused the retention or return improvements. The defensible conclusion is that control evidence, compliance speed, insurance economics, adoption, and retention improved together while the portfolio introduced the operating system described here.

## What I would defend in an investment committee

The work increased value because it made previously hidden risk governable. It gave the investment team comparable evidence across companies, gave operators architecture-level choices, and gave bank buyers proof they could inspect. The portable asset was not a checklist; it was a way to connect a material loss scenario to a usable product control, production evidence, a responsible owner, and an economic consequence.

### Research record

- [NIST Cybersecurity Framework 2.0 (2024)](https://doi.org/10.6028/NIST.CSWP.29) — outcome-based structure for portfolio governance and control ownership.
- [NIST AI RMF: Generative Artificial Intelligence Profile (2024)](https://doi.org/10.6028/NIST.AI.600-1) — model-specific risk, measurement, and human-oversight frame.
- [AWS Nitro Enclaves documentation](https://docs.aws.amazon.com/enclaves/latest/user/) — isolation properties and operating constraints of the selected confidential-compute path.
- [AWS Nitro Enclaves cryptographic attestation](https://docs.aws.amazon.com/enclaves/latest/user/set-up-attestation.html) — signed measurements and KMS authorization design.
- [Role chronology](https://github.com/beastofbayarea/shivam-singh-investments/blob/main/shivam-singh-investments.pdf) — establishes my AWS work period beginning in July 2024; it is not used as evidence for external technical claims.
