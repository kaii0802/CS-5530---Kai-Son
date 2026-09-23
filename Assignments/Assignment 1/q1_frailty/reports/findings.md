# Q1 - Frailty Study: Findings

Sample: n = 10 female participants (4 frail, 6 not frail).

## 1. Summary statistics (numeric columns)

Units: Height_in = inches, Weight_lb = pounds, Age_yr = years, Grip_kg = kg, Height_m = metres, Weight_kg = kg, BMI = kg/m2.

| Variable       |   mean |   median |   std |
|:---------------|-------:|---------:|------:|
| Height_in      |  68.6  |    68.45 |  1.67 |
| Weight_lb      | 131.9  |   136    | 14.23 |
| Age_yr         |  32.5  |    29.5  | 12.86 |
| Grip_kg        |  26    |    27    |  4.52 |
| Height_m       |   1.74 |     1.74 |  0.04 |
| Weight_kg      |  59.83 |    61.69 |  6.46 |
| BMI            |  19.68 |    19.19 |  1.78 |
| Frailty_binary |   0.4  |     0    |  0.52 |

## 2. Processed data

|    |   Height_in |   Weight_lb |   Age_yr |   Grip_kg | Frailty   |   Height_m |   Weight_kg |   BMI | AgeGroup   |   Frailty_binary |
|---:|------------:|------------:|---------:|----------:|:----------|-----------:|------------:|------:|:-----------|-----------------:|
|  0 |        65.8 |         112 |       30 |        30 | N         |    1.67132 |     50.8023 | 18.19 | 30–45      |                0 |
|  1 |        71.5 |         136 |       19 |        31 | N         |    1.8161  |     61.6886 | 18.7  | <30        |                0 |
|  2 |        69.4 |         153 |       45 |        29 | N         |    1.76276 |     69.3996 | 22.33 | 30–45      |                0 |
|  3 |        68.2 |         142 |       22 |        28 | Y         |    1.73228 |     64.4101 | 21.46 | <30        |                1 |
|  4 |        67.8 |         144 |       29 |        24 | Y         |    1.72212 |     65.3173 | 22.02 | <30        |                1 |
|  5 |        68.7 |         123 |       50 |        26 | N         |    1.74498 |     55.7919 | 18.32 | 46–60      |                0 |
|  6 |        69.8 |         141 |       51 |        22 | Y         |    1.77292 |     63.9565 | 20.35 | 46–60      |                1 |
|  7 |        70.1 |         136 |       23 |        20 | Y         |    1.78054 |     61.6886 | 19.46 | <30        |                1 |
|  8 |        67.9 |         112 |       17 |        19 | N         |    1.72466 |     50.8023 | 17.08 | <30        |                0 |
|  9 |        66.8 |         120 |       39 |        31 | N         |    1.69672 |     54.4311 | 18.91 | 30–45      |                0 |

AgeGroup counts: <30 = 5, 30-45 = 0, 46-60 = 0, >60 = 0. No participant is older than 60, so the AgeGroup_>60 one-hot column is all zeros ## 3. Relationship between grip strength and frailty

| Frailty   |   count |   mean |   median |   std |
|:----------|--------:|-------:|---------:|------:|
| N         |       6 |  27.67 |     29.5 |  4.63 |
| Y         |       4 |  23.5  |     23   |  3.42 |

Correlation coefficient between Grip_kg and Frailty_binary: **-0.48**

**Interpretation.** The correlation is lower: participants with higher grip strength tend to be coded 0 (not frail), and those with lower grip strength tend to be coded 1 (frail). The frail group averages 23.5 kg versus 27.7 kg for the non-frail group. With only n = 10, this is a plausible signal from a small sample, not a firm conclusion.

## Conclusion

Lower grip strength goes with more frailty in this small sample (correlation = -0.48), matching the pattern the assignment describes. A larger sample would be needed to confirm it.
