# Results

## Within Year Analysis

Values in the right-most 3 columns are: Pearson r correlation coefficient (p-value).

| Year | Group       | N   | Premium v Transfers | Costs v Transfers | Costs v Premiums |
|------|-------------|-----|---------------------|-------------------|------------------|
| 2014 | individual  | 403 | 0.2898 (<1e-4)      | 0.6666 (<1e-4)    | 0.6300 (<1e-4)   |
|      | small group | 539 | 0.0098 (0.821)      | 0.1524 (3e-4)     | 0.7664 (<1e-4)   |
| 2015 | individual  | 453 | 0.3993 (<1e-4)      | 0.7196 (<1e-4)    | 0.6316 (<1e-4)   |
|      | small group | 542 | 0.1138 (0.008)      | 0.1947 (<1e-4)    | 0.6443 (<1e-4)   |
| 2016 | individual  | 420 | 0.4221 (<1e-4)      | 0.8319 (<1e-4)    | 0.6372 (<1e-4)   |
|      | small group | 475 | 0.2429 (<1e-4)      | 0.2509 (<1e-4)    | 0.5983 (<1e-4)   |

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
| T        | Transfers per member month in a given year (14, 15, 16)                                      |
| L        | Losses per member month in a given year (Premiums + Transfers + Reinsurance - Costs)         |
| EM       | Dichotomous variable: 1 if a company has exited the market in a given year; 0 otherwise      |
| Q        | Dichotomous variable: 1 if a company's 2014 losses puts it in a given quintile; 0 otherwise  |

Q1 indicates that a company has lost a lot of money, and Q5 indicates that a company has lost little money (perhaps even gained money).

| Model | Coeff   | N (ind) | Estimate | Std Err | t-value | p-value | N (small grp) | Estimate | Std Err | t-value | p-value |
|-------|---------|---------|----------|---------|---------|---------|---------------|----------|---------|---------|---------|
| *6    | (Const) | 290     | 2.6661   | 3.515   | 0.758   | 0.449   | 431           | -6.2944  | 2.876   | -2.189  | 0.029!  |
|       | L14     |         | -0.1604  | 0.048   | -3.375  | 0.001!  |               | 0.0290   | 0.030   | 0.971   | 0.332   |
|       | T15     |         | 1.1779   | 0.036   | 32.998  | 0.000!  |               | 0.765    | 0.042   | 18.032  | 0.000!  |
| *7    | (Const) | 293     | 3.0379   | 6.070   | 0.501   | 0.617   | 432           | -4.3722  | 3.451   | -1.267  | 0.206   |
|       | L14     |         | -0.2083  | 0.079   | -2.644  | 0.009!  |               | 0.0003   | 0.036   | 0.010   | 0.992   |
|       | T14     |         | 1.0920   | 0.080   | 13.634  | 0.000!  |               | 0.7471   | 0.062   | 11.986  | 0.000!  |
| *8    | (Const) | 290     | 2.0190   | 3.532   | 0.572   | 0.568   | 431           | -6.2978  | 3.270   | -1.926  | 0.055   |
|       | L14     |         | -0.1135  | 0.056   | -2.023  | 0.044!  |               | -0.0542  | 0.037   | -1.462  | 0.144   |
|       | T14     |         | -0.0179  | 0.069   | -0.259  | 0.796   |               | 0.2689   | 0.067   | 4.034   | 0.000!  |
|       | L15     |         | -0.0702  | 0.040   | -1.762  | 0.079   |               | 0.0874   | 0.036   | 2.418   | 0.016!  |
|       | T15     |         | 1.1892   | 0.053   | 22.485  | 0.000!  |               | 0.5865   | 0.058   | 10.184  | 0.000!  |
| **9   | (Const) | 376     | -2.4764  | 3.351   | -0.739  | 0.460   | 499           | -6.7551  | 2.847   | -2.372  | 0.018!  |
|       | L14     |         | 0.0220   | 0.042   | 0.529   | 0.597   |               | 0.0476   | 0.029   | 1.617   | 0.107   |
|       | T14     |         | 0.9135   | 0.046   | 19.712  | 0.000!  |               | 0.7656   | 0.054   | 14.096  | 0.000!  |
| *10   | (Const) | 362     | 0.9639   | 3.006   | 0.321   | 0.749   | 458           | -8.9256  | 3.012   | -2.963  | 0.003!  |
|       | L15     |         | -0.1297  | 0.033   | -3.931  | 0.000!  |               | 0.0565   | 0.030   | 1.904   | 0.058   |
|       | T15     |         | 1.1158   | 0.034   | 32.412  | 0.000!  |               | 0.06236  | 0.045   | 13.952  | 0.000!  |
| ^11   | (Const) | 403     | 0.2863   | 0.029   | 10.012  | 0.000!  | 539           | 0.1238   | 0.022   | 5.744   | 0.000!  |
|       | Q1      |         | 0.0470   | 0.057   | 0.825   | 0.410   |               | 0.2465   | 0.043   | 5.724   | 0.000!  |
|       | Q5      |         | -0.1135  | 0.057   | -1.990  | 0.047!  |               | 0.1262   | 0.043   | 2.929   | 0.004!  |
| ^12   | (Const) | 376     | 0.2520   | 0.022   | 11.216  | 0.000!  | 499           | 0.2042   | 0.027   | 7.547   | 0.000!  |
|       | L14     |         | -0.0010  | 0.000   | -3.142  | 0.002!  |               | -0.0006  | 0.000   | -1.623  | 0.105   |
|       | L15     |         | 3.938e-5 | 0.000   | 0.147   | 0.883   |               | -0.0003  | 0.000   | -1.234  | 0.218   |

* Dependent Variable: T16

** Dependent Variable: T15

^ Dependent Variable: EM16

! Significant at alpha = 0.05

Columns 3-7 represent the model fitted with data from the individual marketplace; Columns 8-12 represent the model fitted with data from the small group marketplace.

