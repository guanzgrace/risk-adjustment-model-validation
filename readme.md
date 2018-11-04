# Results

## Within Year Analysis


| Year | Group       | N   | Premium v Transfers r (p-value) | Costs v Transfers r (p-value) | Costs v Premiums r (p-value) |
|------|-------------|-----|---------------------------------|-------------------------------|------------------------------|
| 2014 | individual  | 403 | 0.2898 (<1e-4)                  | 0.6666 (<1e-4)                | 0.6300 (<1e-4)               |
|      | small group | 539 | 0.0098 (0.821)                  | 0.1524 (3e-4)                 | 0.7664 (<1e-4)               |
| 2015 | individual  | 453 | 0.3993 (<1e-4)                  | 0.7196 (<1e-4)                | 0.6316 (<1e-4)               |
|      | small group | 542 | 0.1138 (0.008)                  | 0.1947 (<1e-4)                | 0.6443 (<1e-4)               |
| 2016 | individual  | 420 | 0.4221 (<1e-4)                  | 0.8319 (<1e-4)                | 0.6372 (<1e-4)               |
|      | small group | 475 | 0.2429 (<1e-4)                  | 0.2509 (<1e-4)                | 0.5983 (<1e-4)               |

## Between Year Analysis

| Model Number | Model                       |
|--------------|-----------------------------|
| 6            | T16 ~ L14 + L15             |
| 7            | T16 ~ L14 + T14             |
| 8            | T16 ~ L14 + T14 + L15 + T15 |
| 9            | T15 ~ L14 + T14             |
| 10           | T16 ~ L15 + T15             |
| 11           | EM16 ~ Q1 + Q5              |
| 12           | EM16 ~ L14 + L15            |

Where each variable has the following definition:

| Variable | Meaning                                                                                      |
|----------|----------------------------------------------------------------------------------------------|
| T        | Transfers per member month in a given year                                                   |
| L        | Losses per member month in a given year (Premiums + Transfers + Reinsurance - Costs)         |
| EM       | Dichotomous variable: 1 if a company has exited the market in a given year; 0 otherwise      |
| Q        | Dichotomous variable: 1 if a company's 2014 losses puts it in a given quintile; 0 otherwise  |

Q1 indicates that a company has lost a lot of money, and Q5 indicates that a company has lost little money (perhaps even gained money).