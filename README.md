ver, for the static graph version swapping one optimizer for another works just fine.
Note how much faster Adam converges here (though it starts overfitting by epoch
4).

| Epoch | SGD train set loss | Adam train set loss | SGD train set accuracy | Adam train set accuracy | SGD dev set accuracy | Adam dev set accuracy |
| --- | --- | --- | --- | --- | --- | --- |
| 1 | 4.857 | 3.934 | 0.52 | 0.90 | 0.46 | 0.62 |
| 2 | 4.613 | 1.784 | 0.5 | 0.98 | 0.5 | 0.75 |
| 3 | 4.482 | 0.750 | 0.5 | 0.99 | 0.5 | 0.82 |
| 4 | 4.304 | 0.603 | 0.5 | 0.99 | 0.5 | 0.76 |
| 5 | 4.058 | 0.411 | 0.5 | 0.99 | 0.5 | 0.72 |

### Batching examples
It should not be too hard to add batching t
