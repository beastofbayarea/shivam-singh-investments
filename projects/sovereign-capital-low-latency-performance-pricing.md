# Sovereign Capital Trading — Low-Latency Execution & Performance Pricing

> **Portfolio lens:** Institutional mandate strategy, investment infrastructure, downside alignment, allocator trust, and performance-linked economics.

## Executive snapshot

Connected a deterministic low-latency trading architecture to a sovereign investor's need for controlled downside and aligned fees. Stress replay, shadow mode, firm-capital proof, hardware risk gates, and hurdle-based pricing made the technical moat governable and commercially credible.

## Resume-ready impact

- Sponsored a GPU/RDMA execution redesign that held 35 microsecond median and 40 microsecond p99 latency under a severe market shock.
- Validated the platform through historical replay, six-week shadow mode, and $50M of firm capital before exposing client assets.
- Helped secure a $500M mandate with 1-and-30 pricing above a hard hurdle; the strategy produced an 18% net first-year return and $25M in performance fees.

## Interview story

### Situation

A sovereign investor needed protection against concentrated macro risk but distrusted fixed fees and opaque managers. The existing CPU architecture showed eight-millisecond tail spikes precisely when liquidity deteriorated.

### Task

Prove that infrastructure, controls, and commercial terms could make the same promise: the manager would earn upside only when execution protected and compounded client capital.

### Actions

- Selected a deterministic GPU design based on stressed tail latency rather than average speed.
- Used GPUDirect RDMA, persistent kernels, an independent FPGA risk gate, heartbeat controls, and CPU fallback.
- Progressed through crash replay, shadow comparison, firm capital, and live-event proof.
- Structured a 1% base fee and 30% incentive fee only above the risk-free rate plus a 4% hurdle.

### Results

- The engine completed 94% of intended hedges with less than 0.5 basis points of slippage during the cited event.
- The portfolio experienced no drawdown during the event.
- The investor approved a $500M allocation.
- First-year net return reached 18%, generating $25M in performance fees.

## Decisions and trade-offs

- Optimize tail-latency determinism, not benchmark averages.
- Risk firm capital before asking the client to trust the new system.
- Make the fee contract part of the investment product and its downside alignment.

## Leadership signal

Translated engineering evidence for investment committees, quants, infrastructure leaders, boards, and sovereign allocators without reducing the decision to a hardware benchmark.

## Skills and keywords

institutional investing · sovereign wealth · low-latency trading · performance fees · mandate origination · allocator relations · risk controls · shadow testing · investment infrastructure · fee alignment

## Source

[Original Notion project page](https://app.notion.com/p/2f6f9e255f2180cfb46fcc435e8a0573)

