# Test cases (referral rules)

| # | Scenario | Expected level | Next review |
|---|---|---|---|
| 1 | Pressure injury category 2, no warning signs | MONITOR | 3 days |
| 2 | Pressure injury category 1, pus or foul smell | URGENT | same day |
| 3 | Diabetic foot wound, no signs | REFER | 2 days |
| 4 | Pressure injury category 3 | REFER | 2 days |
| 5 | Leg ulcer, increasing pain | REFER | 2 days |
| 6 | No wound, 3 risk factors | HIGH risk | 7 days |
| 7 | No wound, 1 risk factor | MODERATE risk | 14 days |
| 8 | No wound, no risk factors | LOW risk | 30 days |
| 9 | Diabetic foot wound with fever | URGENT | same day |
| 10 | Pressure injury unstageable | REFER | 2 days |

Run `runTests()` in the browser console to check all 10.
