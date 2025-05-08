In machine learning, a **learning curve** is a plot that shows how a model’s performance changes as it is exposed to more training data (or, in some cases, more training iterations). By examining learning curves, you can diagnose whether your model is:  
**Underfitting (high bias)**  
**Overfitting (high variance)**  
**Well-balanced**  
  

| Scenario         | Training Error    | Validation Error | Train-Val Gap | Behavior as Data ↑             | Typical Fixes                                          |
| ---------------- | ----------------- | ---------------- | ------------- | ------------------------------ | ------------------------------------------------------ |
| **Underfitting** | High              | High             | Small         | Flat (little change)           | ↑ Model complexity<br>↓ Regularization<br>Add features |
| **Good Fit**     | Low               | Low              | Small         | Both decrease & converge       | —                                                      |
| **Overfitting**  | Very low (near 0) | High             | Large         | Gap persists or narrows slowly | ↑ Regularization<br>Simplify model<br>More data        |
