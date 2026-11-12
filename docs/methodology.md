# Methodology

The audit gives a **directional** yearly cost of inaction. It is not a forecast.

## Baseline

```
deals per year   = leads/month × 12 × lead→customer %
revenue per year = deals per year × average deal value
not converted    = leads/month × 12 × (1 − lead→customer %)
```

## Leak formulas

| Leak | Formula | Default |
|---|---|---|
| `sla` No 24-hour reply | revenue × p | p = 15% |
| `disc` Demo before discovery | revenue × p | p = 10% |
| `nurt` "Not now" not nurtured | not converted × share × win × deal value | share = 30%, win = 5% |
| `cov` Sellers prospecting | reps × hours/week × 46 weeks × hourly cost | 4 × 8 × $75 |
| `loop`, `metric`, `proof` | score only, no dollar value | |

Leaks are **added**, not compounded. That keeps the total conservative.

## Alignment score

`100 − weights of ticked leaks`. Weights: `sla` 20, `disc` 15, `nurt` 15, `loop` 15, `metric` 15, `cov` 10, `proof` 10.

| Score | Grade |
|---|---|
| 80–100 | Aligned engine |
| 60–79 | Leaky pipeline |
| 40–59 | Siloed teams |
| 0–39 | Two companies under one logo |

## Sources (checked against the books)

| Claim | Source |
|---|---|
| 24-hour response raised conversion to sale 7–10×; 22% of inquiries never answered; average 58 days | John Coe, *The Fundamentals of Business-to-Business Sales & Marketing* (McGraw-Hill, 2003), citing Performark |
| 30–50% of B2B inquiries buy within 12–18 months | Coe (2003) |
| Inquiries: 10–20% ready now, 20–30% evaluating, 30–40% starting, 10–20% unqualified | Coe (2003) |
| A field sales call costs $300–400 (Cahners: $329) | Coe (2003) |
| Demos without discovery are 73% less successful; demos tied to pain are 35% more likely to win | Cognism, *The B2B Sales Process Handbook* (2021), citing Sales Benchmark Index |
| "Easyboy & Hardfellow"; the Pre-Approach; Demonstration; Closing | W. W. Atkinson, *The Psychology of Salesmanship* (1912) |
| Compensation plans: straight commission, salary, salary + commission, bonus | S. Roland Hall, *The Handbook of Sales Management* (1924) |

Rule for new claims: if it isn't in a source you can name, it doesn't get a number.
