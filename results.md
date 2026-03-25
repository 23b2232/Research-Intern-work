## Results

| Metric    | Value  |
| --------- | ------ |
| Accuracy  | 98.21% |
| Precision | 0.00   |
| Recall    | 0.00   |
| F1 Score  | 0.00   |


## Key Insight

The dataset is highly imbalanced, leading to:

* High accuracy
* Poor detection of actual transits (no true positives)


## Key Learnings

* Class imbalance severely impacts model performance
* CNNs are effective for time-series feature extraction
* Preprocessing (smoothing + normalization) is crucial
* Accuracy alone is misleading for imbalanced datasets
