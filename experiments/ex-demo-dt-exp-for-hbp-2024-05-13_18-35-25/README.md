
# Experiment: demo-dt-exp-for-hbp

## Parameters
- Historical data starting from: 2021-10-01 00:00:00
- Historical data ending at: 2022-02-01 00:00:00
- Streaming data starting from: 2022-02-01 00:00:00
- Streaming data ending at: 2022-11-01 00:00:00
- Minimum waiting time: 120 minutes
- Minimum required amount of data: 100
- Batch processing technique: HYBRID
- Concept drift handling strategy: ACTIVE
- Concept drift detection algorithm: DDM
- Strategy to update the outdated model: INCREMENTAL LEARNING
- Is buffer enabled: False
- DDM:

| Attribute | Value |
|---|---|
| Warning level factor | 0.1 |
| Drift level factor | 1.5 |
| Minimum numbers of instances/batches to start looking for changes | 1 |


## Results
- Model performance metrics:

| Model                                     | MAE (s)              | RMSE (s)              |
|-------------------------------------------|----------------------|-----------------------|
| Base model without concept drift handling | 28.941 | 43.283 |
| Base model with concept drift handling    | 21.326      | 37.762      |

- Error reduction percentage in terms of MAE: 26.314 %
- Average processing time after the batch preparation: 59.603 ms
    