**Table 1.** Experiment results on fine-tuning OPT-2.7B with different anchor.
| Anchor         | SST-2 |           | RTE  |           | SQuAD |           |
|-----------------|-------|-----------|------|-----------|-------|-----------|
|          | Acc   | GPU hours | Acc  | GPU hours | Acc   | GPU hours |
| NA (MeZO)     | 90.0  | 100%      | 63.5 | 100%      | 68.7  | 100%      |
| **0**           | 87.9     | 85.7%         | 59.4    | 91.0%         | 63.2     | 81.8%         |
| $\theta_{t-1}$      | 90.7  | 87.8%     | 64.5 | 90.3%     | 67.2  | 88.4%     |
| $\theta_0$ (DiZO) | 92.5  | 55.7%     | 68.2 | 62.3%     | 69.0  | 65.4%     |


**Table 2.** Layer-wise distance gap of fine-tuning OPT-2.7B at different iteration (using the Value layer in the first attention module as an example).

| Iter. | 400   | 800  | 1200 | 1600 | 2000 | 2400 | 2800 | 3200 |
|-------|-------|------|------|------|------|------|------|------|
| MeZO  | 1.429 | 2.18 | 2.54 | 2.98 | 3.37 | 3.83 | 4.23 | 4.53 |
| DiZO  | 1.59  | 2.36 | 3.46 | 3.29 | 2.98 | 3.48 | 3.32 | 3.37 |

