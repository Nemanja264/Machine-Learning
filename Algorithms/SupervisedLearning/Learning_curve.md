Thought for a few seconds


Here’s a concise summary of the three scenarios in one table:

| Scenario         | Training Error    | Validation Error | Train-Val Gap | Behavior as Data ↑             | Typical Fixes                                          |
| ---------------- | ----------------- | ---------------- | ------------- | ------------------------------ | ------------------------------------------------------ |
| **Underfitting** | High              | High             | Small         | Flat (little change)           | ↑ Model complexity<br>↓ Regularization<br>Add features |
| **Good Fit**     | Low               | Low              | Small         | Both decrease & converge       | —                                                      |
| **Overfitting**  | Very low (near 0) | High             | Large         | Gap persists or narrows slowly | ↑ Regularization<br>Simplify model<br>More data        |
