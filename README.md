# Target Labels Are Not Portfolio Returns

**Working Draft — June 2026**

This repository contains the current working-draft version of the research paper:

**Target Labels Are Not Portfolio Returns: A Triple-Barrier Failure Mode in Factor Investing**

Author: **Rodrigo Sucupira Andrade de Carvalho Lima**
Affiliation: **Independent Researcher, Brazil**

---

## Status

This is an intermediate working draft shared for professional and research discussion purposes.

The paper has **not yet been submitted to SSRN or to an academic journal**.
It is made available here as a research note for review, feedback, and discussion.

---

## Paper

The current PDF draft is available here:

[[Download the working draft](TargetLabelsAreNotPortfolioReturns.pdf)](https://github.com/rsucupira/Target_Labels/blob/main/TargetLabelsAreNotPortfolioReturns.pdf)

---

## Abstract

This paper studies a practical failure mode in financial machine learning: treating target-label prediction as sufficient evidence for portfolio performance.

Using a proprietary U.S. equity research panel and research artifacts from the FactorInvest environment, the study evaluates triple-barrier model labels in a factor-investing setting. The primary target, `TBM_LONG_FIX_21D_SL5_TP10`, defines a long event over a 21-trading-day horizon with a 5% stop-loss barrier and a 10% take-profit barrier.

The model produces a positive top-decile take-profit lift, but the same top decile shows negative event-return lift and a high stop-label share. When converted into a temporal-safe mark-to-market portfolio rule and compared with a high-liquidity equal-weight benchmark, the apparent label signal fails economically.

The contribution is a methodological case study rather than a new trading strategy. The central lesson is that triple-barrier labels should be bridged to explicit economic return contracts before being treated as investable signals.

**The model learned the label. It did not learn the trade.**

---

## Research Question

Can a financial machine learning model that successfully predicts triple-barrier target labels also generate economically meaningful portfolio performance?

This paper documents a negative case: label prediction improves, but portfolio performance does not.

---

## Key Takeaways

* Target-label prediction is not the same as portfolio-return prediction.
* A positive take-profit label lift can coexist with negative event-return lift.
* Ranking assets by predicted take-profit probability may select names with poor benchmark-relative performance.
* Triple-barrier labels require an explicit bridge to economic return contracts.
* Backtest governance matters: diagnostic repairs should not be promoted unless they pass validation before test interpretation.

---

## Scope and Disclaimer

This paper is an independent historical research study.

It is **not investment advice**, **not a live trading strategy**, and **not a production-ready portfolio model**.
The results are based on historical simulations using a proprietary U.S. equity research panel.

Reported returns are research returns and do not fully include all transaction costs, borrow costs, market impact, taxes, slippage, corporate actions, delisting treatment, capacity constraints, or other implementation frictions.

---

## Data and Code Availability

The underlying dataset is proprietary and is not included in this repository.

This repository currently provides only the working-draft paper.
No trading signals, production code, proprietary data, or implementation files are included.

---

## Suggested Citation

Sucupira Andrade de Carvalho Lima, Rodrigo.
*Target Labels Are Not Portfolio Returns: A Triple-Barrier Failure Mode in Factor Investing*.
Working Draft, June 2026.

---

## Keywords

Financial machine learning; triple-barrier labeling; factor investing; target engineering; backtesting; portfolio validation; label mismatch; research governance.

---

## JEL Codes

G11; G12; G17; C53; C58.

---

## Copyright

© 2026 Rodrigo Sucupira Andrade de Carvalho Lima. All rights reserved.

This working draft may be shared for professional review and research discussion. No part of this work may be reproduced, redistributed, or used for commercial purposes without prior written permission from the author.
